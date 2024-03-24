# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20240324232624**) for **Linux**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/d96aaeb131299f274f277e81c613dd99a9004894**
* **BUILD_DATE = Sun Mar 24 10:33:19 PM UTC 2024**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: next)**
* **BUILD_LOG_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/619640388**
* **BUILD_OS = (linux) Linux lgb 6.2.0-1018-gcp #20~22.04.1-Ubuntu SMP Mon Oct 23 12:29:43 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Linux**
* **BUILD_UPTIME =  22:33:19 up 2 min,  1 user,  load average: 1.10, 0.56, 0.22**
* TRAVIS_APP_HOST = build.travis-ci.com
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = next
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 269630919
* TRAVIS_BUILD_NUMBER = 1390
* TRAVIS_BUILD_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/builds/269630919
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Linux
* TRAVIS_COMMIT = d96aaeb131299f274f277e81c613dd99a9004894
* TRAVIS_COMMIT_MESSAGE = BUILD: use newer ubuntu LTS on Travis CI
* TRAVIS_COMMIT_RANGE = 95e87a58929e...d96aaeb13129
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
* TRAVIS_JOB_ID = 619640388
* TRAVIS_JOB_NAME = Linux native compilation
* TRAVIS_JOB_NUMBER = 1390.1
* TRAVIS_JOB_WEB_URL = https://app.travis-ci.com/lgblgblgb/xemu/jobs/619640388
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
* TRAVIS_TIMER_ID = 1d00c580
* TRAVIS_TIMER_START_TIME = 1711319599193662830
* TRAVIS_TMPDIR = /tmp/tmp.mGhgBNXzmO
* TRAVIS_UID = 2000

## Commit log (last 25)

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

commit 6122459b6f70ee4d0bd41f15bb9c490273d6bfd4
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Dec 6 00:02:12 2023 +0100

    MEGA65: text pasting via hw kbd queue #391
    
    Originally part of issue #103
    
    Implementing some "paste text" (from OS paste buffer) is something which
    is really hard to do with Xemu/MEGA65. A C64 emulator usually injects
    into the software keyboard buffer implemented by the ROM. I cannot do
    that with a MEGA65 emulator since the wide variation of ROMs and ROM
    versions are in case. This method though used the _hardware_ keyboard
    scanner queue which is not ROM dependent, so it's fine. However the
    disadvantage: only works with newer ROMs and won't work in "GO64" mode.

commit e7119f3d36a3c80e5a2262db22f0231b5c3f0da0
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Dec 5 10:36:01 2023 +0100

    MEGA65: unified hw kbd scanner queue #391
    
    Newer beta ROMs use the concept of the new unified hardware keyboard scanner
    queue scheme. This also required change in mega65-core.

commit 2cf798333fef29c6ab79777417c04e3456bcce66
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Nov 27 00:54:06 2023 +0100

    MEGA65: forcing R/W HDOS D81 mounts #390
    
    It seems - for whatever unknown reasons - HDOS instructs R/O mounts when
    HDOS virtualisation is turned off (ie, D81 mounts from the - emulated -
    SD-card). No idea why it happens, but here it is a quick workaround which
    forces R/W mount, rehardless of whatever HDOS want to do. Part of #367

commit 393dd267d2c146b428df2ca00dc46051ddbf6462
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Nov 9 22:07:14 2023 +0100

    MEGA65: refine the message for UI format sd-card
    
    Some users were scared that their whole OS (ie, Windows, etc) will be
    deleted because of the wording of the warning window. Let's try not to
    scare users away :)

commit 2cc8eb2b31ae60fc5569efea514d500a97ce0b0d
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Nov 6 15:06:26 2023 +0100

    ANDROID: porting to android: phase-1 #98
    
    Currently nothing works yet, just the ability to actually run configure
    for Android cross-compilation on UNIX, and allow the compilation
    succeeded till the point of getting a shared object. Surely, this alone
    is not useful for anything, an APK should be built, JNI activation
    should be added, and these all do not mean it actually runs on any
    Android device yet, still ...
    
    Thanks btoschi on Discord for the chat on the topic and for some useful
    tips here and there.

