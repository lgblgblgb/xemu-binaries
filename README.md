# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20240807161529**) for **Linux**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu









## Binary versions for **master**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/7a9e860ff5ce61dad53de5b9ca18b7100dd2bb8a**
* **BUILD_DATE = Wed Aug  7 02:20:09 PM UTC 2024**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: master)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/624900906**
* **BUILD_OS = (linux) Linux lgb 6.5.0-1025-gcp #27~22.04.1-Ubuntu SMP Tue Jul 16 23:03:39 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Linux**
* **BUILD_UPTIME =  14:20:09 up 4 min,  1 user,  load average: 1.24, 0.58, 0.23**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = master
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 271784464
* TRAVIS_BUILD_NUMBER = 1404
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/271784464
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Linux
* TRAVIS_COMMIT = 7a9e860ff5ce61dad53de5b9ca18b7100dd2bb8a
* TRAVIS_COMMIT_MESSAGE = Merge pull request #406 from lgblgblgb/next
* TRAVIS_COMMIT_RANGE = 828804b7277b...7a9e860ff5ce
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
* TRAVIS_JOB_ID = 624900906
* TRAVIS_JOB_NAME = Linux native compilation
* TRAVIS_JOB_NUMBER = 1404.1
* TRAVIS_JOB_RESTARTED = false
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/624900906
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2024-08-01T11:56:22
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_PRIVATE = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = basic disabled-ipv6 docker docker-compose elasticsearch firefox go-toolchain google-chrome jdk memcached mongodb mysql nodejs_interpreter perl_interpreter perlbrew phantomjs postgresql python_interpreter redis ruby_interpreter sqlite xserver
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2204__ c c++ cplusplus cpp ruby python go java php generic node_js smalltalk shell csharp perl rust elixir erlang
* TRAVIS_STACK_NAME = ubuntu_2204
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2024-08-01 11:56:36 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 1704c753
* TRAVIS_TIMER_START_TIME = 1723040408950837428
* TRAVIS_TMPDIR = /tmp/tmp.K9LSPKJrYj
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 7a9e860ff5ce61dad53de5b9ca18b7100dd2bb8a
Merge: 828804b 74e13c8
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Aug 7 16:15:29 2024 +0200

    Merge pull request #406 from lgblgblgb/next
    
    Next

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

commit 828804b7277ba2858693eac0e00ecf0b1aad37a4
Merge: 968f7e0 089ad07
Author: LGB <lgblgblgb@gmail.com>
Date:   Sat May 11 22:35:52 2024 +0200

    Merge pull request #399 from lgblgblgb/next
    
    Next

commit 089ad07bda055c027ce5a2bbe3280ddd99a25442
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat May 11 22:12:52 2024 +0200

    BUILD: do not test grep -o on non-Linux #396
    
    configure tests for working `grep` utility for building, however it
    seems some systems (it seems NetBSD in particular) have problems with
    the `-o` switch combined with others. As the `-o` is only used for real
    at Linux hosts, let's not test `-o` if the build system is not Linux.
    
    Reported by @Rhialto

commit d96aaeb131299f274f277e81c613dd99a9004894
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Mar 24 23:25:40 2024 +0100

    BUILD: use newer ubuntu LTS on Travis CI
    
    Travis has problems in the past with Ubuntu 20.04. I've issued a bug
    report, and for a while no successfull builds could be done, so I used
    Ubuntu 18.04 for a long time. Now it seems my bug report was addressed
    by Travis, and it works now. It means that a newer mingw compiler is
    used to produce Windows builds, which hopefully means a bit better
    emulation performance on Windows. Or not ... ;)

commit 775c87f5e5410d3e9b4ecd2a4ea1ca5e146158ed
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Mar 24 23:22:43 2024 +0100

    MEGA65: fix RRB rowmask reset
    
    RRB rowmask was implemented in #363 by me. However it seems, there is
    one important fact I missed: to clear RRB when it's not asked in case of
    a "GotoX token". Reported/suggested by RetroCogs.

