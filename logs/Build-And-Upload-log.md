# Лог сборки проекта Java через Jenkins

- **Started by upstream project "JavaAppCI" build number 6**
  - originally caused by:
    - Started by user admin
- **Running as SYSTEM**
- **Building in workspace /home/jenkinsuser/.jenkins/workspace/Build-And-Upload**
- **The recommended git tool is: NONE**
- **No credentials specified**

## Git Operations
- **Fetching changes from the remote Git repository**
  - `git config remote.origin.url https://github.com/Ivan-k35/java-app-repo.git # timeout=10`
  - `git --version # 'git version 2.34.1'`
  - `git fetch --tags --force --progress -- https://github.com/Ivan-k35/java-app-repo.git +refs/heads/:refs/remotes/origin/ # timeout=10`
- **Checking out Revision**
  - `3b5a815eeea45749b2ada36ed72baf108ec81b4d (refs/remotes/origin/main)`
  - `Commit message: "Update README.md"`

## Maven Build Operations
- **[INFO] Scanning for projects...**
- **Project:** `org.example:SimpleToDoList`
- **Version:** `1.0-SNAPSHOT`
- **Packaging:** `jar`

### Maven Phases
1. **Clean**
   - `Deleting /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target`
2. **Resources**
   - `Copying resources (UTF-8 encoding)`
   - `Skipping non-existing resourceDirectory`
3. **Compile**
   - `Compiling 1 source file to /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target/classes`
4. **Test Resources**
   - `Skipping non-existing testResourceDirectory`
5. **Test Compile**
   - `No sources to compile`
6. **Test**
   - `No tests to run.`
7. **Jar**
   - `Building jar: /home/jenkinsuser/.jenkins/workspace/Build-And-Upload/target/SimpleToDoList-1.0-SNAPSHOT.jar`
8. **Install**
   - `Installing jar and pom to local repository`

## Build Summary
- **BUILD SUCCESS**
- **Total time:** `3.424 s`
- **Finished at:** `2024-01-19T14:59:41+03:00`

## Post-Build Actions
- **Archiving artifacts**
- **Triggering a new build of Deploy-With-Ansible**

**Finished: SUCCESS**
