# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20240324213138**) for **Windows**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **dev branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **dev**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-dev
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-dev
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-dev

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/8c1cfbbaa64250021d166246b4475c43f75d98d0**
* **BUILD_DATE = Sun Mar 24 08:37:10 PM UTC 2024**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: dev)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/619639727**
* **BUILD_OS = (linux) Linux lgb 6.2.0-1018-gcp #20~22.04.1-Ubuntu SMP Mon Oct 23 12:29:43 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Windows**
* **BUILD_UPTIME =  20:37:10 up 4 min,  1 user,  load average: 1.86, 1.21, 0.52**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = dev
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 269630635
* TRAVIS_BUILD_NUMBER = 1389
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/269630635
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Windows
* TRAVIS_COMMIT = 8c1cfbbaa64250021d166246b4475c43f75d98d0
* TRAVIS_COMMIT_MESSAGE = Testing row mask change
* TRAVIS_COMMIT_RANGE = 481b1774444b...8c1cfbbaa642
* TRAVIS_COMPILER = gcc
* TRAVIS_CPU_ARCH = amd64
* TRAVIS_DIST = jammy
* TRAVIS_ENABLE_INFRA_DETECTION = true
* TRAVIS_EVENT_TYPE = push
* TRAVIS_FILTERED = redirect_io
* TRAVIS_HOME = /home/travis
* TRAVIS_INFRA = unknown
* TRAVIS_INIT = systemd
* TRAVIS_INTERNAL_RUBY_REGEX = ^ruby-(2\.[0-4]\.[0-9]|1\.9\.3)
* TRAVIS_JOB_ID = 619639727
* TRAVIS_JOB_NAME = Windows cross-compilation on Linux
* TRAVIS_JOB_NUMBER = 1389.2
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/619639727
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2023-11-02T13:43:09
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_PRIVATE = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = generic basic ruby_interpreter
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2204__ c c++ cplusplus cpp ruby python go java php node_js smalltalk shell csharp perl rust elixir erlang
* TRAVIS_STACK_NAME = ubuntu_2204
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2023-11-02 13:43:20 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 2dbea57a
* TRAVIS_TIMER_START_TIME = 1711312630634991530
* TRAVIS_TMPDIR = /tmp/tmp.jQxzTKro8X
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 8c1cfbbaa64250021d166246b4475c43f75d98d0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Mar 24 21:31:38 2024 +0100

    Testing row mask change

commit 481b1774444bb3a53d1ff2ef4a83bcf58000d6ee
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Mar 19 15:13:31 2024 +0100

    MEGA65: further new memory works #209 #378
    
    More optimizations and modifications:
    
    * It seems the old method is superior: using linear addresses to the
      actual slot backend readers/writers
    * Introducing optional data-pointer driven mechanism for further
      emulation performance
    * Unfinished "memory-watch" mode
    * Various minor modifications and/or optimizations

commit 2f380361dce682216fa37d847820296ec5ba64e4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Mar 16 00:37:37 2024 +0100

    MEGA65: first try of new mem decoder #209
    
    It seems to work without too much testing yet. The bad news though: it's
    seems to a be a bit slower than the old one :( I expected to opposite.
    
    This also uses the baking/mapping behaviour as mentioned in #378

commit 78a8adce0faf4cf5ae9abf2342f7811625504736
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Mar 16 00:24:33 2024 +0100

    Trying github with ubuntu jammy

commit b970f56e2a506a991cec7b562b517c23ce698d16
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Mar 4 20:18:58 2024 +0100

    MEGA65: DMA audio stop + 16 bit samples #398
    
    DMA audio stop (or loop) conidition is checked against the limit after
    incrementing the address. However in case of 16 bit samples it can
    happen that it skips the limit, if the limit is odd and start address is
    even or vice versa.
    
    Reported by @dansanderson

commit 6a71a4954ad28825b2739e0730a26a79f483483e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Feb 13 15:10:09 2024 +0100

    MEGA65: allow OPL work on slow-dev space, too #380
    
    Note, currently I don't know why the slow device space is used for OPL
    why not the native I/O space, or the MEGA65 specific OPL regs
    at $FE000xx which is intended for that very purpose!
    
    btoschi on Discord has great success to make OPL working on MEGA65 but
    requires this access mode, so this quick hack is intended to serve that
    holy purpose :)

