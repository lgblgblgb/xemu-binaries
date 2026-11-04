# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20261104234052**) for **Windows**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/dee5189c512c1e540241725258e8a08626379da7**
* **BUILD_DATE = Wed Nov  4 22:43:15 UTC 2026**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu (branch: next)**
* **BUILD_LOG_URL = https://github.com/lgblgblgb/xemu/actions/runs/41927431101**
* **BUILD_OS = (linux) Linux runnervmwuk1x 7.0.0-1019-azure #20-Ubuntu SMP PREEMPT Mon Oct 19 22:41:16 UTC 2026 x86_64 GNU/Linux**
* **BUILD_TARGET = Windows**
* **BUILD_UPTIME =  22:43:15 up 2 min,  0 users,  load average: 2.20, 0.86, 0.32**
* GITHUB_ACTION = __run_19
* GITHUB_ACTIONS = true
* GITHUB_ACTOR = lgblgblgb
* GITHUB_API_URL = https://api.github.com
* GITHUB_ARTIFACTS = /home/runner/work/_temp/_runner_file_commands/artifacts_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_ARTIFACTS_LIST = /home/runner/work/_temp/_runner_file_commands/artifacts_list_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_ENV = /home/runner/work/_temp/_runner_file_commands/set_env_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_EVENT_NAME = push
* GITHUB_GRAPHQL_URL = https://api.github.com/graphql
* GITHUB_JOB = linux-for-windows
* GITHUB_OUTPUT = /home/runner/work/_temp/_runner_file_commands/set_output_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_REF = refs/heads/next
* GITHUB_REF_NAME = next
* GITHUB_REF_PROTECTED = false
* GITHUB_REF_TYPE = branch
* GITHUB_REPOSITORY = lgblgblgb/xemu
* GITHUB_REPOSITORY_OWNER = lgblgblgb
* GITHUB_RETENTION_DAYS = 90
* GITHUB_RUN_ATTEMPT = 1
* GITHUB_RUN_NUMBER = 1068
* GITHUB_SERVER_URL = https://github.com
* GITHUB_STATE = /home/runner/work/_temp/_runner_file_commands/save_state_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_STEP_SUMMARY = /home/runner/work/_temp/_runner_file_commands/step_summary_58ab6c5d-6938-46fa-9aad-0ab7e11931db
* GITHUB_TRIGGERING_ACTOR = lgblgblgb
* GITHUB_WORKFLOW = CI
* GITHUB_WORKFLOW_REF = lgblgblgb/xemu/.github/workflows/main.yml@refs/heads/next
* GITHUB_WORKSPACE = /home/runner/work/xemu/xemu
* TRAVIS_BRANCH = next
* TRAVIS_COMMIT = dee5189c512c1e540241725258e8a08626379da7
* TRAVIS_JOB_WEB_URL = https://github.com/lgblgblgb/xemu/actions/runs/41927431101
* TRAVIS_OS_NAME = linux
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu

## Commit log (last 10)

    commit dee5189c512c1e540241725258e8a08626379da7
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Wed Nov 04 22:37:45 2026 +0000
    
        CORE: additional pref-dir relocation ways
        
        ... untested
        
        [DEPLOYMENT]
    
    commit 2a2130bc535b86eb99ad9e43cfe1387989f64bdc
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Wed Nov 04 22:17:07 2026 +0000
    
        CORE: ignore SIGPIPE signal
    
    commit 4e0b454feaeefd51858f8cfac8bc3a4793e5003d
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Wed Nov 04 22:08:46 2026 +0000
    
        MEGA65: Multi-fire-button joystick emulation #415
        
        ... and some joystick port selection cleanup
    
    commit 8111b31e833029f26caab299a10e4a38046ea2fe
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Wed Nov 04 21:35:38 2026 +0000
    
        CORE: Avoid to write template cfgs in some cases
    
    commit 1b0011d3b474ed732798f66c45eb0280ee40a0be
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Fri Oct 30 12:50:59 2026 +0000
    
        PROJECT: Refined guidelines and no-AI policy
    
    commit f0a711c5a46f49929132ac2272d564cd143d68e6
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sun Oct 11 17:44:24 2026 +0000
    
        BUILD: trying to build multi-arch MacOS binaries
        
        Also, upgrade Ubuntu Linux used for Linux and Windows cross compilation,
        from 24.04 to 26.04
        
        [DEPLOYMENT]
    
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
    
