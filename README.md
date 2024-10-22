# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20241022151724**) for **Windows**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/5e4178d860c4d7bc08dd5beeb3ab1fb74566da02**
* **BUILD_DATE = Tue Oct 22 01:37:58 PM UTC 2024**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: dev)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/627364814**
* **BUILD_OS = (linux) Linux lgb 6.8.0-1014-gcp #16~22.04.1-Ubuntu SMP Mon Aug 26 16:53:29 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Windows**
* **BUILD_UPTIME =  13:37:58 up 5 min,  1 user,  load average: 1.55, 1.06, 0.47**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = dev
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 272837488
* TRAVIS_BUILD_NUMBER = 1424
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/272837488
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Windows
* TRAVIS_COMMIT = 5e4178d860c4d7bc08dd5beeb3ab1fb74566da02
* TRAVIS_COMMIT_MESSAGE = MEGA65+C65: making "F10 to reset" remappable
* TRAVIS_COMMIT_RANGE = 57485669b05e...5e4178d860c4
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
* TRAVIS_JOB_ID = 627364814
* TRAVIS_JOB_NAME = Windows cross-compilation on Linux
* TRAVIS_JOB_NUMBER = 1424.2
* TRAVIS_JOB_RESTARTED = false
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/627364814
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2024-09-13T13:00:20
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_PRIVATE = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = basic disabled-ipv6 docker docker-compose elasticsearch firefox go-toolchain google-chrome jdk memcached mongodb mysql nodejs_interpreter perl_interpreter perlbrew phantomjs postgresql python_interpreter redis ruby_interpreter sqlite xserver
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2204__ c c++ cplusplus cpp ruby python go java php generic node_js smalltalk shell csharp perl rust elixir erlang
* TRAVIS_STACK_NAME = ubuntu_2204
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2024-09-13 13:00:30 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 1e1c9a32
* TRAVIS_TIMER_START_TIME = 1729604278899853708
* TRAVIS_TMPDIR = /tmp/tmp.XJG3ssQein
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 5e4178d860c4d7bc08dd5beeb3ab1fb74566da02
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Tue Oct 22 14:29:16 2024 +0200

    MEGA65+C65: making "F10 to reset" remappable
    
    STATUS: patch has been introduced in dev

commit 57485669b05e072c82245ee0e1931a275df14680
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Tue Oct 22 11:51:43 2024 +0200

    MEGA65: hwerrata register initial support
    
    sync with next:
    
            dae4fa20ba3e79ac1f5c1fc7705c930f867e657c
    
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Fri Sep 20 23:19:17 2024 +0200
    
        MEGA65: hwerrata register initial support #414
    
        * Basic HWERRATA and VIC BUGCOMPAT bit support
        * Rudimentary X scroll register offset fix support from level 1 and up
        * But NO support yet for char attribute fix at level 2

commit ef9be42a0a12de8cb37642e231f809edd5da17d4
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Thu Sep 26 14:51:55 2024 -0700

    Fixing CHRCOUNT for being 10 bits
    
    Issue has been found and fixed by @RetroCogs
    
    Sync with next from a00858f01054931e69840e15d8d73c2deed69057

commit 7d5dc0f592b3f9f490a5cada920450e14c248380
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Tue Oct 22 11:34:20 2024 +0200

    MEGA65: next merge: disable mouse + joy port swap
    
    73949895d9051c63c1a90cb5b13416fb45474201
    
        MEGA65: adding option to disable mouse emulation
    
        The problem: Xemu user may leave mouse grab mode to do something with
        their mouse. To avoid bothering the mouse-aware MEGA65 program running,
        I returned zero for relative mouse position change in this case. However
        that can cause problems with certain programs which are not mouse based
        and expecting $FF if mouse is not there.
    
    a2c06b75c0ec79ad429d7c4881beaba2ad2c11a9
    
        MEGA65: fix joy port swap with mouse grab
    
        Also adding an config option '-joyport N' (N can be 1 or 2) as a CLI
        option to select the default emulated port. Also, now the configuration
        can be saved which preserves the "swap state" of ports.
    
        The original problem was discovered by @Gurcei when he noticed that
        using the UI menu's "swap port" functionalty does nothing. It was
        because for some reason I wrote code to force port-1 when in mouse grab
        mode. Which is bad ...

commit f6d98d19435087dee8f44585ae024ba4ad024591
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Oct 21 23:06:47 2024 +0200

    MEGA65: HDOS virtualization: loadfile_attic
    
    Sync with next.

commit 7c045736d47a2e480577a95369ae8654648a7de8
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Oct 22 01:28:31 2024 +0200

    BUILD: Travis advice to add dpl_version
    
    Recently MacOS builds didn't worked anymore. Travis support suggested to
    add this line:
    
       dpl_version: 1.10.16
    
    into .travis.yml at the deploy section. Since it's OSX related problem,
    I've added only there.

