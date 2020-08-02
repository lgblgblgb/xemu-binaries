# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu for **MacOS**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu









## Binary versions for **master**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/0d43fb97c26349a7cc820356f9113db86a95fc7d**
* **BUILD_DATE = Sun Aug  2 16:16:05 GMT 2020**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: master)**
* **BUILD_LOG_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/714236916**
* **BUILD_OS = (osx) Darwin lgb 18.7.0 Darwin Kernel Version 18.7.0: Thu Jan 23 06:52:12 PST 2020; root:xnu-4903.278.25~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME = 16:16  up 5 mins, 2 users, load averages: 2.39 3.82 2.16**
* TRAVIS_APP_HOST = build.travis-ci.org
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = master
* TRAVIS_BUILD_DIR = /Users/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 714236913
* TRAVIS_BUILD_NUMBER = 744
* TRAVIS_BUILD_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/builds/714236913
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy MacOS
* TRAVIS_COMMIT = 0d43fb97c26349a7cc820356f9113db86a95fc7d
* TRAVIS_COMMIT_MESSAGE = Merge pull request #131 from lgblgblgb/dev
* TRAVIS_COMMIT_RANGE = 31855a4799c2...0d43fb97c263
* TRAVIS_COMPILER = gcc
* TRAVIS_CPU_ARCH = amd64
* TRAVIS_DIST = notset
* TRAVIS_ENABLE_INFRA_DETECTION = true
* TRAVIS_EVENT_TYPE = push
* TRAVIS_FILTERED = redirect_io
* TRAVIS_HOME = /Users/travis
* TRAVIS_INFRA = macstadium
* TRAVIS_INIT = notset
* TRAVIS_INTERNAL_RUBY_REGEX = ^ruby-(2\.[0-4]\.[0-9]|1\.9\.3)
* TRAVIS_JOB_ID = 714236916
* TRAVIS_JOB_NAME = MacOS native compilation
* TRAVIS_JOB_NUMBER = 744.3
* TRAVIS_JOB_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/714236916
* TRAVIS_LANGUAGE = c
* TRAVIS_OSX_IMAGE = xcode11
* TRAVIS_OS_NAME = osx
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 193ee8cb
* TRAVIS_TIMER_START_TIME = 1596384965576212000
* TRAVIS_TMPDIR = /var/folders/17/5mc7816d3mndxjqgplq6057w0000gn/T/tmp.1ukRJWAl

## Commit log (last 25)

commit 0d43fb97c26349a7cc820356f9113db86a95fc7d
Merge: 31855a4 7d3824e
Author: LGB <lgblgblgb@gmail.com>
Date:   Sun Aug 2 18:10:43 2020 +0200

    Merge pull request #131 from lgblgblgb/dev
    
    Merge dev changes into master.

commit 7d3824e8357be7efd2c0bbe2c1f9f56f9c6ab3af
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Aug 1 15:19:11 2020 +0200

    HID: OSD key name debug + C65/MEGA65 UI opt

commit e7b065d41d6e14c99dcccabf4dde5a7dbd4949f8
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 23 16:02:17 2020 +0200

    DOC: add AUTHORS file

commit dc457f0cf7a77f293884bd8ff01d1126443d44d1
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 23 13:33:03 2020 +0200

    MEGA65: implement untested audio DMA + OPL3 #127

commit 6c79db0831b8e787504d75e39e0590ff105c3da3
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 23 13:26:50 2020 +0200

    OPL3: importing Nuked-OPL3 into Xemu

commit 95c816880472ae3b85533a1c90769dd4dc6c93fd
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 13:00:03 2020 +0200

    MEGA65: MEGA65-compliant palette handling finally

commit 3b1790316aa17ae9b7fdb2d5a9d148d9f8aae0e0
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 09:21:36 2020 +0200

    MEGA65: allow PRG inject from the GUI too

commit d31ad0655251d83575ee1bda9c32943c063112d8
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 09:01:23 2020 +0200

    MEGA65: enable 8Mbyte of slow-RAM by default

commit d2b12266d3f84baab0ad3e409c2db1727b4476c3
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 08:53:52 2020 +0200

    MEGA65: PRG injecting directly into the memory

commit 065d4cf28936ae2c3c105d4bc6327e8e558c185a
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 08:45:43 2020 +0200

    MEGA65: DMA: skip one byte if bad enh.opt >=0

commit 5e4de89243a6d2b14b744dce41a697e7705d7d8d
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 08:42:14 2020 +0200

    MEGA65: more clear message on ext.D81 mount problem

commit c25933890080b8bcd3b21857f7b6c747bf4390a8
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu Jul 16 08:39:25 2020 +0200

    CORE+CIA6526: trying to make sub-second precision for TOD #129

commit c746e6ffec2b9d367091f63ac9713acdbe0e947d
Merge: 4c13655 ea4b60e
Author: LGB <lgblgblgb@gmail.com>
Date:   Sun Jul 5 22:28:29 2020 +0200

    Merge pull request #128 from hernandp/input-dev-update
    
    Updated ASCII keycodes + priorities + ALT support.

commit ea4b60ee453dcfdca5ad790013df7800f5b05815
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Sun Jul 5 16:33:28 2020 -0300

    Updated ASCII and priorities according to latest VHDL source, plus ALT key support.

commit 31855a4799c261eb9244ffe14dee600aac0bc760
Merge: 527c2b0 4c13655
Author: LGB <lgblgblgb@gmail.com>
Date:   Sat Jun 20 21:54:54 2020 +0200

    Merge pull request #123 from lgblgblgb/dev
    
    Merge dev back, especially because of windows large file problems.

commit 4c13655840303faf4920b21b9e01e4592847b451
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jun 20 16:23:06 2020 +0200

    Windows: large file support request for Mingw

commit ad4c29c3667715a4cf7742799e7dce2c01c1f1ce
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jun 17 20:20:16 2020 +0200

    C65+M65: add disk change signal #118

commit aea8cd2bd63353a61f811d1f0ce947fce5967104
Author: LGB <lgblgblgb@gmail.com>
Date:   Mon Jun 15 21:21:57 2020 +0200

    BUILD: work-around old/missing GIT failing build

commit 16acaa9ce35cdec1cd0b3ffcb3081cc832f3d3f2
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jun 10 00:19:34 2020 +0200

    BUILD: try to avoid absolute paths in configure

commit 68a1d233cd4ae1cdb01a7880b38ec484a896da60
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jun 9 21:17:11 2020 +0200

    M65: 8K WOM, correct 2nd offset, ability to re-WOM

commit 527c2b021966f6f9f2444c23d6402c141d1c19d2
Merge: 69b0c90 702b839
Author: LGB <lgblgblgb@gmail.com>
Date:   Tue Jun 9 13:33:47 2020 +0200

    Merge pull request #116 from lgblgblgb/dev
    
    Merge dev stage into master

commit 702b83942400d92bf12f9e7b24ffb4b04ab8637f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jun 9 13:18:18 2020 +0200

    MEGA65: add help UI entry (online)

commit 8e298c8061b56b3233628ad7b73b08a11de22858
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Jun 5 15:05:16 2020 +0200

    M65: SD fdisk/update upgrades

commit 468852a8f212a65ece8c721ff528a0e2ea3524b9
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Jun 5 14:49:08 2020 +0200

    BUILD: build system tweaks, RELEASE=yes mode

commit a8408ca6e5662d7726d0d5406509e5168e74db3d
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Fri Jun 5 14:03:46 2020 +0200

    M65: MEGA65 as the official name
