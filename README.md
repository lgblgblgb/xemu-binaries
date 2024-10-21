# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20241022012831**) for **MacOS**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **next branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **next**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-next
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-next
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-next

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/b4d8b8a2b289bddbeab789f1711b71858aedba4b**
* **BUILD_DATE = Mon Oct 21 23:34:30 GMT 2024**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: next)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/627337929**
* **BUILD_OS = (osx) Darwin lgb 18.7.0 Darwin Kernel Version 18.7.0: Thu Jan 23 06:52:12 PST 2020; root:xnu-4903.278.25~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME = 23:34  up 3 mins, 2 users, load averages: 5.96 5.33 2.43**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = next
* TRAVIS_BUILD_DIR = /Users/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 272826907
* TRAVIS_BUILD_NUMBER = 1422
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/272826907
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy MacOS
* TRAVIS_COMMIT = b4d8b8a2b289bddbeab789f1711b71858aedba4b
* TRAVIS_COMMIT_MESSAGE = BUILD: Travis advice to add dpl_version
* TRAVIS_COMMIT_RANGE = 73949895d905...b4d8b8a2b289
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
* TRAVIS_JOB_ID = 627337929
* TRAVIS_JOB_NAME = MacOS native compilation
* TRAVIS_JOB_NUMBER = 1422.3
* TRAVIS_JOB_RESTARTED = false
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/627337929
* TRAVIS_LANGUAGE = c
* TRAVIS_OSX_IMAGE = xcode11
* TRAVIS_OS_NAME = osx
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_PRIVATE = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 02d0aea0
* TRAVIS_TIMER_START_TIME = 1729553670314238000
* TRAVIS_TMPDIR = /var/folders/17/5mc7816d3mndxjqgplq6057w0000gn/T/tmp.Sl95wvSD

## Commit log (last 25)

commit b4d8b8a2b289bddbeab789f1711b71858aedba4b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Oct 22 01:28:31 2024 +0200

    BUILD: Travis advice to add dpl_version
    
    Recently MacOS builds didn't worked anymore. Travis support suggested to
    add this line:
    
       dpl_version: 1.10.16
    
    into .travis.yml at the deploy section. Since it's OSX related problem,
    I've added only there.

commit 73949895d9051c63c1a90cb5b13416fb45474201
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Oct 21 23:12:18 2024 +0200

    MEGA65: adding option to disable mouse emulation
    
    The problem: Xemu user may leave mouse grab mode to do something with
    their mouse. To avoid bothering the mouse-aware MEGA65 program running,
    I returned zero for relative mouse position change in this case. However
    that can cause problems with certain programs which are not mouse based
    and expecting $FF if mouse is not there.

commit 9b89f57c0abd3befbe99b195ea53a72eb2a02a77
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Oct 21 23:06:47 2024 +0200

    MEGA65: HDOS virtualization: loadfile_attic #331

commit a00858f01054931e69840e15d8d73c2deed69057
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Thu Sep 26 14:51:55 2024 -0700

    Fixing CHRCOUNT for being 10 bits #416
    
    Issue #416 has been found and fixed by @RetroCogs

commit a2c06b75c0ec79ad429d7c4881beaba2ad2c11a9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Sep 25 00:18:11 2024 +0200

    MEGA65: fix joy port swap with mouse grab #415
    
    Also adding an config option '-joyport N' (N can be 1 or 2) as a CLI
    option to select the default emulated port. Also, now the configuration
    can be saved which preserves the "swap state" of ports.
    
    The original problem was discovered by @Gurcei when he noticed that
    using the UI menu's "swap port" functionalty does nothing. It was
    because for some reason I wrote code to force port-1 when in mouse grab
    mode. Which is bad ...

commit dae4fa20ba3e79ac1f5c1fc7705c930f867e657c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Sep 20 23:19:17 2024 +0200

    MEGA65: hwerrata register initial support #414
    
    * Basic HWERRATA and VIC BUGCOMPAT bit support
    * Rudimentary X scroll register offset fix support from level 1 and up
    * But NO support yet for char attribute fix at level 2

