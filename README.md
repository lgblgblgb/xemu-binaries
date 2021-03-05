# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20210305200506**) for **Windows**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/6a67b7f33776fbbd19e64542de72dc346ea0bcb9**
* **BUILD_DATE = Fri 05 Mar 2021 07:21:10 PM UTC**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: dev)**
* **BUILD_LOG_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/761622429**
* **BUILD_OS = (linux) Linux lgb 5.4.0-1037-gcp #40-Ubuntu SMP Fri Feb 5 11:57:53 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Windows**
* **BUILD_UPTIME =  19:21:10 up 4 min,  1 user,  load average: 1.62, 1.29, 0.59**
* TRAVIS_APP_HOST = build.travis-ci.org
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = dev
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 761622427
* TRAVIS_BUILD_NUMBER = 991
* TRAVIS_BUILD_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/builds/761622427
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Windows
* TRAVIS_COMMIT = 6a67b7f33776fbbd19e64542de72dc346ea0bcb9
* TRAVIS_COMMIT_MESSAGE = Next minor backporting
* TRAVIS_COMMIT_RANGE = 58a4cc8a291f...6a67b7f33776
* TRAVIS_COMPILER = gcc
* TRAVIS_CPU_ARCH = amd64
* TRAVIS_DIST = focal
* TRAVIS_ENABLE_INFRA_DETECTION = true
* TRAVIS_EVENT_TYPE = push
* TRAVIS_FILTERED = redirect_io
* TRAVIS_HOME = /home/travis
* TRAVIS_INFRA = unknown
* TRAVIS_INIT = systemd
* TRAVIS_INTERNAL_RUBY_REGEX = ^ruby-(2\.[0-4]\.[0-9]|1\.9\.3)
* TRAVIS_JOB_ID = 761622429
* TRAVIS_JOB_NAME = Windows cross-compilation on Linux
* TRAVIS_JOB_NUMBER = 991.2
* TRAVIS_JOB_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/761622429
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2021-03-02T09:46:09
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = generic basic ruby_interpreter
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2004__ c c++ cplusplus cpp ruby python go java php node_js smalltalk csharp perl rust erlang
* TRAVIS_STACK_NAME = ubuntu_2004
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2021-03-02 09:46:18 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 0c384378
* TRAVIS_TIMER_START_TIME = 1614972070678800896
* TRAVIS_TMPDIR = /tmp/tmp.plJg6JCVp5
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 6a67b7f33776fbbd19e64542de72dc346ea0bcb9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Mar 5 20:05:06 2021 +0100

    Next minor backporting

commit 58a4cc8a291fef48307e6845ec764e6f039b30a9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Mar 5 19:51:40 2021 +0100

    Next minor backporting

commit 36e75581bcd227b52681d2ef5f7e6b0943f4470e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Mar 5 12:27:20 2021 +0100

    Fix some trailing white spaces and such

commit bf541b73c5b2ec220ea2d465968866bac0219016
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Mar 5 11:02:34 2021 +0100

    Push inject fixes into DEV too

commit c199ef0d715fb8db7616c1dee383d4ba7abac514
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Feb 8 15:36:46 2021 +0100

    ConfigDB more fixes and tweaks

commit 5673869109ae0b0ad1503f314289e26e1d82de55
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Feb 8 10:15:00 2021 +0100

    ConfigDB fixes and tweaks

commit 574f74fbfd685ef73b5bdc5abd496553a01391d0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Feb 5 01:23:40 2021 +0100

    Try to re-work ConfigDB

commit 98c58f836e621667627757ebb3c5e7310aeb0e57
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 23 16:20:45 2021 +0100

    CORE: seed random number generator

commit e8a04843bfb02fab363eb8ff330e9eeac6202c69
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 23 16:19:35 2021 +0100

    CORE: add CFG multidef + dereference check

commit 00d62973486a984dbb95f08009e359e2476db682
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Jan 20 14:12:34 2021 +0100

    ...

commit c0c57fec7d9c2c5828772e03aecb5a3e60e5ea08
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jan 19 14:05:35 2021 +0100

    M65: trying to implement DAT #126

commit 8c1b59ebf1f0e3305a65d8e04f51113b9e45d79e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jan 19 00:23:12 2021 +0100

    Another round of 'alignment' fixing

commit a1fa15b9b218ec09714e17403fa0b865b039f825
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 18 00:38:13 2021 +0100

    CBM screen to paste buffer rvs feature

commit 2383bed95da3d57c344f3cc992c65dc26eff0f9d
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 23:13:24 2021 +0100

    C65: this emu has screen to OS paste buf too

commit aa3bc7396bb495a60da99d067dcd32a4d04d659c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 16 21:02:17 2021 +0100

    M65: auto-detect paste capture

commit 19f4cf764338036e1679cbc95d3b5791b2a3e4e0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 16 02:15:50 2021 +0100

    M65: UI to put screen content to OS paste buffer

commit 0ccb1ef9249e00af0c131ed4fd38ef77f9536306
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 15 23:43:29 2021 +0100

    MEGA65: bitplane bank selection fix

commit 1da0f39627f6e2b4d8f334ac5763827f46e10b31
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 15 23:42:54 2021 +0100

    Some drive#1 stuff

commit 462fd7acfadf61952836cfb6fd63ca166e02a2d9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 15 20:46:10 2021 +0100

    MEGA65: bitplane bank sel, VIC4 reset

commit dd84545506d8608205d33c5a7770d38ad9cd1d31
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jan 14 22:18:20 2021 +0100

    gcc warning fix, better

commit ca3c2943b2c9ff5b8720ad464877afc89464c27c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jan 14 19:17:41 2021 +0100

    CORE: avoid a stupid gcc warning

commit 8534b506ddd5e76ef4ccdd8933261f24f13bce4b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jan 14 01:24:04 2021 +0100

    M65: do not use ethertap on ARM linux

commit 99481c4bacb0657427614c1ae39ca46fb2b4de9c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jan 13 15:45:54 2021 +0100

    M65: some clean-up for D610 stuff #225

commit e564c647a289b4d6f2c86de74c55845cee734db6
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jan 13 01:06:11 2021 +0100

    M65: 2nd try to fix D610-stuff on C65 keys #225

commit f2402d7b8ee0b1c12c1c697e98efbb7e85b37dc8
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jan 13 00:12:47 2021 +0100

    M65: trying to fix D610-stuff on extra C65 keys