commit 4bfa730f0b3a88d3647fcc9d9bdd04cd8d9948d9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Nov 6 15:02:07 2023 +0100

    MEGA65: matrix 2nd page + new disassembly ability
    
    The second page feature is not perfect yet, causing glitches on paging
    back and forth. Page UP/DOWN can be used to see the previous and the
    current (active) page of the "matrix console".
    
    Disassembly can be done in matrix mode with the "a" command, which
    requires some address parameter, the syntax follows the "d" (dump)
    command in that regard. Command "a" alone just continues the disassembly
    from the last address.
    
    WARNING: disassembly can be buggy/incorrect, it was not highly checked
    yet, if it's 100% accurate. It knows the MEGA65 "compound" opcodes as
    well.

commit 3e4011768dccc980e762f3cbf3cc21f854a1f80e
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Wed Oct 25 09:36:31 2023 +0200

    MEGA65: matrix mode new features
    
    * Left CTRL and TAB is used now for toogling matrix mode
    
      Previously, right ALT-TAB was used, however it seems that's often
      captured by the OS, not only left ALT-TAB, what I would expect
    
    * Live-update of memory dumps
    
      If a memory dump can be seen on the matrix screen, it is constantly
      updated "magically". The new matrix command `live` can be used to
      turn this behaviour on/off
    
    * History buffer
    
      History buffer for command editing, can be accessed by up/down cursor
      keys as you would expect
    
    * New config options and UI menu item addition
    
      `-matrixstart` can be used to start Xemu with matrix enabled ASAP,
      `-matrixdisable` can be used to disable the matrix hotkey, if you
      are in a situation that CTRL-ALT must be used inside the emulation
      for something else. "Matrix disable" can be accessed via UI menu
      as well in the "Debug/Advanced" menu.

commit 7f73f1984e688150f0122609aa560ba430213962
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Oct 24 09:45:27 2023 +0200

    MEGA65: restore default config UI option
    
    The new "Restore default config" option internally just deletes the
    configuration file, so any previously saved config lost, thus the
    "factory default" is restored this way.

commit d879741217cc3e1aa29705ba613558b000bebc45
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 21 23:26:04 2023 +0200

    MEGA65: row-mask for RRB (first try) #363

commit 8c643476536d92636c7c43e52301d89ae1816f50
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 21 23:21:19 2023 +0200

    MEGA65: alt-palette in FCM mode on bold+inverse
    
    Alternative palette feature was implemented before in Xemu/MEGA65 for
    RRB, and for the monochrome character renderer, but not for FCM mode.

commit 0ea6fe85d74c4cd3845d337be72c06a76fadefc9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Sep 15 21:16:02 2023 +0200

    MEGA65: PETSCII kbd empty = $FF + xlat table mods #388

commit 7474cc87347e32de364f8bfaf6b6da3b3deaf1c9
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Sep 11 10:24:12 2023 +0200

    MEGA65: new compressed R/O SD image format
    
    Can be more useful with emscripten #96 where a 4Gbyte sized image
    is very unrealistic. The old format allowed compression of my image
    to about 20-30Mbyte, this one is down to about 500K which means much
    less data transfer needs from the browser. It uses RLE kind of
    compression methods, and uncompressed on-the-fly per 64K "pages" basis
    to have a balance between peformance, memory usage and compression.

commit 9a1a079e14d6e079054e19967b41d830e960d84b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Sep 9 19:07:42 2023 +0200

    WINDOWS: allow regkey to silent OS warnings #385

commit d7d3799a2a7cec51c1c277e45d4c074b91591531
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Thu Sep 7 23:07:15 2023 +0200

    WINDOWS: use Windows-10 UTF-8 FS funcs #385
    
    Since a while, Microsoft **FINALLY** introduced a way to allow to use
    UTF-8 filenames using the normal UNIX/POSIX-like FS API (thus with
    "narrow" functions not the "wide" ones!). So finally **AT LAST** we can
    unify standard functions on all OSes, where Windows was always lagging
    behind! See issue #385 for more details. This though will cause problems
    for users running Xemu on older Windows OS versions .............
