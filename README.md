# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20230201213937**) for **Linux**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **github branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **github**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-github
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-github
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-github

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/9e3c1c9647687e8e2eb68de49108e18765884610**
* **BUILD_DATE = Wed 01 Feb 2023 08:42:57 PM UTC**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: github)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/594925248**
* **BUILD_OS = (linux) Linux lgb 5.15.0-1017-gcp #23~20.04.2-Ubuntu SMP Wed Aug 17 02:46:40 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Linux**
* **BUILD_UPTIME =  20:42:57 up 2 min,  1 user,  load average: 1.61, 0.78, 0.31**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = github
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 260257456
* TRAVIS_BUILD_NUMBER = 1311
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/260257456
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Linux
* TRAVIS_COMMIT = 9e3c1c9647687e8e2eb68de49108e18765884610
* TRAVIS_COMMIT_MESSAGE = Try travis now ...
* TRAVIS_COMMIT_RANGE = cc323602a99d...9e3c1c964768
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
* TRAVIS_JOB_ID = 594925248
* TRAVIS_JOB_NAME = Linux native compilation
* TRAVIS_JOB_NUMBER = 1311.1
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/594925248
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2022-09-12T10:38:55
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_PRIVATE = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = generic basic ruby_interpreter
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2004__ c c++ cplusplus cpp ruby python generic go java php node_js smalltalk csharp perl rust elixir erlang
* TRAVIS_STACK_NAME = ubuntu_2004
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2022-09-12 10:39:05 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 03bf0e4d
* TRAVIS_TIMER_START_TIME = 1675284177375732134
* TRAVIS_TMPDIR = /tmp/tmp.vZ0HicNoke
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 9e3c1c9647687e8e2eb68de49108e18765884610
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Feb 1 21:39:37 2023 +0100

    Try travis now ...

commit cc323602a99d8380c8d2ce37c1c93de779e537fb
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 13:09:56 2023 +0100

    reCPM: facelift for current Xemu API

commit d2d2af6686b7d7aa3ba4db6195b48e953fb7e533
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 11:33:40 2023 +0100

    github fix try/5

commit 61dc780033a5f3d031f575526f379043873c0c22
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 11:05:28 2023 +0100

    github fix try/4

commit baf5ea31a2c0fc0504f02dbace9111454d145659
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 10:39:47 2023 +0100

    github fix try/3

commit 54562ccadfbc4d53250dcf9f7b74976b05a4f21e
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 10:25:39 2023 +0100

    github fix try/2

commit 92e84baf40dd5d2db6e360e5ebf8f9af800e52ab
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Feb 1 09:52:37 2023 +0100

    github fix try #1

commit a48fa733bafb3f34f2f2fc9fe2ba49e1b2785dc5
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Feb 1 08:55:49 2023 +0100

    Try to fix github action defects ...
    
    Damn github changed something so build does not work anymore. Let's experiment in this branch, deleting travis yml first, to avoid to trigger travis builds all the time here too.

commit 4b62b108cb0fbb3141db482e04fb357135462e94
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Oct 20 19:09:37 2022 +0200

    MEGA65: keep main & colour RAM sync on writes #361
    
    Originally discovered in AnotherWorld's MEGA65 port: #304
    
    It was unknown what causes that, but as Majikeyric noticed, it can be something
    with using glyphs from $1F800-1FFFF area, which is also the 2K colour RAM of
    the C65. It turned out that Xemu's logic is broken when writing colour RAM in
    _general_ to keep the sync between that memory area and the colour RAM, where
    - as a kind of performance hack - it used as a kind of "shadowed area" in Xemu.

commit c434826674a8f5ef1a94ae3c65f41f7ddfb59b77
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Oct 13 21:47:59 2022 +0200

    MEGA65: D68A,B feedback of D81/D64/D71 mount type

commit bee6e9d7c9d561a67e9e41d012ed84b039bb8346
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Oct 13 21:46:46 2022 +0200

    MEGA65: Preliminary support: umon (u)mount disks

commit 8514c7809d4382028df9a2a420c1650b040cfe90
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Oct 12 00:10:00 2022 +0200

    MEGA65: reconstruct VIC-IV video std switching

commit 5410498b23ce4da3385a515ca8038b9252d249f0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Oct 8 21:22:54 2022 +0200

    MacOS: New Apple hw doesn't have right click? #358
    
    It seems newer Apple notebooks do not have ability to produce right
    click with the built-in touch pad (works with external mode). This is
    shocking how lame Apple is, not having INS key, what Apple has at all,
    removing all features? :-O Anyway ;) It seems the standard way is to use
    CTRL + click to emulate right click. However that is not enforced by the
    OS itself and must be done by the applications. SDL2 has this ability,
    but must be requested. So this patch does exactly that.

