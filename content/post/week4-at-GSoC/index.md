---
title: "GSoC: Week4"
date: 2023-06-30T12:10:45+05:30
Description: "My forth week at Google has been good. In this blog I will share my learnings and progress for the same"
# thumbnail: "images/post6/week4.png"
cover:
  image: "images/post6/week4.png"
  relative: false
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series:
  - "gsoc-weekly-report"
---

Alright, Week 4 has completed. And I know that I am late in publishing my blog post. Week 4 has been little chaos to me in the context of work because I have been with my friends and couldn't completly focus on my work. I haven't made much progress with my project, but I have learned my lessons. Let me explain my progress in detail.


In the [week3] blog post I have told that we (I and my mentor) have extended `FakePkg` class and this made room for more complex testing capabilities, now it is possible to just add things or just hardcode and it simply works, this way is still good when compared to the previous test suite.

[week3]: /post/week3-at-gsoc/

I have finally opened a [draft pull request], where it consists all the commits that I have previously made. It is still a draft, because there are some more points to include into this pull request. My mentor has roughly planned to open review for the pull request in coming week or so, but not very long.

[draft pull request]: https://github.com/rpm-software-management/rpmlint/pull/1079

The next week which is week5, I have to contribute to more complex tests. like tests that check for dependencies of python packages (Yes, I am still in writing tests for `PythonCheck.py` file), for both kinds of python packages 
1. Dependencies from `METADATA`
2. Dependencies from `requires.txt`

Not sure about the way of python packaging, but rpmlint currently has support for these two files.

Hopefully, next week I may be able to remove some more binary rpm files, that are considerably large for their usecase. Like some of the binaries that I am planning to get rid have like 130 kilobytes. They are there just for a single file in them (either for `METADATA` or `requires.txt`). 

And also GSoC Evaluation is coming too. It's planned to be aroung July 10<sup>th</sup> to July 14<sup>th</sup>. I will try my best to work on this and for the next week too.

See you again in the next one! :grinning_face_with_smiling_eyes:


Links:
- [week3]
- [draft pull request]


---
