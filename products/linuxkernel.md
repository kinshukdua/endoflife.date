---
title: Linux Kernel
layout: post
permalink: /linux
category: os
iconSlug: linux
link: https://www.kernel.org/
releaseImage: https://upload.wikimedia.org/wikipedia/en/timeline/7fd581c797074c2059bfdcf078447733.png
changelogTemplate: |
  https://cdn.kernel.org/pub/linux/kernel/v{{"__LATEST__"| split: "." | first}}.x/ChangeLog-{{"__LATEST__"}}
activeSupportColumn: false
releaseDateColumn: true
releaseColumn: true
sortReleasesBy: 'cycleShortHand'
command: uname -r
releases:
  - releaseCycle: "5.14"
    cycleShortHand: 514
    release: 2021-08-29
    eol: false
    latest: "5.14.9"
    
  - releaseCycle: "5.13"
    cycleShortHand: 513
    release: 2021-06-28
    eol: 2021-09-18
    latest: "5.13.19"
    
  - releaseCycle: "5.10"
    cycleShortHand: 510
    release: 2020-12-13
    eol: 2026-12-01
    lts: true
    latest: "5.10.70"
    
  - releaseCycle: "5.4"
    cycleShortHand: 504
    release: 2019-11-24
    eol: 2025-12-01
    lts: true
    latest: "5.4.150"
    
  - releaseCycle: "4.19"
    cycleShortHand: 419
    release: 2018-10-22
    eol: 2024-12-01
    lts: true
    latest: "4.19.208"
    
  - releaseCycle: "4.14"
    cycleShortHand: 414
    release: 2017-11-12
    eol: 2024-01-01
    lts: true
    latest: "4.14.248"
    
  - releaseCycle: "4.9"
    cycleShortHand: 409
    release: 2016-12-11
    eol: 2023-01-01
    lts: true
    latest: "4.9.284"
    
  - releaseCycle: "4.4"
    cycleShortHand: 404
    release: 2016-01-10
    eol: 2022-02-01
    lts: true
    latest: "4.4.285"


---

> The Linux kernel is a free and open-source, monolithic, modular, multitasking, Unix-like operating system kernel.
Linux is deployed on a wide variety of computing systems, such as embedded devices, mobile devices (including Android), personal computers, servers, mainframes, and supercomputers.

There are several main categories into which kernel releases may fall:

- **Prepatch or "RC"** kernels are mainline kernel pre-releases that are mostly aimed at other kernel developers and Linux enthusiasts. They must be compiled from source and usually contain new features that must be tested before they can be put into a stable release.

- **Mainline tree**  It's the tree where all new features are introduced and where all the exciting new development happens. New mainline kernels are released every 2-3 months.    

- **Stable** is labeled after each mainline kernel is released. Any bug fixes for a stable kernel are backported from the mainline tree. There are usually only a few bugfix kernel releases until next mainline kernel becomes available -- unless it is designated a "longterm maintenance kernel". Stable kernel updates are released on as-needed basis, usually once a week.
        
- **Longterm (LTS)** are usually several longterm maintenance kernel releases provided for the purposes of backporting bugfixes for older kernel trees. By default these are only supported for two years (as opposed to the 4 months of a non-LTS release) [but are usually extended depending on how long companies pledge to back it.](https://lore.kernel.org/lkml/YA%2FE1bHRmZb50MlS@kroah.com/) Only important bugfixes are applied to such kernels and they don't usually see very frequent releases, especially for older trees. 

