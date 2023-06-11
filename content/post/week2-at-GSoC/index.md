---
title: "GSoC: Week2"
date: 2023-06-11T14:23:52+05:30
Description: "My Second Week at Google Summer of Code 2023 at OpenSUSE"
thumbnail: "images/post4/week2.png"
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series: 
    - "gsoc-weekly-report"
DisableComments: false
---

Hello All, As I step into the completion of 2<sup>nd</sup> week at Google Summer of Code 2023 at OpenSUSE, I would like to share my work progress and experience in this blog post.


---


This week, my main focus was on gaining a clearer understanding of the codebase, particularly the [`Pkg`](https://github.com/afrid18/rpmlint/blob/main/rpmlint/pkg.py) module in the `rpmlint` package. It has been quite a journey delving into the inner workings of the RPM package object. I feel that I've made significant progress in grasping the concept, but there are still several other methods within the `Pkg` object that I need to explore. I believe I should dedicate more time to comprehensively understand the codebase, which will ultimately guide my contributions.

Once I feel confident with the codebase, my plan is to either implement patching using pytest-mock's `patch` or enhance the functionality of `FakePkg` to mimic the behavior of `Pkg`.

In my opinion, utilizing pytest-mock's `patch` is the optimal approach for implementing mocking in the current `Pkg`. This approach will not only improve the implementation of testing for new features and other tests, but also save time and computational resources. Otherwise, manually creating a mock package for each individual package using `FakePkg` would be a more time-consuming and computationally intensive task.

I'm looking forward to diving deeper into the project and making meaningful contributions in the coming weeks. Stay tuned for more updates in my next blog post!

<h1 align="center"> Thank you </h1>

Links

* https://github.com/afrid18/rpmlint/blob/main/rpmlint/pkg.py

---
