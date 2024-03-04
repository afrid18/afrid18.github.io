---
title: "GSoC:  Week1"
date: 2023-06-03T12:20:45+05:30
cover:
  image: "images/post3/week1.png"
  relative: false
Description: "Blog series of my GSoC Journey"
Tags: ["GSoC", "OpenSUSE"]
Categories: ["Open Source", "Software Developement"]
Series: 
    - "gsoc-weekly-report"
DisableComments: false
---

Hi 👋🏻, Welcome back again, It has been a week since official start of coding period at Google Summer of Code. In this blog post, I am going to share my experience as a GSoC contributor at [@OpenSUSE](https://opensuse.org). OpenSUSE has been great to me, people in it are awesome, my mentor is awesome too, he has got my back everytime I am stuck. I am really thankful for having such mentor. Now, Since past week I have been contributing to [rpmlint](https://github.com/rpm-software-management/rpmlint). I will share my coding experience here in this blog post..

---

## WEEK-1 contributing to RPMLint

My Week started off with my mentor assigning me a small task, in which I have to use pre-defined class and define a new helper function to easily creat a mock rpm package object. Be patient for couple of minutes, lets go deeper into what I have did and internal details of project.

I and my mentor had a talk on how to mock packages, and we have decided to move ahead with existing method and improve on it. And the whole idea of the project is same, to improve testing that uses mocking, and mocking will be done with existing `Pkg` and `FakePkg` that are currently available in codebase.


The past week, I have created a new utility or a helper function that basically take rpm details and convert it into a `Pkg` or `FakePkg` object.

Here look at an overview of the process

{{< figure src="images/week1-gsoc.png" title="Basic pictorial explaination of test suite" align="center">}}

Here is the previous code...
```python3
def test_systemd_unit_file(binariescheck):
    output, test = binariescheck
    with FakePkg('fake') as pkg:
        pkg.add_file_with_content('/usr/lib/systemd/system/yast-timesync.service', '')
        output, test = binariescheck
        test.check(pkg)
        out = output.print_results(output.results)
        assert 'only-non-binary-in-usr-lib' not in out
```

and the modified code.

```python3
@pytest.mark.parametrize('package', [
    get_tested_mock_package(files={
        '/usr/lib/systemd/system/yast-timesync.service': { 'content': '' }
    })
])
def test_systemd_unit_file(package, binariescheck):
    output, test = binariescheck
    test.check(package)
    out = output.print_results(output.results)
    assert 'only-non-binary-in-usr-lib' not in out
```

For more information look at my commits here: [My commits to GSoC Branch](https://github.com/afrid18/rpmlint/commits?author=afrid18)

As you can see I have to create this helper function `get_tested_mock_package` and I have come up with this

```python3
def get_tested_mock_package(files=None):
    mockPkg = FakePkg('mockPkg')
    if files is not None:
        for path, file in files.items():
            mockPkg.add_file_with_content(path, file.get('content'))
    return mockPkg
```


This is so far I was able to go into codebase. I will be posting many more updates soon here on my blog. I have yet learn and contribute to rpmlint and I have a big learning week ahead.

See you in the next one!✌🏻


<h1 align="center"> Thank You </h1>

___

links:
- https://opensuse.org
- https://github.com/rpm-software-management/rpmlint
- https://github.com/afrid18/rpmlint/commits?author=afrid18
