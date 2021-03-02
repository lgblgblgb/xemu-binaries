# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20210302012957**) for **MacOS**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **hmw branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **hmw**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-hmw
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-hmw
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-hmw

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/3f5c1816f94341e1e0ba9395c64feab67abcce12**
* **BUILD_DATE = Tue Mar  2 00:36:58 GMT 2021**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: hmw)**
* **BUILD_LOG_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/761044489**
* **BUILD_OS = (osx) Darwin lgb 18.7.0 Darwin Kernel Version 18.7.0: Thu Jan 23 06:52:12 PST 2020; root:xnu-4903.278.25~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME =  0:36  up 5 mins, 2 users, load averages: 2.51 3.75 2.09**
* TRAVIS_APP_HOST = build.travis-ci.org
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = hmw
* TRAVIS_BUILD_DIR = /Users/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 761044486
* TRAVIS_BUILD_NUMBER = 987
* TRAVIS_BUILD_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/builds/761044486
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy MacOS
* TRAVIS_COMMIT = 3f5c1816f94341e1e0ba9395c64feab67abcce12
* TRAVIS_COMMIT_MESSAGE = MEGA65: quick'n'dirty fix for double speed CPU bug
* TRAVIS_COMMIT_RANGE = 27688a402b83...3f5c1816f943
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
* TRAVIS_JOB_ID = 761044489
* TRAVIS_JOB_NAME = MacOS native compilation
* TRAVIS_JOB_NUMBER = 987.3
* TRAVIS_JOB_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/761044489
* TRAVIS_LANGUAGE = c
* TRAVIS_OSX_IMAGE = xcode11
* TRAVIS_OS_NAME = osx
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 1103e100
* TRAVIS_TIMER_START_TIME = 1614645418437756000
* TRAVIS_TMPDIR = /var/folders/17/5mc7816d3mndxjqgplq6057w0000gn/T/tmp.Jgd5sPii

## Commit log (last 25)

commit 3f5c1816f94341e1e0ba9395c64feab67abcce12
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Mar 2 01:29:57 2021 +0100

    MEGA65: quick'n'dirty fix for double speed CPU bug

commit 27688a402b837d641d120a1c9e2ccb9e58097807
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Feb 11 01:33:10 2021 +0100

    M65: Trying to fix memptr with inject here, too

commit b753cc04abd683f789ded5082ae721e776f20d85
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Feb 11 01:16:44 2021 +0100

    Build related material

commit 5d1d8e94c831ad4e1703ea47f3b83462dc0838c4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Feb 10 14:14:22 2021 +0100

    MEGA65: bitplane bank selection

commit c8a1bca1d22582bbd4fada0434d43a2b3d21b546
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Feb 10 13:29:07 2021 +0100

    MEGA65: 32x32bit div/mult unit support backported

commit afc557c3bf24f688aecd15458430056cbdfc2cc6
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 29 23:38:19 2021 +0100

    MEGA65: D613/D614 kbd matrix scan support #228

commit 4c78b8a80386a8c37ef1fb9cf1e6e4f02b097965
Merge: 7b1b27c 1231229
Author: LGB <lgblgblgb@gmail.com>
Date:   Tue Nov 3 15:29:03 2020 +0100

    Merge pull request #207 from hernandp/megawat
    
    Added H320  BPM mode for C65 Snoopy image demo.

commit 7b1b27ca5a7c2b91d30295ff9497943568f88e72
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Tue Nov 3 10:38:07 2020 +0100

    Adding version info on deploy

commit 1231229af4847f0810ee415c6f152676e8b35f8c
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Tue Nov 3 02:32:16 2020 -0300

    Added H320  BPM mode for C65 Snoopy image demo.

commit 0509f756c4b39bd3089e5ea0d89a158acc28d365
Merge: 61d87a5 04f6c67
Author: LGB <lgblgblgb@gmail.com>
Date:   Mon Sep 21 17:58:24 2020 +0200

    Merge pull request #170 from hernandp/megawat
    
    Incorporates PR to fix Catalina Compilation

commit 04f6c673e1674246e4a1f85741e111627c4ac466
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Mon Sep 21 12:36:00 2020 -0300

    Incorporates PR to fix Catalina Compilation (#146)

commit 61d87a50dce2a6718c8a9273fa6a0db3c914ca9d
Merge: 46ef860 7806a61
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Sep 9 21:55:03 2020 +0200

    Merge pull request #141 from hernandp/megawat
    
    Removed warning when writing to $D031 .

commit 7806a61aecd18ce176bb7d7363d49844137f3ea1
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Wed Aug 26 17:04:11 2020 -0300

    Removed warning when writing to $D031 .

commit 46ef860baf4f8552ca9e203ca401c830d59b9cdb
Merge: 5d4cde6 58531eb
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Aug 26 08:40:52 2020 +0200

    Merge pull request #138 from hernandp/megawat
    
    Megawat

commit 5d4cde6162b69b5aeafdbbc74b1cb950ee0edbc7
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Aug 26 08:31:59 2020 +0200

    BUILD: use ubuntu version 20.04 on travis

commit 58531ebcfd5355cf70316e7cc8979b11fb74025d
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Wed Aug 26 01:06:50 2020 -0300

    Disable DMA debug output messages.

commit b437d6cf11a99ee322dd0b7f0a42773ca9123508
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Wed Aug 26 00:08:17 2020 -0300

    Full frame rendering with enhanced timings.

commit b51c914dbd6c21f0941e49b52ea295e07bec3af6
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Tue Aug 25 12:23:44 2020 -0300

    Basic Perf stats collection.

commit 9ff9a110f25421c92a7032e1ebbfaf0fdf5face0
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Mon Aug 24 12:23:42 2020 -0300

    impl: Color RAM offset (COLPTR)

commit 630ab570163e2e5cbf618fa03f15cbea729f66ee
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Sun Aug 23 19:15:12 2020 -0300

    FIX:  0x51 XPOS will return bogus data for MEGAWAT intro to work.  FIX: DD00 bits considered for character addr FIX: $D018 register write

commit 996c1234c47105ff4745f9ec6e4bbd6e396e645d
Merge: 765ab9c 350b294
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Aug 19 11:41:02 2020 +0200

    Merge pull request #137 from hernandp/megawat
    
    Update 200818

commit 350b294cad9340f6d782f0271e3dbde9e24f3f08
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Wed Aug 19 01:21:20 2020 -0300

    D018 returns bit #0 as 1.   MULTICOLOR register has priority (game SUPERNATURAL renders sprites OK)

commit 27878942586acca0facf2113375e5fe83bca7fb4
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Tue Aug 18 02:18:59 2020 -0300

    16-color sprite implies 16-pixel wide enable (SPRX64EN)

commit f37dfd7bdbb06faf842a74321575f428a33db9c8
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Mon Aug 17 23:38:07 2020 -0300

    FIX: Honours VIC-II banking

commit f7b77dd7a804a95235e30dac99db7c4a1fd918b9
Author: Hernán Di Pietro <hernan.di.pietro@gmail.com>
Date:   Mon Aug 17 15:50:41 2020 -0300

    emutools viewport service + mega65 borders + const correctness.
