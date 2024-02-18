---
title: "GSoC: Week10"
date: 2023-08-12T19:45:47+05:30
Description: "In this blog post, I would like to share my weekly progress of Google Summer of code with OpenSUSE"
# thumbnail: "images/post13/week10.png"
cover:
  image: "images/post13/week10.png"
  relative: false
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series:
  - "gsoc-weekly-report"
---

Welcome back to the. In this blog, I would like to share my week10 progress of Google Summer of Code with OpenSUSE.

Firstly, I can't stop worrying about the end of Google Summer of Code, GSoC has given me so much. I learnt good stuff from my mentor, I learned new technologies and many other soft skill and at the same time I was enjoying the process. Its really sad that GSoC is coming to end. Anyways, I will enjoy the rest of the time.

## Progress [##########....]

This week, I worked on mocking few more tests, I started off with `config_files`, and also tried to mock `test_files` but latter is far more complex to just replace with mocking because this requires some more capabilities of `FakePkg`, which may take in depth understanding of `RPMLint` codebase.

Talking about `config_files.py`, I have successfully mocked the tests and was able to remove 1 binary rpm file. This was relatively easy than `test_files.py`. I spent lot of time working on `test_files.py` just to figure out a simple and easy way to mock, but It seems

## Misc.

My mentor was telling me about documenting the new test framework, so the coming week I shall work on documenting about the new test suite design and how to write new tests using the implemented `FakePkg`.

Also, My project is most likely to be merged next week, if all the runner checks passes. 🤞

The most intereting part of Google Summer of Code is that I get to visit SUSE office at Bangalore. I will be vising around 22 of August. I will give the exact date next week.

<h1 align="center"> Thank You </h1>

---