commit 812232223e5bde444a17e96a52adcbb172e11a50
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Sep 20 00:14:46 2024 +0200

    C65: DMA rev detection fix for ROMs #413

commit efcf16df74ed7fbd49ca7339e7a417fe7a6e0706
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Sep 15 13:06:18 2024 +0200

    MEGA65: allow pre-init Attic RAM content
    
    Allow Attic RAM to be pre-inited from the content of a file, given by
    the CLI option "-initattic FILENAME".
    
    Idea from @ki-bo on Discord
    
    Also can be part of #238 ... though that issue has bigger scope.

commit 7c88427e21b549fa05c27b602ee691e05eb3b9dc
Merge: 802cdbb 02584e7
Author: LGB <lgblgblgb@gmail.com>
Date:   Sun Sep 15 11:09:38 2024 +0200

    Merge pull request #412 from RetroCogs/Fix-for-issue-#353
    
    Fix for issue #353 RRB is drawing outside top border

commit 02584e7231dcef690a05e257fbb43fa2213422c6
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Fri Sep 13 23:56:37 2024 -0700

    Update vic4.c

commit 802cdbb1db65c37ee97cb193fdac9ce79d46aa53
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Sep 11 20:15:02 2024 +0200

    MEGA65: umon should cpu view writes #411
    
    Xemu's "umon" (uart mon) implementation forgot to include support for
    the $777xxxx signalled "cpu view" write. It's implemented on reads, just
    not on writes. Probably it was my mistake to forget to add the support
    for the 's' command as well.

commit 487f7d22452a36d7d32e941ecb7ac272e384c208
Merge: c33bf19 1e12961
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Aug 21 10:11:49 2024 +0200

    Merge pull request #409 from RetroCogs/fixforissue407
    
    MEGA65: Update vic4.c for fix for transparency issue

commit 1e1296154dd782e91c26d37295b5ecfb95eb204d
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Tue Aug 20 22:24:26 2024 -0700

    Update vic4.c

commit c33bf19cea4c0f33e5e926e0ebfd5763c0871277
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Aug 19 12:15:41 2024 +0200

    MEGA65: first try of line drawing DMA (WIP!!) #404
    
    Incomplete and possible buggy first try implementation of DMA line
    drawing. Ideas are based on a "draft implementation" by btoschi
    on Discord (@bjotos on github).
    
    The only reason I present this highly incomplete work in the next branch
    of Xemu (so not in dev) because I am on holiday, so it's a bit random
    when I have time to do more work. Thus it's better to release it in
    this unfinished form, I guess, if someone wants to play with it.

commit bd47ac995d3c9c80e6d20412eb6d9c90180e2237
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Aug 5 20:45:57 2024 +0200

    MEGA65: "read of unwritten memory" debug mode #405
    
    Rhialto had the feature request to have a mode, where Xemu/MEGA65 can warn you
    on reading memory which was not written before, can be useful to find ROM bugs.
    
    In this current form, it's quite minimal and simple:
    
    1. Only works on the first 126K of physical RAM
    2. Only works from command line, start emulation with paramter: -ramcheckread
    3. You need to watch the output of the emulator, so on UNIX-like/Linux/Mac systems,
       emulator should be started from terminal window, on Windows, Xemu
       console must be open (start also with parameter: -syscon)
    4. Check the output of the emulator, you can find lines like:
       MEM: DEBUG: main RAM at linear address $101A0 has been read without prior write; PC=$8613 [$20613]
       The PC value can be off by some bytes, because it may have been
       incremented already during opcode emulation. The [...] is the linear
       address for the mentioned CPU PC value.
    
    Well, that's it.

commit 74e13c89f3d9406cb857c56e0b41941ec54b7a0f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jun 20 20:10:19 2024 +0200

    MEGA65: cleanup and reorg uartmon stuff #11
    
    Moving everything out of mega65.c which is uartmon into uart_monitor.c, well,
    at least allmost everything ... Still, no new feature is used from CPU65
    emulation, just mainly reorganization of the source to look nicer for
    further hacking/developing.

