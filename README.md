# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20210126001453**) for **Linux**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu

This is from the **discord branch** (see below "MASTER"), for regular usage you "should" use **master**.

## Binary versions for **MASTER** (what regular users may prefer):

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Binary versions for **discord**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-discord
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-discord
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-discord

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/5a7fad6d0a5b07fdf30f55b599df4b628f83a993**
* **BUILD_DATE = Tue 26 Jan 2021 01:01:37 AM UTC**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu.git (branch: discord)**
* **BUILD_LOG_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/756174745**
* **BUILD_OS = (linux) Linux lgb 5.4.0-1034-gcp #37-Ubuntu SMP Wed Jan 6 19:44:41 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Linux**
* **BUILD_UPTIME =  01:01:37 up 3 min,  1 user,  load average: 1.36, 0.83, 0.35**
* TRAVIS_APP_HOST = build.travis-ci.org
* TRAVIS_APT_PROXY = http://build-cache.travisci.net
* TRAVIS_ARCH = amd64
* TRAVIS_BRANCH = discord
* TRAVIS_BUILD_DIR = /home/travis/build/lgblgblgb/xemu
* TRAVIS_BUILD_ID = 756174744
* TRAVIS_BUILD_NUMBER = 967
* TRAVIS_BUILD_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/builds/756174744
* TRAVIS_CMD = build/deploy/before-deploy.sh xemu-deploy Linux
* TRAVIS_COMMIT = 5a7fad6d0a5b07fdf30f55b599df4b628f83a993
* TRAVIS_COMMIT_MESSAGE = Discord webhook test
* TRAVIS_COMMIT_RANGE = b8164334cd9f...5a7fad6d0a5b
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
* TRAVIS_JOB_ID = 756174745
* TRAVIS_JOB_NAME = Linux native compilation
* TRAVIS_JOB_NUMBER = 967.1
* TRAVIS_JOB_WEB_URL = https://travis-ci.org/lgblgblgb/xemu/jobs/756174745
* TRAVIS_LANGUAGE = c
* TRAVIS_OS_NAME = linux
* TRAVIS_PRE_CHEF_BOOTSTRAP_TIME = 2021-01-19T09:45:30
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu
* TRAVIS_ROOT = /
* TRAVIS_STACK_FEATURES = generic basic ruby_interpreter
* TRAVIS_STACK_JOB_BOARD_REGISTER = /.job-board-register.yml
* TRAVIS_STACK_LANGUAGES = __ubuntu_2004__ c c++ cplusplus cpp ruby python go java php node_js smalltalk csharp perl rust erlang
* TRAVIS_STACK_NAME = ubuntu_2004
* TRAVIS_STACK_NODE_ATTRIBUTES = /.node-attributes.yml
* TRAVIS_STACK_TIMESTAMP = 2021-01-19 09:45:41 UTC
* TRAVIS_SUDO = true
* TRAVIS_TEST_RESULT = 0
* TRAVIS_TIMER_ID = 1242f978
* TRAVIS_TIMER_START_TIME = 1611622897761492871
* TRAVIS_TMPDIR = /tmp/tmp.nH4GtyyqPj
* TRAVIS_UID = 2000

## Commit log (last 25)

commit 5a7fad6d0a5b07fdf30f55b599df4b628f83a993
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Tue Jan 26 00:14:53 2021 +0100

    Discord webhook test

commit b8164334cd9f5052b2cc8adff0e5aa171d740041
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 25 23:13:33 2021 +0100

    Discord webhook test

commit 812ea795cd12ba7c5fb7f990bb0c40aa7e5f6a8f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 25 18:51:43 2021 +0100

    Discord webhook test

commit 632ee173ba8cfed6b505b0ed760485f556efb08f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 25 15:38:32 2021 +0100

    M65: auto-format just created SDcard image by Xemu
    
    Xemu provides auto creation of the SD-card image file if it's the
    default one (no user override on its path) and it haven't existed yet.
    Thus, it's logical to assume, the user wants to format it. Since it has
    been just created, really, no danger to format it (no data loss) thus
    it's even not worth to bother the user with questions if it's OK to do
    so, or ask the user to use the UI menu to do it. This way, many
    confusion can be avoided for new users, who sees Hyppo's "menu" and try
    to use that to format (which works of course, but more complicated and
    slower). Also the final Xemu signature check has been modified, to tell
    the user how to access the menu at all, and he needs to update the files
    on the card now.

commit ba2b502f81f0dac4f1e7dab462511d5d86358e94
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 24 22:04:27 2021 +0100

    M65: SD-card image creation message/button mods
    
    First, use shorter text for buttons, since on eg Windows, it will not
    fit into the button, hard to realize what those buttons are. Second,
    drop a simple message box after image creation on the further details
    how to continue the process.
    
    Motivated by Phaze101's YT adventures on starting using Xemu.

