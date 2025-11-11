# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_BlackDuckSca_Auto_FixPR/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 37 sec and counting
- **Timestamp:** 2025-11-11 16:33:28 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 224ec63738e7d105c286ec0478f7728020fe798f
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/hub_BlackDuckSca_Auto_FixPR_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/.git # timeout=10
 > git config remote.origin.url https://github.com/blackducksca-jenkins-samples/automatic-fixpr.git # timeout=10
Fetching upstream changes from https://github.com/blackducksca-jenkins-samples/automatic-fixpr.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/blackducksca-jenkins-samples/automatic-fixpr.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 224ec63738e7d105c286ec0478f7728020fe798f (main)
Commit message: "Jenkins log upload - Build #2"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 224ec63738e7d105c286ec0478f7728020fe798f # timeout=10
 > git rev-list --no-walk 715550b52accfbc3c62f18583194093adc7b93cd # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_BlackDuckSca_Auto_FixPR/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 12s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (blackduck-security-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
[Pipeline] {
[Pipeline] echo
DETECT_PROJECT_NAME will be set to: MBP_Github_BlackDuckSca_Auto_FixPR
[Pipeline] withEnv
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackDuckSca_Auto_FixPR
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [BLACKDUCKSCA]
[Security Scan] INFO: Parameters for blackducksca:
[Security Scan] INFO:  --- blackducksca_waitForScan = true
[Security Scan] INFO:  --- blackducksca_token = ******************************************************************************
[Security Scan] INFO:  --- blackducksca_fixpr_enabled = true
[Security Scan] INFO:  --- blackducksca_fixpr_filter_severities = CRITICAL
[Security Scan] INFO:  --- blackducksca_fixpr_maxcount = 2
[Security Scan] INFO:  --- blackducksca_url = https://saastest.app.blackduck.com
[Security Scan] INFO:  --- blackducksca_fixpr_useUpgradeGuidance = SHORT_TERM
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Black Duck SCA parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackDuckSca_Auto_FixPR
[Security Scan] INFO: Github repositoryName: automatic-fixpr
[Security Scan] INFO: Github repositoryOwner: blackducksca-jenkins-samples
[Security Scan] INFO: Github branchName: main
[Security Scan] INFO: Github githubHostUrl: https://github.com/
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackDuckSca_Auto_FixPR
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage blackducksca --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/blackducksca_input6767925894377129839.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-11 16:32:18.9014 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-11 16:32:18.9101 IST [Bridge CLI] INFO: Found version "3.0.143" in registry for workflow "blackducksca", trying to load it from local cache
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: Input Resources:
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: resource = value [source]
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: blackducksca.fixPr.enabled = true [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: blackducksca.fixPr.filter.severities = [CRITICAL] [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0160 IST [Bridge CLI] INFO: blackducksca.fixPr.maxCount = 2 [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: blackducksca.fixPr.useUpgradeGuidance = [SHORT_TERM] [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: blackducksca.token = ***************************************** [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: blackducksca.url = https://saastest.app.blackduck.com [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: blackducksca.waitForScan = true [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: github.repository.branch.name = main [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: github.repository.name = automatic-fixpr [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: github.repository.owner.name = blackducksca-jenkins-samples [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: github.user.token = ***************************************** [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: network.airgap = false [blackducksca_input6767925894377129839.json]
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 16:32:19.0161 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca
2025-11-11 16:32:19.0164 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Controller
2025-11-11 16:32:19.0215 IST [Bridge CLI] INFO: Starting Adapter: Default Black Duck SCA Scan Mode
2025-11-11 16:32:19.0257 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-11 16:32:19.0564 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-11 16:32:19.0566 IST [Check pull request] INFO: Adapter finished
2025-11-11 16:32:19.1001 IST [Default Black Duck SCA Scan Mode] INFO: Provided value for resource 'blackducksca.scan.full'
2025-11-11 16:32:19.1003 IST [Default Black Duck SCA Scan Mode] INFO: Adapter finished
2025-11-11 16:32:19.9659 IST [Blackduck SCA Controller] INFO: Found Black Duck SCA Detect jar file "detect-11.0.0.jar" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0"
2025-11-11 16:32:19.9897 IST [Blackduck SCA Controller] INFO: Provided value for resource 'detect.execution.path'
2025-11-11 16:32:19.9899 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-detect
2025-11-11 16:32:19.9899 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-11 16:32:19.9899 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-post-processing
2025-11-11 16:32:19.9919 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Results
2025-11-11 16:32:19.9953 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Detect Execution
2025-11-11 16:32:19.9959 IST [Bridge CLI] INFO: Starting Adapter: Detect Component Locator
2025-11-11 16:32:19.9963 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-11 16:32:19.9968 IST [Blackduck SCA Controller] INFO: Adapter finished
2025-11-11 16:32:20.0711 IST [Blackduck SCA Detect Execution] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect --blackduck.offline.mode=false --blackduck.url=https://saastest.app.blackduck.com --blackduck.api.token= --detect.wait.for.results=true --detect.blackduck.scan.mode=INTELLIGENT
2025-11-11 16:32:20.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect-Self-Updater:  Checking https://saastest.app.blackduck.com/api/tools/detect API for centrally managed Detect version to download to /Users/madhusud/tmp.
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Unable to download jar from https://saastest.app.blackduck.com/api/tools/detect.
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Response code from https://saastest.app.blackduck.com/api/tools/detect was: 400 Bad Request
2025-11-11 16:32:23.2704 IST [Blackduck SCA Detect Execution] INFO: ______     _            _
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: |  _  \   | |          | |
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: | | | |___| |_ ___  ___| |_
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: |___/ \___|\__\___|\___|\__|
2025-11-11 16:32:23.2705 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 16:32:23.3594 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 16:32:23.3594 IST [Blackduck SCA Detect Execution] INFO: Detect Version: 11.0.0
2025-11-11 16:32:23.3594 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Current property values:
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- --property = value [notes]
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.api.token = **************************************************************************************************** [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.offline.mode = false [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.url = https://saastest.app.blackduck.com [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.blackduck.scan.mode = INTELLIGENT [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge [env] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.project.name = MBP_Github_BlackDuckSca_Auto_FixPR [env] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.wait.for.results = true [cmd] 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect build date: 2025-10-30
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-02-23-351
2025-11-11 16:32:23.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:32:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully connected to Black Duck SCA (version 2025.7.1)!
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Docker tool.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Docker actions finished.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Bazel tool.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Bazel actions finished.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Detectors tool.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Searching for detectors.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detector Report
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm (depth 0)
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/package-lock.json
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/package.json
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detectors actions finished.
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project name: MBP_Github_BlackDuckSca_Auto_FixPR
2025-11-11 16:32:31.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project version: 1.3.0
2025-11-11 16:32:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully completed package manager scan of file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact/scan.bdio
2025-11-11 16:32:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the codelocation file uploads.
2025-11-11 16:32:45.0000 IST [Blackduck SCA Detect Execution][pool-1-thread-1] INFO: --- Try #1 for task bdio upload (elapsed: 00:00:00.000)...complete!
2025-11-11 16:32:45.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the codelocation file uploads.
2025-11-11 16:32:45.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:32:45.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Signature Scanner tool.
2025-11-11 16:32:48.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The Black Duck Signature Scanner downloaded/found successfully: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools
2025-11-11 16:32:48.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No scan targets provided - registering the source path /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm to scan
2025-11-11 16:32:50.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the Black Duck Signature Scan commands.
2025-11-11 16:32:50.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck CLI command: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/jre/Contents/Home/bin/java -Done-jar.silent=true -Done-jar.jar.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/cache/scan.cli.impl-standalone.jar -Xmx4096m -jar /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/scan.cli-1.0.6-standalone.jar --no-prompt --scheme https --host saastest.app.blackduck.com --port 443 -v --logDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-02-23-351/scan/BlackDuckScanOutput/2025-11-11_11-02-50-633_1 --statusWriteDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-02-23-351/scan/BlackDuckScanOutput/2025-11-11_11-02-50-633_1 --project MBP_Github_BlackDuckSca_Auto_FixPR --release 1.3.0 --name nodejs-npm/MBP_Github_BlackDuckSca_Auto_FixPR/1.3.0 signature --exclude /node_modules/ --exclude /.bridge/ --scass-scan /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- 
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck Signature Scanner return code: 0
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Signature Scanner log output directory: '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-02-23-351/scan/BlackDuckScanOutput/2025-11-11_11-02-50-633_1'
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the Black Duck Signature Scan commands.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature Scanner actions finished.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Binary Scanner tool.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary scanner found nothing to upload.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary Scanner actions finished.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Container Scanner tool.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No detect.container.scan.file.path property was provided. Skipping container scan.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Container Scanner actions finished.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- IaC Scanner tool will not be run.
2025-11-11 16:33:00.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 16:33:01.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/849ba034-11fe-432d-b198-93c5a0e4be5f (elapsed: 00:00:00.000)...complete!
2025-11-11 16:33:01.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/e89799bf-f052-4bd0-ade8-0f7d3251a61c (elapsed: 00:00:00.000)...not done yet, waiting 1 seconds and trying again...
2025-11-11 16:33:03.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #2 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/e89799bf-f052-4bd0-ade8-0f7d3251a61c (elapsed: 00:00:01.769)...not done yet, waiting 2 seconds and trying again...
2025-11-11 16:33:06.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #3 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/e89799bf-f052-4bd0-ade8-0f7d3251a61c (elapsed: 00:00:04.522)...not done yet, waiting 3 seconds and trying again...
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #4 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/e89799bf-f052-4bd0-ade8-0f7d3251a61c (elapsed: 00:00:08.285)...complete!
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Checking to see if Detect should check policy for violations.
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-11-02-23-351/status/status.json
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Result ========
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck SCA Project BOM: https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/components
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Status ========
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- NPM: SUCCESS
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature scan / Snippet scan on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm: SUCCESS
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ===============================
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 16:33:11.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect duration: 00h 00m 51s 133ms
2025-11-11 16:33:11.7314 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.completed'
2025-11-11 16:33:11.7319 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.results.path'
2025-11-11 16:33:11.7328 IST [Blackduck SCA Detect Execution] INFO: Adapter finished
2025-11-11 16:33:13.3222 IST [Blackduck SCA Results] INFO: Bearer token retrieved successfully
2025-11-11 16:33:13.6603 IST [Blackduck SCA Results] INFO: Project data retrieved successfully
2025-11-11 16:33:14.0343 IST [Blackduck SCA Results] INFO: Version data retrieved successfully
2025-11-11 16:33:14.0344 IST [Blackduck SCA Results] INFO: Using configured severities to filter issues: CRITICAL
2025-11-11 16:33:15.3008 IST [Blackduck SCA Results] INFO: Vulnerabilities retrieved successfully
2025-11-11 16:33:15.3010 IST [Blackduck SCA Results] INFO: Fetching upgrade guidance for vulnerable BOMs...
2025-11-11 16:33:16.1740 IST [Blackduck SCA Results] INFO: Provided value for resource 'blackducksca.project.id'
2025-11-11 16:33:16.1743 IST [Blackduck SCA Results] INFO: Provided value for resource 'blackducksca.project.version.id'
2025-11-11 16:33:16.1746 IST [Blackduck SCA Results] INFO: Added entry to resource 'blackducksca.issues'
2025-11-11 16:33:16.1754 IST [Blackduck SCA Results] INFO: Adapter finished
2025-11-11 16:33:16.2633 IST [SCM Checker] INFO: Provided value for resource 'jenkins.enabled'
2025-11-11 16:33:16.2634 IST [Bridge CLI] INFO: Starting adapters for stage githubfixpr
2025-11-11 16:33:16.2634 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-policy-violations-fetcher
2025-11-11 16:33:16.2639 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Policy Violations Fetcher
2025-11-11 16:33:16.2639 IST [Bridge CLI] INFO: Starting Adapter: GitHub Pull Request Handler
2025-11-11 16:33:16.2641 IST [SCM Checker] INFO: Adapter finished
2025-11-11 16:33:16.3218 IST [Detect Component Locator] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -cp /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar -Dloader.main=com.blackduck.integration.componentlocator.ComponentLocator org.springframework.boot.loader.PropertiesLauncher /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/detect_component_locator/source-input.json /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/detect_component_locator/components-with-locations.json
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- ##################################################################################################
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #                                                                                                #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  Product Notice                                                                                #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- #                                                                                                #
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- ##################################################################################################
2025-11-11 16:33:16.0000 IST [Detect Component Locator][main] INFO: --- Running Component Locator v2.1.1 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 16:33:23.2198 IST [Detect Component Locator] INFO: Using upgrade guidance config ["SHORT_TERM"]
2025-11-11 16:33:23.2198 IST [Detect Component Locator] WARNING: No available upgrade guidance found for "getobject/0.1.0" ([SHORT_TERM]), skipping
2025-11-11 16:33:23.2198 IST [Detect Component Locator] INFO: Cannot find component locations for component "is-my-json-valid/2.19.0"
2025-11-11 16:33:23.2199 IST [Detect Component Locator] INFO: Cannot find component locations for component "is-my-json-valid/2.15.0"
2025-11-11 16:33:23.2254 IST [Detect Component Locator] INFO: Adapter finished
2025-11-11 16:33:23.2753 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected Intelligent scan, will fetch Intelligent scan policy violations data
2025-11-11 16:33:24.2949 IST [Blackduck SCA Policy Violations Fetcher] INFO: Bearer token retrieved successfully
2025-11-11 16:33:24.6684 IST [Blackduck SCA Policy Violations Fetcher] INFO: Project data retrieved successfully
2025-11-11 16:33:25.0056 IST [Blackduck SCA Policy Violations Fetcher] INFO: Version data retrieved successfully
2025-11-11 16:33:25.3477 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected 5 policy violations
2025-11-11 16:33:25.7068 IST [Blackduck SCA Policy Violations Fetcher] INFO: Added entry to resource 'blackducksca.policy.rules.violations'
2025-11-11 16:33:25.7076 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.ok'
2025-11-11 16:33:25.7081 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.unspecified'
2025-11-11 16:33:25.7084 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.minor'
2025-11-11 16:33:25.7087 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.blocker'
2025-11-11 16:33:25.7090 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.critical'
2025-11-11 16:33:25.7093 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.major'
2025-11-11 16:33:25.7096 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.trivial'
2025-11-11 16:33:25.7099 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.projectBomUrl'
2025-11-11 16:33:25.7110 IST [Blackduck SCA Policy Violations Fetcher] INFO: Adapter finished
2025-11-11 16:33:27.8306 IST [GitHub Pull Request Handler] INFO: skipping fix pull requests creation as "fixPR.issues" is found empty
2025-11-11 16:33:27.8398 IST [GitHub Pull Request Handler] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 1095
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:blackducksca-jenkins-samples, repoName:automatic-fixpr, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_BlackDuckSca_Auto_FixPR/main
[Pipeline] echo
Build Number: 3
[Pipeline] echo
GitHub Organization: blackducksca-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: automatic-fixpr
[Pipeline] echo
Target repository: blackducksca-jenkins-samples/automatic-fixpr
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*