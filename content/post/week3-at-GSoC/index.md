---
title: "GSoC: Week3"
date: 2023-06-21T17:59:05+05:30
Description: "My third week at Google Summer of Code 2023 at OpenSUSE"
thumbnail: "images/post5/week3.png"
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series:
  - "gsoc-weekly-report"
DisableComments: false
---

Hello I am back again with my another GSoC weekly report and in this blog post I will share what I worked on the previous week.

As discussed in the previous [previous post], my mentor and I have decided to go with extending implementation of `FakePkg` class, just to keep everything simple. Whereas with mocking, it would be hard to mock every peice inner piece of functions and other required binary operations. Which eventually consume more design to `Pkg` class itself and this approach will also take more time. However, there a big scope to the project and hence there might be improvements in future.

[previous post]: /post/week2-at-gsoc/

This week, I have made decent progress, also I was able to eliminate 3 following binary rpm packages

- `rpmlint/test/binary/pythoncheck-python-doc-in-site-packages-0-0.x86_64.rpm`
- `rpmlint/test/binary/pythoncheck-python-src-in-site-packages-0-0.x86_64.rpm`
- `rpmlint/test/binary/pythoncheck-python-tests-in-site-packages-0-0.x86_64.rpm`

{{% notice info %}}

> These packages are basically files within python packages that are not necessary to be packaged with rpm files.

{{% /notice %}}

Here is the commit **[db63a42](https://github.com/afrid18/rpmlint/commit/db63a4226b2fc50e169dca348fb5aa9a256fccc9)** if you are interested.

Looking ahead to the coming week, my plan is to focus on developing more complex tests and, hopefully, work alongside my mentor to create some well-designed and effective mocked tests.

<h1 align="center"> Thank you </h1>

links:

---
