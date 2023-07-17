---
title: "GSoC: Week6"
date: 2023-07-17T15:56:39+05:30
Description: "In this blog, I would like to share my progress of Google Summer of Code 2023, for week 6"
thumbnail: "images/post8/week6.png"
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series:
  - "gsoc-weekly-report"
---

Hi, in this series, I have been sharing my Google Summer of Code progress, in this post I will share my progress on project [rpmlint] for the week6.

[rpmlint]: https://github.com/rpm-software-management/rpmlint

## Overview

Week 6, which is the final week of the Google Summer of Code (for a standard 12 weeks) first phase, which means my project progress should also be half way through, which is not indeed. Let me explain.

My project is quite a large project, definitely all the work cannot be achieved in just 12 weeks, but I make sure to complete as much as possible. I have explained about the work to be done in my [previous post] please refer to it.

[previous post]: /post/week5-at-gsoc/

## Progress [######............]

This week I have mocked all the tests that were left in [`test_python.py`](https://github.com/afrid18/rpmlint/blob/main/test/test_python.py), where I have removed 15 binary files :fire:.

Pull request is still in Draft stage, very soon, my mentor will review the changes and hopefully I will be making it out to review. Here is my [pull request] if you are interested 

[pull request]: https://github.com/rpm-software-management/rpmlint/pull/1079

My next step is to work on warnings, there are many warnings that are being generated for pytest. Many of them are because of `libmagic` or `python-magic`. And these warnings are only generated in opensuse distributions. I think there might be a library mismatch. I don't know for sure what the problem is. I am still figuring it out.

Apart from GSoC23, I am contributing to RPMLint in any other case possible. 
* I have opened 1 [issue] it might have resolved if you are viewing in future 
* opened a pull request for a small warning which is [merged],
* opened a pull request for adding test coverage badge on README; [merged2]

[issue]: https://github.com/rpm-software-management/rpmlint/issues/1083
[merged]: https://github.com/rpm-software-management/rpmlint/pull/1084
[merged2]: https://github.com/rpm-software-management/rpmlint/pull/1086

For the week7, I would be working on RPMTags, specifically on `test_tags.py`, which covers `TagsCheck.py`. I will share more about it in week7 blog.

Thats it for this week.


## Miscellaneous

Also, the next week I will be having my GSoC Mid Term Evaluation. Hopefully it should all go well.

As said in my previous blog, that I have started my development workflow on Digital Ocean. I also have docker instances but they are not so powerful in terms of features, as they are shipped with very few libraries, bindings etc. They don't give much power. However I use docker containers with podman and for faster editing and testing I use them.

<h1 style="text-align: center"> Thank You </h1>

---