commit 95e87a58929e29e1606c888298d6d02d2a52d500
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Mar 4 20:18:58 2024 +0100

    MEGA65: DMA audio stop + 16 bit samples #398
    
    DMA audio stop (or loop) conidition is checked against the limit after
    incrementing the address. However in case of 16 bit samples it can
    happen that it skips the limit, if the limit is odd and start address is
    even or vice versa.
    
    Reported by @dansanderson

commit 968f7e05ab5fbfeeb288487210c83216da34cbf5
Merge: 8aa261c 4c0a711
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Feb 28 18:38:12 2024 +0100

    Merge pull request #397 from lgblgblgb/next
    
    Merge next as master.

commit 4c0a711f2d066af90275b74d98fdfd9550bbee98
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Feb 13 15:10:09 2024 +0100

    MEGA65: allow OPL work on slow-dev space, too #380
    
    Note, currently I don't know why the slow device space is used for OPL
    why not the native I/O space, or the MEGA65 specific OPL regs
    at $FE000xx which is intended for that very purpose!
    
    btoschi on Discord has great success to make OPL working on MEGA65 but
    requires this access mode, so this quick hack is intended to serve that
    holy purpose :)

commit d810c30278ef825e95251bc4a4359aba5ad2576b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Feb 13 15:07:11 2024 +0100

    MEGA65: matrix mode memory map #209
    
    Plus a 'shade' command to set the transparency of the matrix background.

commit 8574726c6be06b776418dc71e1f420c09b27fd4e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 21 11:55:17 2024 +0100

    MEGA65: avoid ROM start lockup b/c CIA state #395
    
    Note: this is _not_ a proper fix, rather than a workaround by setting
    CIA latched values to $0101 initially on start-up. Without this, newer
    beta ROMs (v920391 and v920392) is left in an infinite loop at their
    start-up routines with some CIA checking magic ... As a real MEGA65
    works without workarounds, this must be an Xemu issue, but the proper
    fix is hard to develop because the inprecise basic foundation of Xemu
    for clock-accurate CIA emulation :( See the mentioned #395 issue above
    for more details.

commit 175e64643cbd11a1180c63c584bbfee548bcbc53
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 8 12:30:28 2024 +0100

    MEGA65: minor uartmon map fix by mteufel
    
    Mteufel pointed out another mistake in register dump. As-is fix
    according to him.

commit 1a6bcf5c894c9e60978140d0de82d083b9be80d8
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 5 13:17:59 2024 +0100

    M65/CORE: allow winpos set/restore #383
    
    This commit allows to set Xemu window position via CLI switch. Also, UI
    menu has been added to be able to save current window position which is
    restored on the next execution of the emulator. The save itself is NOT
    automatic, since it seems, this is a bit awkward (not because of Xemu):
    it seems sometimes SDL2 sees window pos _without_ the decoration border,
    but sometimes with it ... So always saving winpos (window position) and
    always restoring it can cause the window to draft away a bit at every
    executuion, which is annoying ...

commit ea1f46cd927c13e3b2ac1cec759a7add41317400
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jan 2 12:16:05 2024 +0100

    CORE: yay, it's 2024 ...

commit da5feaf6cb74b6ffc6ec411317b5b07a6e778580
Author: Gurce Isikyildiz <Gurce.Isikyildiz@resmed.com.au>
Date:   Fri May 21 13:27:53 2021 +1000

    @220: Some repairs to the 'r' register output, to match more closer to the hardware (particularly the extra map-mask bits in MAPL, MAPH)

commit 8aa261c07ec7c2f9820e99f9c8fb1930fd42e86a
Merge: 2bdb979 2ff51e0
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Dec 20 12:21:40 2023 +0100

    Merge pull request #392 from lgblgblgb/next
    
    New master release

commit 2ff51e095f1b1a9382c145188a6567dd81877d4a
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Dec 13 12:46:23 2023 +0100

    CPU65: Opcode BIT #nn should work as all BIT ops!
    
    For the CPU65 emulator I used (maybe old) datasheet on 65C02, which all stated
    that BIT #immed is special, and only the Z flag is affected, unlike other BIT
    addressing modes. However it seems it was just for early 65C02s. Also
    mega65-core (and it seems also C65 iself) uses the regular implementation for
    immediate addressing mode as well. Just in case, I left open the possibility
    to use the old impementation if CPU65_OLD_BIT_IMMEDIATE is defined.
