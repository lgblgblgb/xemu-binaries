# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20260928222910**) for **MacOS**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/042400177af3d773732763d731f2fcc4316d8322**
* **BUILD_DATE = Mon Sep 28 22:06:06 UTC 2026**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu (branch: next)**
* **BUILD_LOG_URL = https://github.com/lgblgblgb/xemu/actions/runs/36490186909**
* **BUILD_OS = (darwin) Darwin iad01-dz253-121c98f9-1a46-452d-9624-5916ccf24076-0A29C99A7966.local 24.6.0 Darwin Kernel Version 24.6.0: Tue Jul 21 20:50:07 PDT 2026; root:xnu-11417.140.69.711.44~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME = 22:06  up 9 mins, 1 user, load averages: 2.18 9.02 7.90**
* GITHUB_ACTION = __run_14
* GITHUB_ACTIONS = true
* GITHUB_ACTOR = lgblgblgb
* GITHUB_API_URL = https://api.github.com
* GITHUB_ARTIFACTS_LIST = /Users/runner/work/_temp/_runner_file_commands/artifacts_list_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_ARTIFACTS = /Users/runner/work/_temp/_runner_file_commands/artifacts_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_ENV = /Users/runner/work/_temp/_runner_file_commands/set_env_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_EVENT_NAME = workflow_dispatch
* GITHUB_GRAPHQL_URL = https://api.github.com/graphql
* GITHUB_JOB = macos
* GITHUB_OUTPUT = /Users/runner/work/_temp/_runner_file_commands/set_output_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_REF_NAME = next
* GITHUB_REF_PROTECTED = false
* GITHUB_REF_TYPE = branch
* GITHUB_REF = refs/heads/next
* GITHUB_REPOSITORY_OWNER = lgblgblgb
* GITHUB_REPOSITORY = lgblgblgb/xemu
* GITHUB_RETENTION_DAYS = 90
* GITHUB_RUN_ATTEMPT = 1
* GITHUB_RUN_NUMBER = 1039
* GITHUB_SERVER_URL = https://github.com
* GITHUB_STATE = /Users/runner/work/_temp/_runner_file_commands/save_state_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_STEP_SUMMARY = /Users/runner/work/_temp/_runner_file_commands/step_summary_7572d9af-f8f0-4ef8-af8b-b925e7550030
* GITHUB_TRIGGERING_ACTOR = lgblgblgb
* GITHUB_WORKFLOW_REF = lgblgblgb/xemu/.github/workflows/main.yml@refs/heads/next
* GITHUB_WORKFLOW = CI
* GITHUB_WORKSPACE = /Users/runner/work/xemu/xemu
* TRAVIS_BRANCH = next
* TRAVIS_COMMIT = 042400177af3d773732763d731f2fcc4316d8322
* TRAVIS_JOB_WEB_URL = https://github.com/lgblgblgb/xemu/actions/runs/36490186909
* TRAVIS_OS_NAME = darwin
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu

## Commit log (last 10)

    commit 042400177af3d773732763d731f2fcc4316d8322
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Mon Sep 28 20:29:10 2026 +0000
    
        MEGA65: add missing emutools fn's for future use
    
    commit 48f6586fa99e5574a95d87e0374ff9664c08b8e1
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Mon Sep 28 20:03:11 2026 +0000
    
        MEGA65: fix buf overflow on screen cmd injection
        
        The issue has been originally reported by ctalkobt on Discord
    
    commit 50792fecb0a60164bd9e4f153e0c8be7b3f017cb
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Mon Sep 28 20:10:38 2026 +0000
    
        BUILD: releases page workflow fix
        
        target_commitish must be used it seems, otherwise the tag is put on the
        master head always!
    
    commit 53f60c9c5fa86ac781988f9244f09ef9062d9902
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Fri Apr 24 20:26:15 2026 +0000
    
        CORE: XEMU_NO_DIALOGS env variable sensing
        
        To avoid dialogs even in the config/CLI parsing phase
        
        [DEPLOYMENT]
    
    commit 2391eb59edec96932c4742b51289b9c55d451638
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Thu Aug 06 21:16:40 2026 +0000
    
        MEGA65: mouse emulation only in mouse grab mode
        
        Basically reverting commit 73949895d9051c63c1a90cb5b13416fb45474201
        with some addition. The original intent was:
        
            The problem: Xemu user may leave mouse grab mode to do something with
            their mouse. To avoid bothering the mouse-aware MEGA65 program running,
            I returned zero for relative mouse position change in this case. However
            that can cause problems with certain programs which are not mouse based
            and expecting $FF if mouse is not there.
        
        However this solution is complicated, as the user needs to modify Xemu
        configuration each time, since newer joystick support was added to ROM
        using the POT lines as the mouse too. Thus now, without disabled mouse
        emulation, there will be phantom extra joy presses all the time.
        
        Instead of the user needs to enable/disable mouse emulation all the
        time, let's present mouse emulation only in grab mode. It introduce some
        mouse position "jump" on entering/leaving mouse grab mode, but it's
        still mouse better than the previous complicated solution, I think.
        
        Somewhat related: #415
    
    commit 1036513d9207fea6c08bdfdf8563267b6aa8ae25
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Wed Apr 29 21:46:36 2026 +0000
    
        MEGA65: adding undocumented LDQ nnnn,Y opcode
    
    commit 9a1251089c2cac479eb6df26cc8a14e577da0df4
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Thu Aug 06 18:09:07 2026 +0000
    
        DEPLOY: deploy to github releases page, too #447
    
    commit f95530a1f714c15e0ee342df293c80cb300ba704
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Thu Apr 09 18:31:17 2026 +0000
    
        MEGA65: result must be zero when divide by zero
        
        As strange as sounds, this is how mega65-core behaves currently.
        Previously, the core set all result register bits to '1' but it seems
        it's no longer the case since this mega65-core commit:
        
        https://github.com/MEGA65/mega65-core/commit/ed1794e5f49dc09ed415d7fd4fb788ddee1c0e6c
        
        and now all bits should be set to '0' instead.
        
        Reported by @MirageBD
        
        [DEPLOYMENT]
    
    commit 7984458c8b2fe8596c529022f9bece568c8f693c
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Mon Apr 06 22:11:03 2026 +0000
    
        MEGA65: EMSCRIPTEN refinements #96
        
        Separating CSS and JS stuff from the shell HTML, more functionality.
    
    commit a7eb18145250c9584cb713e50285c926b8efa818
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Fri Apr 03 20:55:17 2026 +0000
    
        MEGA65: new reset type (soft)
        
        Trying to 'simulate' a full system reset after at least a single
        successfull real system reset, but faster.
        
        Especially useful with the EMSCRIPTEN build #96
        Because normal hyppo based reset is *SLOW* there even with -fastboot
    
