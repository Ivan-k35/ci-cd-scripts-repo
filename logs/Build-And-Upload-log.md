Started by upstream project "JavaAppCI" build number 6
originally caused by:
 Started by user admin
Running as SYSTEM
Building in workspace /home/jenkinsuser/.jenkins/workspace/Build-And-Upload
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/Ivan-k35/java-app-repo.git # timeout=10
Fetching upstream changes from https://github.com/Ivan-k35/java-app-repo.git
 > git --version # timeout=10
 > git --version # 'git version 2.34.1'
 > git fetch --tags --force --progress -- https://github.com/Ivan-k35/java-app-repo.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision 3b5a815eeea45749b2ada36ed72baf108ec81b4d (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 3b5a815eeea45749b2ada36ed72baf108ec81b4d # timeout=10
Commit message: "Update README.md"
 > git rev-list --no-walk 3b5a815eeea45749b2ada36ed72baf108ec81b4d # timeout=10
[Build-And-Upload] $ mvn clean install
[INFO] Scanning for projects...
[INFO] 
[INFO] ---------------------< org.example:SimpleToDoList >---------------------
[INFO] Building SimpleToDoList 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-clean-plugin:2.5:clean (default-clean) @ SimpleToDoList ---
[INFO] Deleting /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ SimpleToDoList ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/src/main/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ SimpleToDoList ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target/classes
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ SimpleToDoList ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ SimpleToDoList ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ SimpleToDoList ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ SimpleToDoList ---
[INFO] Building jar: /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target/SimpleToDoList-1.0-SNAPSHOT.jar
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ SimpleToDoList ---
[INFO] Installing /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target/SimpleToDoList-1.0-SNAPSHOT.jar to /home/jenkinsuser/.m2/repository/org/example/SimpleToDoList/1.0-SNAPSHOT/SimpleToDoList-1.0-SNAPSHOT.jar
[INFO] Installing /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/pom.xml to /home/jenkinsuser/.m2/repository/org/example/SimpleToDoList/1.0-SNAPSHOT/SimpleToDoList-1.0-SNAPSHOT.pom
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  3.424 s
[INFO] Finished at: 2024-01-19T14:59:41+03:00
[INFO] ------------------------------------------------------------------------
Archiving artifacts
Triggering a new build of Deploy-With-Ansible
Finished: SUCCESS