commit fbd314f49a152fe5e53879ee9d573f9d090e38d6
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jun 18 10:39:05 2024 +0200

    MEGA65+CORE: reorg. window title dynamic update

commit 6558f7234d17195569585514034adce0fcde72eb
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jun 18 09:59:35 2024 +0200

    MEGA65: cleanup, remove snapshot related stuff
    
    Emulator snapshots for the MEGA65 emulators are disabled since years for
    now, and wouldn't even work for multiple reasons in this very form. So
    it's fine to remove the "considered as dead" code. Even if I want this
    to work some day, a serious total rewrite would be needed.

commit ab2290e79f2dbc19dbf815a26f057ab42ba1802c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Jun 12 14:12:25 2024 +0200

    MEGA65: fix alt.palette selection #402
    
    Reported/suggested by Mirage_BD on Discord. Thanks!!

commit ec2504defc208687b106fdc39e18e87b16396c4b
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

commit 7e3fd0d46a5ebda578ef9895c522e5691601ba5f
Merge: 45f9ebf 5951ac3
Author: LGB <lgblgblgb@gmail.com>
Date:   Mon May 27 20:29:31 2024 +0200

    Merge pull request #401 from RetroCogs/RRBFeatureForIssue400
    
    Add support for RRB reverse Y-row adjust #400 by @RetroCogs

commit 5951ac324a23145009233f45e7e94d113d408753
Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
Date:   Mon May 27 03:23:52 2024 -0700

    Add support for RRB feature 796

commit 45f9ebfed919bab759ee329cffebda1b4de15b01
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun May 12 23:08:51 2024 +0200

    MEGA65: new memory decoder #209 #378
    
    This quite big change rewrites the MEGA65 emulation memory decoder
    subsystem. Some of the reasons:
    
    * Create a new, not overcomplicated decoder which can be understood at
      all without major headache, and can be also faster as per #209
    * Taking account some new findings about how C65 worked (both Xemu and
      MEGA65 was wrong here) and adopted since then by MEGA65 as per #378
    * More about the future (not ready in this commit): allow functionality
      for debugger implementation "watchmem" which can monitor about every
      memory r/w events debugger want to check as per #11
    
    This commit is quite big as was mentioned, and may introduce some
    regressions. So it's important to have feedback in those cases. Also it
    changes the behaviour of memory decoding (#378). The new decoder seems
    to be already faster than the old one and more easy to understand and
    maintain. Also there is some room for future improvements still in every
    areas, including optimizations. The "memwatch" part currently is not
    usable though, but the basis are there to be able to implement that at
    all (wouldn't be possible with the older scheme).

commit b6db38ec7948d4c2076ebcc87c29eb31c11a8e08
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun May 12 22:39:55 2024 +0200

    CORE: simple debug hooks into CPU65 emu #11
    
    To allow easier debugger implementation with breakpoints, and such, a
    new (optional to be used) mechanism is introduced. It allows the CPU65
    emulation core to call target emulator defined functions on each op code
    executions (and in case of IRQ and NMI acceptance). The target emulator
    itself can decide what to do in the callbacks, it can simply return, or
    instructing the CPU emulation to be stopped (ie: breakpoint or step
    based opcode execution during debugging).
    
    NOTE: still, the target emulator's main loop must aware of this, the
    CPU65 core itself alone cannot stop the whole emulation in a sane way.

commit 089ad07bda055c027ce5a2bbe3280ddd99a25442
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat May 11 22:12:52 2024 +0200

    BUILD: do not test grep -o on non-Linux #396
    
    configure tests for working `grep` utility for building, however it
    seems some systems (it seems NetBSD in particular) have problems with
    the `-o` switch combined with others. As the `-o` is only used for real
    at Linux hosts, let's not test `-o` if the build system is not Linux.
    
    Reported by @Rhialto