commit 322db3f4fb596ff3ca2883598b4ae30a5431f641
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Feb 1 19:15:12 2024 +0100

    Catching up /w next + matrix devel

commit 22431867100db0902eec3265927cbb57704cb1e4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Sep 23 20:47:25 2023 +0200

    vic4 mods so far, before something else

commit 31f8144114b1523363ba50da5884702d407f6ca5
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Sep 15 14:54:09 2023 +0200

    petscii kbd scanner

commit 389c4eff8cebbff074076b92e39630c615c92082
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Sep 13 00:11:31 2023 +0200

    Compressed disk image format still

commit 9aa381f58e8600820139be37580e1d9ea4f272ba
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Sep 11 09:08:10 2023 +0200

    ...

commit 4b17b38ea0d6bc566bfa70b364c8cf9ba5638bef
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Sep 9 19:07:42 2023 +0200

    WINDOWS: allow regkey to silent OS warnings
    
    Cherry-pick from next, commit 9a1a079e14d6e079054e19967b41d830e960d84b

commit fde85b7174a7e9f9c0a68b9b15728351fe0bdfbd
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Sep 10 01:34:46 2023 +0200

    New compressed SD image format

commit 8e1829ff52aa8cd0356ba36fef379171ae1c0f78
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 7 21:29:28 2023 +0200

    Merges with next

commit 2b3f51812289f0369c39003d23370e8426f706c3
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Sep 6 00:45:11 2023 +0200

    Misc + uartmon 'g' command

commit d2655dde1c4543fff911deb5eafcfe53c8993e02
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Sep 3 18:56:17 2023 +0200

    EMSCRIPTEN: Various misc web target fixes

commit 3e369295478091fcc529c4e8ed90ec4a0aac3f51
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Sep 1 10:06:58 2023 +0200

    Quick fixed to compile MEGA65 emu with emscripten

commit 292439b2c38117fc7b2c0b60f7e021949f657f59
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Sep 1 10:06:32 2023 +0200

    Detect grep by configure

commit 60b3445e126e50442994a7c9fdc1106045c06db4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Aug 30 00:01:41 2023 +0200

    MacOS 'sed' problem in 'configure'.
    
    It seems at least some MacOS sed utilities are broken and does not know
    the '-r` flag at all. Let's try to use '-E' ... It's on the travis MacOS
    instance.

commit b046e1ae7c562cab573b6097cc0446111c167e00
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 29 23:45:45 2023 +0200

    ...

commit 83294883c7da13c944380cbb33f27fe42939f5fd
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Aug 28 11:23:31 2023 +0200

    ...

commit cdd141098cf15172177a07752671a1a392701a36
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 22 11:19:46 2023 +0200

    PRINTF_LLD -> PRINTF_S64, PRINTF_LLU -> PRINTF_U64

commit 79d60a87b1c3b65614a93c18766360a4447f7ede
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 22 11:11:37 2023 +0200

    VIC framecount rework, inject timeout prelim. work

commit edc40e9d9a17629703b2832a40aafe3be1221816
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Aug 18 10:11:23 2023 +0200

    Try to fix 64 bit print format IDs again ...
    
    Still TODO:
    
    * rename PRINTF_LLD -> PRINTF_S64, PRINTF_LLU -> PRINTF_U64
    * review casting
    * drop 64 bit formatting at not needed parts
    * test on MacOS with its clang (faked to be called "gcc")
    * test with gcc _and_ mingw-gcc (32+64 bits!) in Ubuntu 22.04

commit cac121472957ac21e543de2d1bc7798b186efd5c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Aug 18 00:50:35 2023 +0200

    Prepare for kbd hw queues to have different empty markers
