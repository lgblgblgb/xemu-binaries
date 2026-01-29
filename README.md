# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20260129235930**) for **MacOS**. For the source code, further
information and instructions, wiki, issue page, etc, please visit
https://github.com/lgblgblgb/xemu









## Binary versions for **master**:

* Windows 32/64 bit binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-windows-master
* MacOS binaries: https://github.com/lgblgblgb/xemu-binaries/tree/binary-osx-master
* Ubuntu Linux DEB packages: https://github.com/lgblgblgb/xemu-binaries/tree/binary-linux-master

## Information section

These versions are built automatically on deployment request on Travis CI. Even this README ...


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/40dfef0d1d5f56be2469492715c12bdb32c75b67**
* **BUILD_DATE = Thu Jan 29 23:42:05 UTC 2026**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu (branch: master)**
* **BUILD_LOG_URL = https://github.com/lgblgblgb/xemu/actions/runs/21498740962**
* **BUILD_OS = (darwin) Darwin sat12-jr322-76ef5122-759f-4553-9975-b327823f2278-72FF733DF69E.local 24.6.0 Darwin Kernel Version 24.6.0: Wed Nov  5 21:30:23 PST 2025; root:xnu-11417.140.69.705.2~1/RELEASE_X86_64 x86_64**
* **BUILD_TARGET = MacOS**
* **BUILD_UPTIME = 23:42  up 41 mins, 1 user, load averages: 2.02 1.11 1.31**
* GITHUB_ACTION = __run_14
* GITHUB_ACTIONS = true
* GITHUB_ACTOR = lgblgblgb
* GITHUB_API_URL = https://api.github.com
* GITHUB_ENV = /Users/runner/work/_temp/_runner_file_commands/set_env_300cce22-ad18-4f3f-a81e-16f28cbdfb28
* GITHUB_EVENT_NAME = workflow_dispatch
* GITHUB_GRAPHQL_URL = https://api.github.com/graphql
* GITHUB_JOB = macos
* GITHUB_OUTPUT = /Users/runner/work/_temp/_runner_file_commands/set_output_300cce22-ad18-4f3f-a81e-16f28cbdfb28
* GITHUB_REF_NAME = master
* GITHUB_REF_PROTECTED = false
* GITHUB_REF_TYPE = branch
* GITHUB_REF = refs/heads/master
* GITHUB_REPOSITORY_OWNER = lgblgblgb
* GITHUB_REPOSITORY = lgblgblgb/xemu
* GITHUB_RETENTION_DAYS = 90
* GITHUB_RUN_ATTEMPT = 1
* GITHUB_RUN_NUMBER = 1004
* GITHUB_SERVER_URL = https://github.com
* GITHUB_STATE = /Users/runner/work/_temp/_runner_file_commands/save_state_300cce22-ad18-4f3f-a81e-16f28cbdfb28
* GITHUB_STEP_SUMMARY = /Users/runner/work/_temp/_runner_file_commands/step_summary_300cce22-ad18-4f3f-a81e-16f28cbdfb28
* GITHUB_TRIGGERING_ACTOR = lgblgblgb
* GITHUB_WORKFLOW_REF = lgblgblgb/xemu/.github/workflows/main.yml@refs/heads/master
* GITHUB_WORKFLOW = CI
* GITHUB_WORKSPACE = /Users/runner/work/xemu/xemu
* TRAVIS_BRANCH = master
* TRAVIS_COMMIT = 40dfef0d1d5f56be2469492715c12bdb32c75b67
* TRAVIS_JOB_WEB_URL = https://github.com/lgblgblgb/xemu/actions/runs/21498740962
* TRAVIS_OS_NAME = darwin
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu

## Commit log (last 10)

    commit 40dfef0d1d5f56be2469492715c12bdb32c75b67
    Author: LGB <lgblgblgb@gmail.com>
    Date:   Thu Jan 29 22:59:30 2026 +0000
    
        Merge pull request #445 from lgblgblgb/next
        
        Next
    
    commit 58dee4db7d0976d5c9b601d4565d1b6a4a2f9324
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Tue Jan 20 19:25:47 2026 +0000
    
        2026 is here
    
    commit fdeb691eba6e4b546698bf418262dfbc840a3099
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sun Nov 23 21:32:28 2025 +0000
    
        MEGA65: fix $D60F cursor up/left key query
        
        Thanks to RetroCogs for reporting.
        
        [DEPLOYMENT]
    
    commit b876bad158042ff8ea5902e6023e16229842ce03
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sun Nov 23 20:26:47 2025 +0000
    
        BUILD: using macos-15-intel on github actions
        
        Github obsoleted macos-13 runner, trying macos-15-intel instead ...
    
    commit 60c7d45f4d04ff229faa390e99064d87c11a4f25
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sun Nov 23 20:25:29 2025 +0000
    
        MEGA65: ethernet emu additional works #242
    
    commit 9aa14264b3a71f55af5f7e4d62ddb225e897ceda
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Tue Oct 14 21:51:19 2025 +0000
    
        MEGA65: ethertap build error fix if no debug #242
    
    commit e7fa61a988b71ff1e6b40fd63be0a1daf11466fe
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Tue Oct 14 21:43:46 2025 +0000
    
        MEGA65: WIP, first try of new ethertap #242
    
    commit 0e50c6f1d1d0f53db07d240ad48cffd1f0e535c3
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Mon Oct 06 11:13:02 2025 +0000
    
        CORE: Fix MacOS change breaking BSD sockets #441
        
        It seems Apple has introduced some significant changes in Mac headers
        which breaks many UNIX/BSD socket code. Fortunately, it seems a
        simple:
        
        helps to go back from insanity to normality, thanks, Apple ;)
        
        Thanks to @geir-straume for reporting the issue:
        
        https://github.com/lgblgblgb/xemu/issues/441
        
        The problem was hidden, since github actions still uses an older MacOS
        which does not have this problem yet, so Xemu compiles fine with that
        OS version.
    
    commit 54bf011f847f11d3604dade7fcbec1002c3a3f75
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sat Oct 04 21:41:48 2025 +0000
    
        CORE: add main thread checker
    
    commit 0f50548d330eabf283acaa991bd240de1bc872d7
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sat Oct 04 21:38:06 2025 +0000
    
        MEGA65: rudimentary VIC info for matrix
    
