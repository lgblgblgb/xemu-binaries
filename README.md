# X-Emulators ~ "Xemu" / Binary distribution

This is the **binary** distribution of Xemu (**20260807000921**) for **Linux**. For the source code, further
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


* **BUILD_COMMIT = https://github.com/lgblgblgb/xemu/commit/53f60c9c5fa86ac781988f9244f09ef9062d9902**
* **BUILD_DATE = Thu Aug  6 22:16:54 UTC 2026**
* **BUILD_GIT_REMOTE = https://github.com/lgblgblgb/xemu (branch: next)**
* **BUILD_LOG_URL = https://github.com/lgblgblgb/xemu/actions/runs/31128863923**
* **BUILD_OS = (linux) Linux runnervmvrwv9 6.17.0-1020-azure #20~24.04.1-Ubuntu SMP Fri Jun 19 20:09:14 UTC 2026 x86_64 x86_64 x86_64 GNU/Linux**
* **BUILD_TARGET = Linux**
* **BUILD_UPTIME =  22:16:54 up 2 min,  0 user,  load average: 1.81, 0.79, 0.30**
* GITHUB_ACTION = __run_13
* GITHUB_ACTIONS = true
* GITHUB_ACTOR = lgblgblgb
* GITHUB_API_URL = https://api.github.com
* GITHUB_ARTIFACTS = /home/runner/work/_temp/_runner_file_commands/artifacts_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_ARTIFACTS_LIST = /home/runner/work/_temp/_runner_file_commands/artifacts_list_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_ENV = /home/runner/work/_temp/_runner_file_commands/set_env_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_EVENT_NAME = workflow_dispatch
* GITHUB_GRAPHQL_URL = https://api.github.com/graphql
* GITHUB_JOB = linux-native
* GITHUB_OUTPUT = /home/runner/work/_temp/_runner_file_commands/set_output_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_REF = refs/heads/next
* GITHUB_REF_NAME = next
* GITHUB_REF_PROTECTED = false
* GITHUB_REF_TYPE = branch
* GITHUB_REPOSITORY = lgblgblgb/xemu
* GITHUB_REPOSITORY_OWNER = lgblgblgb
* GITHUB_RETENTION_DAYS = 90
* GITHUB_RUN_ATTEMPT = 1
* GITHUB_RUN_NUMBER = 1027
* GITHUB_SERVER_URL = https://github.com
* GITHUB_STATE = /home/runner/work/_temp/_runner_file_commands/save_state_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_STEP_SUMMARY = /home/runner/work/_temp/_runner_file_commands/step_summary_b1b96f0e-1b42-473c-be2c-c92c23e44d6a
* GITHUB_TRIGGERING_ACTOR = lgblgblgb
* GITHUB_WORKFLOW = CI
* GITHUB_WORKFLOW_REF = lgblgblgb/xemu/.github/workflows/main.yml@refs/heads/next
* GITHUB_WORKSPACE = /home/runner/work/xemu/xemu
* TRAVIS_BRANCH = next
* TRAVIS_COMMIT = 53f60c9c5fa86ac781988f9244f09ef9062d9902
* TRAVIS_JOB_WEB_URL = https://github.com/lgblgblgb/xemu/actions/runs/31128863923
* TRAVIS_OS_NAME = linux
* TRAVIS_PULL_REQUEST = false
* TRAVIS_REPO_SLUG = lgblgblgb/xemu

## Commit log (last 10)

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
    
    commit 69b4042142a87e6d43dcac3d9d05a3810bee68ff
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Fri Apr 03 09:44:41 2026 +0000
    
        MEGA65: EMSCRIPTEN gateway separation #96
    
    commit 261b9a5287981416fe9709e012a4ed0501c88885
    Author: LGB (Gabor Lenart) <lgblgblgb@gmail.com>
    Date:   Sat Mar 28 12:24:28 2026 +0000
    
        MEGA65: EMSCRIPTEN improvements + own shell #96
    
    commit 4e0f2a3add82e3d832cec78c23f6f897954d462c
    Author: RetroCogs <45956643+RetroCogs@users.noreply.github.com>
    Date:   Wed Mar 18 20:12:42 2026 +0000
    
        MEGA65: alt palette select only if rowmask=0 #442
        
        Original PR: https://github.com/lgblgblgb/xemu/pull/443
        
        mega65-core bug: https://github.com/MEGA65/mega65-core/issues/797
        
        [DEPLOYMENT]
    
