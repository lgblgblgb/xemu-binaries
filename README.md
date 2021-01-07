# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20210107201413**) for **MacOS**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **vic branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **vic**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-vic
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-vic
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-vic

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/d9a19fe27a607d9d423c1a1d17b2cf85048a3f30**
* **BUILD_DATE = Thu Jan  7 19:21:37 GMT 2021**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: vic)**
* **BUILD_LOG_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/753410758**
* **BUILD_OS = (osx) Darwin lgb 18.7.0 Darwin Kernel Version 18.7.0: Thu Jan 23 06:52:12 PST 2020; root:xnu-4903.278.25~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME = 19:21  up 6 mins, 2 users, load averages: 2.67 4.03 2.32**
* TRAVIS_APP_HOST = build.travis-ci.org
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = vic
* TRAVIS_BUILD_DIR = /Users/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 753410755
* TRAVIS_BUILD_NUMBER = 927
* TRAVIS_BUILD_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/builds/753410755
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy MacOS
* TRAVIS_COMMIT = d9a19fe27a607d9d423c1a1d17b2cf85048a3f30
* TRAVIS_COMMIT_MESSAGE = M65+C65: better ROM ver + DMA rev setting + UI query
* TRAVIS_COMMIT_RANGE = e1f427674762...d9a19fe27a60
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
* TRAVIS_JOB_ID = 753410758
* TRAVIS_JOB_NAME = MacOS native compilation
* TRAVIS_JOB_NUMBER = 927.3
* TRAVIS_JOB_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/753410758
* TRAVIS_LANGUAGE = c
* TRAVIS_OSX_IMAGE = xcode11
* TRAVIS_OS_NAME = osx
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 10296ff6
* TRAVIS_TIMER_START_TIME = 1610047297486974000
* TRAVIS_TMPDIR = /var/folders/17/5mc7816d3mndxjqgplq6057w0000gn/T/tmp.KFWQO6hR

## Commit log (last 25)

commit d9a19fe27a607d9d423c1a1d17b2cf85048a3f30
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jan 7 20:14:13 2021 +0100

    M65+C65: better ROM ver + DMA rev setting + UI query

commit 30a047c79056ea1402f1561cd033683a981a1a50
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jan 7 20:12:48 2021 +0100

    UI: adding SDL scale render quality and CLI opt

commit 31369af5bb7844ffbbc9458d7dc48075d361c684
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jan 5 12:55:24 2021 +0100

    CORE: SDL hint change, M65: option for quality

commit e5c1fe94cb2c5ae2ed29c21f96c9c3d2ae73185a
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 3 14:29:53 2021 +0100

    Fix tab/space source line endings

commit e1f4276747622d39ab00d36f8288b451d15e9305
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 17:25:36 2021 +0100

    BUILD: Fix querying current git branch

commit 16ab75ac1df411ddd5248dabb2d2c611fa0fdc94
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 17:15:50 2021 +0100

    BUILD: Fix querying current git branch

commit bf1f5dfa98a087c702ee586eb0ecf636c4bd993f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 17:10:25 2021 +0100

    BUILD: Fix querying current git branch

commit be3691000463c7b7ac9714bdb37f8fc2c3db15b9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 16:59:10 2021 +0100

    BUILD: Fix querying current git branch

commit 288ef44aa9f9dd0f61a5ea2de96e6e5d7639997a
Author: LGB <lgblgblgb@gmail.com>
Date:   Sat Jan 2 11:55:32 2021 +0100

    Grrr, git shows HEAD instead of real branch 2

commit 8737e7f89428afed003d9de901d112c518936f94
Author: LGB <lgblgblgb@gmail.com>
Date:   Sat Jan 2 11:45:16 2021 +0100

    Grrr, git shows HEAD instead of real branch

commit 066cd2299fb646431376116126e4e42ace4a10e0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 09:49:21 2021 +0100

    WINDOWS: Trying to fix web-browser call #217

commit c47b7f53a134caae080a4216f9b23cc11bc700ca
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 00:16:01 2021 +0100

    BUILD: Fix querying current git branch

commit b766d2cf14478806c6ef65226401628c1bb7df5f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 23:12:31 2021 +0100

    WINDOWS: Trying to fix web-browser call #217

commit 1612671ed098e8ca38c8defe35beab133d7b513a
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 19:37:11 2021 +0100

    WINDOWS: Trying to fix web-browser call #217

commit 6d9807e976cc1491157773d38c7744d343febc52
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 18:01:05 2021 +0100

    stuff

commit b090fa47d50d850ed776561661993514a2ae06a0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 15:55:08 2021 +0100

    GUI: some mods, parent name pass-through

commit 2932ed17b50b7022334a908490ab146e2231c8db
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 15:43:54 2021 +0100

    GUI: some mods, parent name pass-through

commit ccada0a7d8226981eff1954670f9142f180e8e22
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 14:49:03 2021 +0100

    misc minor mods

commit 566da52c22fed0d4f430015fdf8bccb85cd1e2a8
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 14:41:30 2021 +0100

    GUI: some mods, parent name pass-through

commit 232cb0723c9c028bcd88d4d297c6249a7f655e6f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 14:32:42 2021 +0100

    GUI: some mods, parent name pass-through

commit ae3f38581e43536164c6282e93623ddf20b56a74
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Dec 28 01:24:39 2020 +0100

    CLCD: rom patch on/off

commit 8b7800f9cecba2b7c72a4e84efb6c47514f64793
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Dec 28 01:22:04 2020 +0100

    M65+C65 unif. drv led + UI + misc

commit 904ec97e8484cf1b7c6378f73e39df79199e5917
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Dec 26 18:56:45 2020 +0100

    C65: render drive LED optionally

commit 894aa620fb3a217b4347eb1fe6d33620d9207bb0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Dec 26 18:55:51 2020 +0100

    C65: C65 inject fixes #210

commit 4619bd92c5319f23b56c382563bd1e77e77594c4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Dec 25 00:43:21 2020 +0100

    Trying alternate web browser exec
