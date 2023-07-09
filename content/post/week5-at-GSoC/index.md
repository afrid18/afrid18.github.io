---
title: "GSoC: Week5"
date: 2023-07-09T17:24:20+05:30
Description: "My fifth week at Google has been good. In this blog I will share my learnings and progress for the same"
thumbnail: "images/post7/week5.png"
Tags: ["OpenSUSE", "Open Source", "Google", "Summer of Code"]
Categories: ["Open source", "Programming"]
Series:
  - "gsoc-weekly-report"
---

Hi, I was supposed to write this (week5) blog 6 days back, as you know, I am lagging and I will soon write another blog which is week6. Where I shall discuss about my evalutaion, whats and hows. 

In this blog, let me share week5's work :rocket:, I am really excited, because I have done some decent work in week5.

## Overview

I have been working on `test_python.py` ever since I started my GSoC project and I have covered almost 95% of the tests. There are only 2 more binaries left for this test to be covered with mock tests. After completly mocking tests in `test_python.py`, I would have mocked and removed 10+ binaries.


## Progress [#####..............]

I am made a decent progress, mocking Python related check. Yet, there are a lot of other checks that needs to be mocked. I am hoping to work at a faster pace than I am currently at. The list is a exhaustive one. Here is the list of all the checks in `rpmlint` [repo].

```
     1	AbstractCheck.py
     2	AlternativesCheck.py
     3	AppDataCheck.py
     4	BashismsCheck.py
     5	BinariesCheck.py :check_mark_button:
     6	BuildRootAndDateCheck.py
     7	ConfigFilesCheck.py
     8	DBusPolicyCheck.py
     9	DocCheck.py
    10	DuplicatesCheck.py
    11	ErlangCheck.py
    12	FHSCheck.py
    13	FilesCheck.py
    14	I18NCheck.py
    15	IconSizesCheck.py
    16	InitScriptCheck.py
    17	LSBCheck.py
    18	LibraryDependencyCheck.py
    19	LogrotateCheck.py
    20	MenuCheck.py
    21	MenuXDGCheck.py
    22	MixedOwnershipCheck.py
    23	PAMModulesCheck.py
    24	PkgConfigCheck.py
    25	PostCheck.py
    26	PythonCheck.py :check_mark_button:
    27	SharedLibraryPolicyCheck.py
    28	SignatureCheck.py
    29	SourceCheck.py
    30	SpecCheck.py
    31	SysVInitOnSystemdCheck.py
    32	TagsCheck.py
    33	TmpFilesCheck.py
    34	XinetdDepCheck.py
    35	ZipCheck.py
    36	ZyppSyntaxCheck.py
```

Not all of these checks have binaries used in them, but most of them have binaries used for testing.


## Miscellaneous

The other thing I have worked in this week is that I have setup a work environment. Yes, It is something to be mentioned here, as it took a lot of time to setup. Let me explain my development setup briefly. I shall make a dedicated post about my Developement setup sometime soon!

I started off with virtualizing my MacBook air, but that resulted in heating up my Macbook to more than 50<sup>o</sup>**C**. I then created a GitHub Codespaces with a Opensuse tumbleweed. It was all going good, but It has soon hit usage limit :neutral_face:. GitHub gives 180 core hours, and I configured a 2 cores machine which is a base one. Still It hit a usage limit just only after 13 days. I used to spend quite a lot of time in codespaces.

I had to soon pull my changes, to another working environment. So, I created a DigitalOcean account and created a fedora droplet and started configuring. All went good. Now I have both remote tunnel setup and a remote machine that I can do pretty much everything, play around, ssh into it and more

[repo]: https://github.com/rpm-software-management/rpmlint/tree/main/rpmlint/checks

<h2 style="text-align: center"> Thank You </h2>

links:
- [repo]

---
