# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_BlackDuckSca_Auto_FixPR/main`
- **Build Number:** #9
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 11 sec and counting
- **Timestamp:** 2025-11-11 18:46:23 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 003f0981f54e76155b9128d6e30d173f152efee3
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
Checking out Revision 003f0981f54e76155b9128d6e30d173f152efee3 (main)
Commit message: "Update Jenkinsfile"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 003f0981f54e76155b9128d6e30d173f152efee3 # timeout=10
 > git rev-list --no-walk 26eef41b729c1caebfd7eb1c013380b67c63cc2e # timeout=10
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

up to date, audited 1412 packages in 20s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

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
[Pipeline] echo
Workspace is /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main
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
[Security Scan] INFO:  --- blackducksca_fixpr_filter_severities = CRITICAL,HIGH
[Security Scan] INFO:  --- blackducksca_fixpr_maxcount = 2
[Security Scan] INFO:  --- blackducksca_url = https://saastest.app.blackduck.com
[Security Scan] INFO:  --- detect_args = detect.source.path=${WORKSPACE}/nodejs-npm
[Security Scan] INFO:  --- blackducksca_fixpr_useUpgradeGuidance = SHORT_TERM,LONG_TERM
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage blackducksca --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/blackducksca_input15474170316309089226.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-11 18:44:51.6435 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-11 18:44:51.6535 IST [Bridge CLI] INFO: Found version "3.0.143" in registry for workflow "blackducksca", trying to load it from local cache
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: Input Resources:
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: resource = value [source]
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: blackducksca.fixPr.enabled = true [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: blackducksca.fixPr.filter.severities = [CRITICAL HIGH] [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: blackducksca.fixPr.maxCount = 2 [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7606 IST [Bridge CLI] INFO: blackducksca.fixPr.useUpgradeGuidance = [SHORT_TERM LONG_TERM] [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: blackducksca.token = ***************************************** [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: blackducksca.url = https://saastest.app.blackduck.com [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: blackducksca.waitForScan = true [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: detect.args = detect.source.path=${WORKSPACE}/nodejs-npm [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: github.repository.branch.name = main [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: github.repository.name = automatic-fixpr [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: github.repository.owner.name = blackducksca-jenkins-samples [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: github.user.token = ***************************************** [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: network.airgap = false [blackducksca_input15474170316309089226.json]
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 18:44:51.7607 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca
2025-11-11 18:44:51.7610 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Controller
2025-11-11 18:44:51.7660 IST [Bridge CLI] INFO: Starting Adapter: Default Black Duck SCA Scan Mode
2025-11-11 18:44:51.7701 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-11 18:44:51.7966 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-11 18:44:51.7969 IST [Check pull request] INFO: Adapter finished
2025-11-11 18:44:51.8229 IST [Default Black Duck SCA Scan Mode] INFO: Provided value for resource 'blackducksca.scan.full'
2025-11-11 18:44:51.8232 IST [Default Black Duck SCA Scan Mode] INFO: Adapter finished
2025-11-11 18:44:52.6984 IST [Blackduck SCA Controller] INFO: Found Black Duck SCA Detect jar file "detect-11.0.0.jar" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0"
2025-11-11 18:44:52.7233 IST [Blackduck SCA Controller] INFO: Provided value for resource 'detect.execution.path'
2025-11-11 18:44:52.7234 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-detect
2025-11-11 18:44:52.7234 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-11 18:44:52.7234 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-post-processing
2025-11-11 18:44:52.7251 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Results
2025-11-11 18:44:52.7251 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Detect Execution
2025-11-11 18:44:52.7251 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-11 18:44:52.7251 IST [Bridge CLI] INFO: Starting Adapter: Detect Component Locator
2025-11-11 18:44:52.7256 IST [Blackduck SCA Controller] INFO: Adapter finished
2025-11-11 18:44:52.8109 IST [Blackduck SCA Detect Execution] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect --blackduck.offline.mode=false --blackduck.url=https://saastest.app.blackduck.com --blackduck.api.token= --detect.wait.for.results=true --detect.blackduck.scan.mode=INTELLIGENT detect.source.path=${WORKSPACE}/nodejs-npm
2025-11-11 18:44:53.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect-Self-Updater:  Checking https://saastest.app.blackduck.com/api/tools/detect API for centrally managed Detect version to download to /Users/madhusud/tmp.
2025-11-11 18:44:56.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Unable to download jar from https://saastest.app.blackduck.com/api/tools/detect.
2025-11-11 18:44:56.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Response code from https://saastest.app.blackduck.com/api/tools/detect was: 400 Bad Request
2025-11-11 18:44:56.9799 IST [Blackduck SCA Detect Execution] INFO: ______     _            _
2025-11-11 18:44:56.9800 IST [Blackduck SCA Detect Execution] INFO: |  _  \   | |          | |
2025-11-11 18:44:56.9800 IST [Blackduck SCA Detect Execution] INFO: | | | |___| |_ ___  ___| |_
2025-11-11 18:44:56.9800 IST [Blackduck SCA Detect Execution] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-11 18:44:56.9801 IST [Blackduck SCA Detect Execution] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-11 18:44:56.9801 IST [Blackduck SCA Detect Execution] INFO: |___/ \___|\__\___|\___|\__|
2025-11-11 18:44:56.9801 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:44:57.0712 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:44:57.0712 IST [Blackduck SCA Detect Execution] INFO: Detect Version: 11.0.0
2025-11-11 18:44:57.0713 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Current property values:
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- --property = value [notes]
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.api.token = **************************************************************************************************** [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.offline.mode = false [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.url = https://saastest.app.blackduck.com [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.blackduck.scan.mode = INTELLIGENT [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge [env] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.project.name = MBP_Github_BlackDuckSca_Auto_FixPR [env] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.wait.for.results = true [cmd] 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect build date: 2025-10-30
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-13-14-57-063
2025-11-11 18:44:57.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:03.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully connected to Black Duck SCA (version 2025.7.1)!
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Docker tool.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Docker actions finished.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Bazel tool.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Bazel actions finished.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Detectors tool.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Searching for detectors.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detector Report
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm (depth 0)
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/package-lock.json
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/package.json
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detectors actions finished.
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project name: MBP_Github_BlackDuckSca_Auto_FixPR
2025-11-11 18:45:05.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project version: 1.3.0
2025-11-11 18:45:08.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully completed package manager scan of file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact/scan.bdio
2025-11-11 18:45:10.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the codelocation file uploads.
2025-11-11 18:45:14.0000 IST [Blackduck SCA Detect Execution][pool-1-thread-1] INFO: --- Try #1 for task bdio upload (elapsed: 00:00:00.000)...complete!
2025-11-11 18:45:14.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the codelocation file uploads.
2025-11-11 18:45:14.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:14.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Signature Scanner tool.
2025-11-11 18:45:18.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The Black Duck Signature Scanner downloaded/found successfully: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools
2025-11-11 18:45:18.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No scan targets provided - registering the source path /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm to scan
2025-11-11 18:45:19.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the Black Duck Signature Scan commands.
2025-11-11 18:45:19.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck CLI command: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/jre/Contents/Home/bin/java -Done-jar.silent=true -Done-jar.jar.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/cache/scan.cli.impl-standalone.jar -Xmx4096m -jar /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/scan.cli-1.0.6-standalone.jar --no-prompt --scheme https --host saastest.app.blackduck.com --port 443 -v --logDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-13-14-57-063/scan/BlackDuckScanOutput/2025-11-11_13-15-19-685_1 --statusWriteDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-13-14-57-063/scan/BlackDuckScanOutput/2025-11-11_13-15-19-685_1 --project MBP_Github_BlackDuckSca_Auto_FixPR --release 1.3.0 --name nodejs-npm/MBP_Github_BlackDuckSca_Auto_FixPR/1.3.0 signature --exclude /node_modules/ --exclude /.bridge/ --scass-scan /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- 
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck Signature Scanner return code: 0
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Signature Scanner log output directory: '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-13-14-57-063/scan/BlackDuckScanOutput/2025-11-11_13-15-19-685_1'
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the Black Duck Signature Scan commands.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature Scanner actions finished.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Binary Scanner tool.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary scanner found nothing to upload.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary Scanner actions finished.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Container Scanner tool.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No detect.container.scan.file.path property was provided. Skipping container scan.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Container Scanner actions finished.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- IaC Scanner tool will not be run.
2025-11-11 18:45:29.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:45:30.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/dae1d9cf-8c4d-4ae0-9ba1-1f843667a295 (elapsed: 00:00:00.000)...not done yet, waiting 1 seconds and trying again...
2025-11-11 18:45:32.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #2 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/dae1d9cf-8c4d-4ae0-9ba1-1f843667a295 (elapsed: 00:00:01.750)...not done yet, waiting 2 seconds and trying again...
2025-11-11 18:45:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #3 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/dae1d9cf-8c4d-4ae0-9ba1-1f843667a295 (elapsed: 00:00:04.525)...not done yet, waiting 3 seconds and trying again...
2025-11-11 18:45:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #4 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/dae1d9cf-8c4d-4ae0-9ba1-1f843667a295 (elapsed: 00:00:08.312)...complete!
2025-11-11 18:45:39.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Try #1 for task BOM Scan Wait Job https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/bom-status/95eda8a3-8ecc-4fbe-8cac-bfd49b2d89e8 (elapsed: 00:00:00.000)...complete!
2025-11-11 18:45:39.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Checking to see if Detect should check policy for violations.
2025-11-11 18:45:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-13-14-57-063/status/status.json
2025-11-11 18:45:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:40.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Result ========
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck SCA Project BOM: https://saastest.app.blackduck.com/api/projects/6c55a760-f375-42b9-a45b-38fd668aa22c/versions/f65b1d2f-ad64-478e-ab32-24bdcc147338/components
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Status ========
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- NPM: SUCCESS
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature scan / Snippet scan on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm: SUCCESS
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ===============================
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:45:41.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect duration: 00h 00m 47s 848ms
2025-11-11 18:45:41.1689 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.completed'
2025-11-11 18:45:41.1690 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.results.path'
2025-11-11 18:45:41.1692 IST [Blackduck SCA Detect Execution] INFO: Adapter finished
2025-11-11 18:45:42.2285 IST [Blackduck SCA Results] INFO: Bearer token retrieved successfully
2025-11-11 18:45:42.5678 IST [Blackduck SCA Results] INFO: Project data retrieved successfully
2025-11-11 18:45:42.9111 IST [Blackduck SCA Results] INFO: Version data retrieved successfully
2025-11-11 18:45:42.9112 IST [Blackduck SCA Results] INFO: Using configured severities to filter issues: CRITICAL, HIGH
2025-11-11 18:45:44.0504 IST [Blackduck SCA Results] INFO: Vulnerabilities retrieved successfully
2025-11-11 18:45:44.0505 IST [Blackduck SCA Results] INFO: Fetching upgrade guidance for vulnerable BOMs...
2025-11-11 18:46:00.3112 IST [Blackduck SCA Results] INFO: Provided value for resource 'blackducksca.project.id'
2025-11-11 18:46:00.3114 IST [Blackduck SCA Results] INFO: Provided value for resource 'blackducksca.project.version.id'
2025-11-11 18:46:00.3130 IST [Blackduck SCA Results] INFO: Added entry to resource 'blackducksca.issues'
2025-11-11 18:46:00.3159 IST [Blackduck SCA Results] INFO: Adapter finished
2025-11-11 18:46:00.3816 IST [SCM Checker] INFO: Provided value for resource 'jenkins.enabled'
2025-11-11 18:46:00.3816 IST [Bridge CLI] INFO: Starting adapters for stage githubfixpr
2025-11-11 18:46:00.3816 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-policy-violations-fetcher
2025-11-11 18:46:00.3821 IST [Bridge CLI] INFO: Starting Adapter: GitHub Pull Request Handler
2025-11-11 18:46:00.3821 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Policy Violations Fetcher
2025-11-11 18:46:00.3823 IST [SCM Checker] INFO: Adapter finished
2025-11-11 18:46:00.4233 IST [Detect Component Locator] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -cp /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar -Dloader.main=com.blackduck.integration.componentlocator.ComponentLocator org.springframework.boot.loader.PropertiesLauncher /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/detect_component_locator/source-input.json /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm/.bridge/detect_component_locator/components-with-locations.json
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- ##################################################################################################
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #                                                                                                #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  Product Notice                                                                                #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- #                                                                                                #
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- ##################################################################################################
2025-11-11 18:46:00.0000 IST [Detect Component Locator][main] INFO: --- Running Component Locator v2.1.1 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_BlackDuckSca_Auto_FixPR_main/nodejs-npm
2025-11-11 18:46:11.1337 IST [Detect Component Locator] INFO: Using upgrade guidance config ["SHORT_TERM" "LONG_TERM"]
2025-11-11 18:46:11.1337 IST [Detect Component Locator] INFO: Cannot find component locations for component "is-my-json-valid/2.15.0"
2025-11-11 18:46:11.1338 IST [Detect Component Locator] INFO: Cannot find component locations for component "is-my-json-valid/2.19.0"
2025-11-11 18:46:11.1338 IST [Detect Component Locator] INFO: Cannot find component locations for component "getobject/0.1.0"
2025-11-11 18:46:11.1338 IST [Detect Component Locator] INFO: Cannot find component locations for component "handlebars/4.0.5"
2025-11-11 18:46:11.1338 IST [Detect Component Locator] INFO: Cannot find component locations for component "lodash/2.4.2"
2025-11-11 18:46:11.1338 IST [Detect Component Locator] INFO: Cannot find component locations for component "lodash/4.13.1"
2025-11-11 18:46:11.1339 IST [Detect Component Locator] INFO: Cannot find component locations for component "lodash/4.17.11"
2025-11-11 18:46:11.1339 IST [Detect Component Locator] INFO: Cannot find component locations for component "tar/2.2.1"
2025-11-11 18:46:11.1339 IST [Detect Component Locator] INFO: Cannot find component locations for component "tar/4.4.8"
2025-11-11 18:46:11.1340 IST [Detect Component Locator] INFO: Cannot find component locations for component "selenium-webdriver/2.53.3"
2025-11-11 18:46:11.1340 IST [Detect Component Locator] INFO: Cannot find component locations for component "set-value/2.0.0"
2025-11-11 18:46:11.1340 IST [Detect Component Locator] INFO: Cannot find component locations for component "minimist/1.2.5"
2025-11-11 18:46:11.1340 IST [Detect Component Locator] INFO: Cannot find component locations for component "minimist/0.0.10"
2025-11-11 18:46:11.1342 IST [Detect Component Locator] INFO: Cannot find component locations for component "minimist/0.0.8"
2025-11-11 18:46:11.1343 IST [Detect Component Locator] INFO: Cannot find component locations for component "minimist/1.2.0"
2025-11-11 18:46:11.1344 IST [Detect Component Locator] INFO: Cannot find component locations for component "set-value/0.4.3"
2025-11-11 18:46:11.1344 IST [Detect Component Locator] INFO: Cannot find component locations for component "js-yaml/3.6.1"
2025-11-11 18:46:11.1344 IST [Detect Component Locator] INFO: Cannot find component locations for component "mixin-deep/1.3.1"
2025-11-11 18:46:11.1344 IST [Detect Component Locator] INFO: Cannot find component locations for component "nconf/0.10.0"
2025-11-11 18:46:11.1345 IST [Detect Component Locator] INFO: Cannot find component locations for component "bson/1.0.9"
2025-11-11 18:46:11.1345 IST [Detect Component Locator] INFO: Cannot find component locations for component "jsonpointer/4.0.0"
2025-11-11 18:46:11.1345 IST [Detect Component Locator] INFO: Cannot find component locations for component "jsonpointer/4.0.1"
2025-11-11 18:46:11.1346 IST [Detect Component Locator] INFO: Cannot find component locations for component "json-schema/0.2.3"
2025-11-11 18:46:11.1347 IST [Detect Component Locator] INFO: Cannot find component locations for component "adm-zip/0.4.4"
2025-11-11 18:46:11.1347 IST [Detect Component Locator] INFO: Cannot find component locations for component "js-yaml/3.5.5"
2025-11-11 18:46:11.1347 IST [Detect Component Locator] INFO: Cannot find component locations for component "growl/1.9.2"
2025-11-11 18:46:11.1347 IST [Detect Component Locator] INFO: Cannot find component locations for component "fsevents/1.2.9"
2025-11-11 18:46:11.1348 IST [Detect Component Locator] INFO: Cannot find component locations for component "lodash/4.17.20"
2025-11-11 18:46:11.1348 IST [Detect Component Locator] INFO: Cannot find component locations for component "form-data/2.1.4"
2025-11-11 18:46:11.1348 IST [Detect Component Locator] INFO: Cannot find component locations for component "form-data/2.3.3"
2025-11-11 18:46:11.1348 IST [Detect Component Locator] INFO: Cannot find component locations for component "minimatch/0.3.0"
2025-11-11 18:46:11.1349 IST [Detect Component Locator] INFO: Cannot find component locations for component "form-data/2.0.0"
2025-11-11 18:46:11.1349 IST [Detect Component Locator] INFO: Cannot find component locations for component "form-data/1.0.1"
2025-11-11 18:46:11.1349 IST [Detect Component Locator] INFO: Cannot find component locations for component "form-data/0.1.4"
2025-11-11 18:46:11.1349 IST [Detect Component Locator] INFO: Cannot find component locations for component "express/4.16.4"
2025-11-11 18:46:11.1349 IST [Detect Component Locator] INFO: Cannot find component locations for component "nconf/0.6.9"
2025-11-11 18:46:11.1350 IST [Detect Component Locator] INFO: Cannot find component locations for component "ini/1.3.5"
2025-11-11 18:46:11.1350 IST [Detect Component Locator] INFO: Cannot find component locations for component "ini/1.3.4"
2025-11-11 18:46:11.1350 IST [Detect Component Locator] INFO: Cannot find component locations for component "randomatic/1.1.5"
2025-11-11 18:46:11.1351 IST [Detect Component Locator] INFO: Cannot find component locations for component "send/0.16.2"
2025-11-11 18:46:11.1351 IST [Detect Component Locator] INFO: Cannot find component locations for component "dot-prop/4.2.0"
2025-11-11 18:46:11.1351 IST [Detect Component Locator] INFO: Cannot find component locations for component "babel-traverse/6.11.4"
2025-11-11 18:46:11.1351 IST [Detect Component Locator] WARNING: No available upgrade guidance found for "swig/1.4.2" ([SHORT_TERM LONG_TERM]), skipping
2025-11-11 18:46:11.1351 IST [Detect Component Locator] INFO: Cannot find component locations for component "async/2.6.1"
2025-11-11 18:46:11.1352 IST [Detect Component Locator] INFO: Cannot find component locations for component "ajv/6.10.0"
2025-11-11 18:46:11.1352 IST [Detect Component Locator] INFO: Cannot find component locations for component "tough-cookie/2.2.2"
2025-11-11 18:46:11.1352 IST [Detect Component Locator] INFO: Cannot find component locations for component "tough-cookie/2.4.3"
2025-11-11 18:46:11.1352 IST [Detect Component Locator] INFO: Cannot find component locations for component "tough-cookie/2.3.1"
2025-11-11 18:46:11.1352 IST [Detect Component Locator] INFO: Cannot find component locations for component "tough-cookie/2.3.4"
2025-11-11 18:46:11.1353 IST [Detect Component Locator] INFO: Cannot find component locations for component "undefsafe/2.0.2"
2025-11-11 18:46:11.1353 IST [Detect Component Locator] INFO: Cannot find component locations for component "underscore/1.9.1"
2025-11-11 18:46:11.1353 IST [Detect Component Locator] INFO: Cannot find component locations for component "unset-value/1.0.0"
2025-11-11 18:46:11.1353 IST [Detect Component Locator] INFO: Found 3 vulnerable components eligible for PR creation, but MaxCount is set to 2, PRs will be created only for 2 components
2025-11-11 18:46:11.1429 IST [Detect Component Locator] INFO: Added entry to resource 'fixpr.issues'
2025-11-11 18:46:11.1432 IST [Detect Component Locator] INFO: Adapter finished
2025-11-11 18:46:11.2017 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected Intelligent scan, will fetch Intelligent scan policy violations data
2025-11-11 18:46:12.2242 IST [Blackduck SCA Policy Violations Fetcher] INFO: Bearer token retrieved successfully
2025-11-11 18:46:12.5648 IST [Blackduck SCA Policy Violations Fetcher] INFO: Project data retrieved successfully
2025-11-11 18:46:12.9362 IST [Blackduck SCA Policy Violations Fetcher] INFO: Version data retrieved successfully
2025-11-11 18:46:13.2772 IST [Blackduck SCA Policy Violations Fetcher] INFO: Detected 5 policy violations
2025-11-11 18:46:13.6301 IST [Blackduck SCA Policy Violations Fetcher] INFO: Added entry to resource 'blackducksca.policy.rules.violations'
2025-11-11 18:46:13.6306 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.ok'
2025-11-11 18:46:13.6309 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.minor'
2025-11-11 18:46:13.6312 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.critical'
2025-11-11 18:46:13.6316 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.unspecified'
2025-11-11 18:46:13.6319 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.trivial'
2025-11-11 18:46:13.6322 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.blocker'
2025-11-11 18:46:13.6325 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.policy.status.issues.major'
2025-11-11 18:46:13.6328 IST [Blackduck SCA Policy Violations Fetcher] INFO: Provided value for resource 'blackducksca.projectBomUrl'
2025-11-11 18:46:13.6340 IST [Blackduck SCA Policy Violations Fetcher] INFO: Adapter finished
2025-11-11 18:46:14.5538 IST [GitHub Pull Request Handler] INFO: will use default Github API URL "https://api.github.com", as "github.api.url" and "github.host.url" is not configured
2025-11-11 18:46:17.5863 IST [GitHub Pull Request Handler] ERROR: Failed to retrieve "package.json" file contents, skipping file for creating PR: cannot find "package.json" file in the repository, or token has insufficient permissions
2025-11-11 18:46:20.9574 IST [GitHub Pull Request Handler] ERROR: Failed to retrieve "package.json" file contents, skipping file for creating PR: cannot find "package.json" file in the repository, or token has insufficient permissions
2025-11-11 18:46:22.5247 IST [GitHub Pull Request Handler] INFO: Adapter finished
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
Build Number: 9
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