commit 6568d4ad0d021cbee857a4a5b2f170f4a1c2337e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Sep 20 00:14:46 2024 +0200

    C65: DMA rev detection fix for ROMs #413

commit bc3bf5eb49a42da5e4ddac5bc3c9c9acbbee43e0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 19 22:11:23 2024 +0200

    uartmon write 0x777....

commit 4af2d8580c874e6dcd3f3aee4b4676e7af48b932
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 19 22:10:18 2024 +0200

    MEGA65: HWERRATA $D08F register-only support again

commit 234cc14a531a8749e41cdf814f49b0ebcd879353
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Tue Aug 20 22:24:26 2024 -0700

    Update vic4.c

commit 22baa70360277b28b926aef5719682680f16424b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Sep 15 13:06:18 2024 +0200

    MEGA65: allow pre-init Attic RAM content
    
    Allow Attic RAM to be pre-inited from the content of a file, given by
    the CLI option "-initattic FILENAME".
    
    Idea from @ki-bo on Discord
    
    Also can be part of #238 ... though that issue has bigger scope.

commit 92d035784a74697558897b52a93ebdb7e8f2b4f2
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Fri Sep 13 23:56:37 2024 -0700

    Update vic4.c

commit cae470725ab8ae0d69cc7da169211dc156993d4c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Sep 9 20:37:15 2024 +0200

    HWERRATA ($D08F) register-only support
    
    Also, according to: https://github.com/MEGA65/mega65-core/issues/829
    
    Please note, that this implementation does not implement any erratas at
    all, just the register for it ...

commit 3810fed50f933b669d3804f670bc714f5106bc7f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Aug 9 18:31:53 2024 +0200

    MEGA65: first try line drawing DMA WIP!!!! #404

commit 7cf1df14c5258afdd8e91a15c30211d4e589e26f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Aug 9 18:30:46 2024 +0200

    MEGA65: sync with next + adding mem map developments [WIP!!!!]

commit 6e9d2ce289e5edc7907b8269fb15918fd5d8f5bb
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jun 17 20:25:39 2024 +0200

    Revert "BUILD: try if ubuntu 24.04 works on Travis"
    
    This reverts commit 6e458b4e80ae32c68057c36289b42c4b50f17103.
    
    No, travis does not support Ubuntu 24.04 yet ...
    
    Result was: https://api.travis-ci.com/v3/job/623026323/log.txt

commit 6e458b4e80ae32c68057c36289b42c4b50f17103
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jun 17 20:22:34 2024 +0200

    BUILD: try if ubuntu 24.04 works on Travis
    
    Noble Ubuntu 24.04 LTS (Noble Numbat)

commit a7787a9456d337e99e274da4a6ed0439be26b8db
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jun 17 20:18:34 2024 +0200

    Various works:
    
    * Removing snapshot code from MEGA65 (not worked since years, unlikely
      it will ever will in this form at least)
    * Using a callback to have dynamic windows title other than the speed
      statistics
    * Continuing to reorganize uart_monitor
    * Continuing to mangle CPU65 emulator for breakpoint/etc callbacks

commit fab694e13c8350a01426c80d3cb82fd1d6b12aa2
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jun 13 01:09:30 2024 +0200

    MEGA65: reorg. uartmon #11
    
    Preliminary initial work, reorganization of uartmon, moving things out
    from mega65.c to uart_monitor.c
    
    No functionality change yet! And not even tested yet ;)

commit 82701d0745b0717788a84642df6584c2dd91b4fb
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jun 12 14:12:25 2024 +0200

    MEGA65: fix alt.palette selection #402
    
    Reported/suggested by Mirage_BD on Discord. Thanks!!

commit 7c2636359d87bdb1fa465b4f10eae1eb66bb665c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jun 12 14:06:37 2024 +0200

    MEGA65: DMA debug fix/optimization #198
    
    Small fix for more sane debug output when DO_DEBUG_DMA is defined for
    some extra DMA information. Nothing here which should affect an average
    user, only in a very unlikely scenario:
    
    One limitation of DMA emulation in Xemu: enhanced mode option list is
    read in a blockling fashion, thus an "unended" list will stall the
    emulator (though it's unlikely not to meet a zero byte sooner or later
    in the memory). To avoid this (and also warn the user about something
    fishy is going on) there is a warning window in that case - as the
    number of enhanced mode options are limited, it's simply insane to have
    a very large option list, thus it's a certain sign of some bug in the
    software which produces this: better the user to know.

commit 5dfb9f72219ccb908d7380d6aabe412e538400c7
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Mon May 27 03:23:52 2024 -0700

    Add support for RRB feature 796

commit 40e4dc58d0b4e6521aed6c76208e8bf150435f08
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Thu May 16 12:44:13 2024 +0200

    Sync with next

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