commit c58ba207f9b3369965378839bcccfec46e691fba
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 24 21:50:35 2021 +0100

    M65: key repeat works with hw-accel kbd D610 #148

commit 52c35b7147ea97df7e6bd22268120cba73ebfc25
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 24 20:51:03 2021 +0100

    CORE: yet another alignment mem round

commit 4637eea464c1251fbecba036de256ebd1fbca143
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 24 19:28:19 2021 +0100

    BUILD: fix a typo on branch detection

commit f24ecec18bc62b0de7138ed3501f0ddc4a1682e3
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 24 19:25:14 2021 +0100

    M65: implement DAT /w bitplane bank select #126

commit e56d7026df43a4316dba196641ad89a31d464040
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Mon Jan 18 00:55:37 2021 +0100

    C65: 'screen to OS paste' for C65 too + RVS mode
    
    Now the screen to ASCII routine is shared, and both of MEGA65 and C65
    emulators can use it. Also implemented the RVS on/off information to be
    rendered as text. Also, some minor clean-ups.

commit 03bb40d3fc9b718d996e93149009939b7c6f7594
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 19:39:04 2021 +0100

    M65: bitplane bank selection + VIC reset

commit 2be7f1b18334661263e8053fdc9f8b724b7a34c3
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 19:36:47 2021 +0100

    CORE: trying to fix some aligned mem problem
    
    Some OSes does not have aligned memory allocation, or at least very
    different schematics. Even the same OS on different platforms have
    different ideas ... Like Linux or Mac on X86 and ARM. C11 standard has a
    standard method for this. Which is not implemented by almost everbody,
    strangely enough :( At least not by Windows and MacOS, it seems.

commit a715aba998a59e3346c47f9f69cb0b39c362618d
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 19:24:15 2021 +0100

    M65: ethertap compilation fix + ARM CPU detection

commit 8d3802a7eeb220fb8adca1f383dd5420b524a0ce
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 18:40:13 2021 +0100

    M65: UI to put screen content to OS paste buffer

commit a47428fbfe71ec171a43810fd051b2ffe48a3dba
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sun Jan 17 17:43:31 2021 +0100

    M65: fix hw accel kbd scanner on C65 keys #225
    
    On MEGA65 the hardware accelarated keyboard scanner implemented faulty
    in Xemu. Since extra C65 keys over the usual C64 8*8 key matrix are
    handled separately, the scan-code space for those are very different,
    causing not working C65 extra keys via $D610 (the hardware accelerated
    keyboard scanner). This patches trying to fix this issue.

commit ffb3a4ae46e11669b84ac3c85c66e8cc39960f8c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 8 23:10:13 2021 +0100

    C65+M65: emu state info, C65 ROM load/UI

commit b1b0c00175f4b5cb8e7cbe375b5811e71f0e651f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 8 22:55:51 2021 +0100

    M65+C65: better ROM date & DMA rev check
    
    Make Xemu's ROM signature detection similar to Hyppo's.
    Also there were some serious issues on setting DMA
    revision automatically by Xemu, needs to be addressed.

commit 2c87181c8a9be91780fbc47b426bb60b7afe247c
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 8 22:27:35 2021 +0100

    CORE: Adding SDL render scale quality + CLI option
    
    ... also some rework on the SDL_SetHint() part of emutools.c
    Hinting is repositioned earlier, as some hints needs prior
    some SDL happenings, ie for example render scale quality needs
    to be done before creating texture (similar problems with some
    other hints). Thanks to Hernan for noticing about the render
    scale quality hinting. This suggested me, to be more careful
    with other hints too.

commit 8b916e34500699c84c26df5a700426487854fbfb
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 8 21:52:23 2021 +0100

    Cosmetic fixes on line endings as whitespaces

commit 6cff51e7b4b2301959f5be5a9055aa09faefb568
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 17:55:27 2021 +0100

    WINDOWS: use 'cmd /c start' to show web page #217

commit 0a5d339229357026bc0fd45557b404dabfa0f2c3
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Sat Jan 2 17:53:51 2021 +0100

    BUILD: fix getting branch name on Ci services, etc

commit 00ec390a49c474093ccba9500e87c3a857b4fa6b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 18:02:11 2021 +0100

    MEGA65: UI update

commit 2769f2aaae880dd0653140c44040b0208adaaa75
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 17:39:49 2021 +0100

    MEGA65: some prep-work for Q ops

commit 0b2de2bd806864e286e169a4e3de551a2fe51a1f
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 17:28:38 2021 +0100

    MEGA65: monitor changes by Gurce

commit f52a9e8da3f87d933748d398653ad6d29a77dc4b
Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
Date:   Fri Jan 1 17:24:38 2021 +0100

    MEGA65: update PRG inject #210
