## Лог Развертывания JavaAppCI
Started by user admin
Obtained Jenkinsfile from git https://github.com/Ivan-k35/ci-cd-scripts-repo
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /home/jenkinsuser/.jenkins/workspace/JavaAppCI
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /home/jenkinsuser/.jenkins/workspace/JavaAppCI/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/Ivan-k35/ci-cd-scripts-repo # timeout=10
Fetching upstream changes from https://github.com/Ivan-k35/ci-cd-scripts-repo
 > git --version # timeout=10
 > git --version # 'git version 2.34.1'
 > git fetch --tags --force --progress -- https://github.com/Ivan-k35/ci-cd-scripts-repo +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision 0fb9e6f713e139a9d76bfe74c607f562b43dc485 (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 0fb9e6f713e139a9d76bfe74c607f562b43dc485 # timeout=10
Commit message: "Update Jenkinsfile"
 > git rev-list --no-walk 90377433053dec416c02eccfcf99fcdc673f20c3 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] the
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] build
Scheduling project: Build-And-Upload
Starting building: Build-And-Upload #4
Build Build-And-Upload #4 completed: SUCCESS
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Deploy)
[Pipeline] build
Scheduling project: Deploy-With-Ansible
Starting building: Deploy-With-Ansible #11
Build Deploy-With-Ansible #11 completed: SUCCESS
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
Finished: SUCCESS