commit 9435f8df966e750212aed627fe8f045dc546a120
Merge: 36c0a6f f883a64
Author: LGB <lgblgblgb@gmail.com>
Date:   Wed Aug 31 21:15:37 2022 +0200

    Merge pull request #355 from hernandp/sprite-bank-342
    
    Sprite bank (Fix #342)

commit f883a646c02ab6119eeb72df7153a5cdc91e3235
Author: hernandp <hernan.di.pietro@gmail.com>
Date:   Wed Aug 31 14:59:31 2022 -0300

    Sprite data address bits 14-15 fixed

commit 36c0a6f755ec6c3438ddc29517c32e070c3ef866
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 16 15:56:11 2022 +0200

    MEGA65: PETSCII based hw-key-scanner #350

commit f446ac43c34c525a672f84024ddcd64aed4f9efe
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 16 12:35:52 2022 +0200

    MEGA65: hw accel kbd scanner better behaviou #148
    
    Also adding "fake entires" on PRG injection as many people forget to
    emoty $D610 queue and developing on Xemu with PRG injection make them
    think their program is fine (queue is empty), blaming Xemu then when
    they realise it does not work on real MEGA65. By injecting "fake
    entires" into the kbd queue I would like to trigger this typical bug earlier.

commit 6a93fad79369c39e05349d6bee22af45a0858782
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Aug 14 23:19:13 2022 +0200

    M65: Unify C64 keymatrix + C65 keys & decoder #148
    
    Previously, emulated C64 keyboard matrix and the "extra C65 keys" were
    disjoint in the virtual Xemu matrix because of an initial decision in
    Xemu to have RESTORE "between" those. This became problematic though and
    complicated other tasks, especially the hardware accelerated ASCII
    decoder.

commit 7e9c3898afb5915e7ac979b5d26632778be2364f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 9 11:16:16 2022 +0200

    MEGA65: FPGA-based random number generator 'TRNG'
    
    See: https://github.com/MEGA65/mega65-core/issues/600 about the
    MEGA65-core implementation of this. Now just a naive rand() call here to
    try to mimic the behaviour at least to get "some" random number by
    reading register $D7EF in MEGA65 I/O mode.

commit f4162ccd3bccbe251ea9c0ca85cc2a4680727a68
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Aug 9 11:03:39 2022 +0200

    MEGA65: ability to use Xemu as tester tool #352
    
    Add screenshot before exit feature and a way to trigger this from
    programs as well in "testing mode".

commit 7ba911b26768206e1dd494c6af6d2a7723547ee6
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jul 16 11:35:07 2022 +0200

    CORE,M65: ability to use Xemu as tester tool #352
    
    CORE: added headless and sleepless mode to run Xemu without any output,
    and to run at max speed without trying to sync to emulated target speed.
    MEGA65: added -headless and -sleepless CLI options to expose these
    features in the MEGA65 emulator.
    
    MEGA65: added -dumpscreen CLI option to dump text screen in form of
    ASCII values at exit time. Also an UI menu option to use this promptly.
    
    MEGA65: inject framework (made for -prg etc) is re-worked to use more
    precise VIC-IV values of the current screen memory etc.

commit 7f13d772f7047645ec19d0784ad7f00c415ca90c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jul 16 11:31:17 2022 +0200

    M65: SID osc3 read val, FPGA temperature
    
    Add emulation of some source of possible entropy used by some programs
    to generate "random" numbers. For SID regs, the behaviour is VERY MUCH
    NOT correct, but still better than before when reading those registers
    produced a constant value only ...

commit 0bcae956cb27dc7ea3df81b78adb403c60adc812
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jul 4 09:32:32 2022 +0200

    PC: Import of unfinished PC emulator from 'dev'
    
    Unfinished PC emulator using (reworked) FAKE86 infrastrcture. Please do
    not even have a look on it right now.
    
    The only reason of this commit to have some "base" for further
    development on this emulator (outside of the 'dev' branch as well).
    
    Note, that it should have unified with my tree of Fake86 (fork of the original
    Fake86). Both of them may contain useful modifications/cleanups on the CPU
    emulation which should be important to make nicer first ...
    
    My Fake86 fork: https://github.com/lgblgblgb/fake86

commit 3c7f169adbcaf1b09c5567d7bf13882b7cb97c85
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Jun 16 22:26:05 2022 +0200

    M65: implement CPU-addr DMA-lists #198
    
    * Implementing $D706 triggered DMA session, when address is "CPU
      address"
    * Implementing $D707 triggered DMA session (in mega65-core it's not done
      yet, but planned!) meaning "in-line DMA": the address is from CPU PC
      automatically, only $D707 must be written, DMA list bytes read by PC,
      and after the DMA session, CPU execution continues after the last byte
      of the DMA list ($D706 is simply any 16 bit CPU address, not the PC
      based scheme!)

commit 849002ed58d511901fabe144fcd8ce1e2d16411c
Author: lgblgblgb <lgblgblgb@gmail.com>
Date:   Wed Jun 15 15:58:53 2022 +0200

    M65: limit scr/colorRAM range in VIC-4 emulation
    
    For #349
