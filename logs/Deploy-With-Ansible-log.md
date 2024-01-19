Started by upstream project "Build-And-Upload" build number 4
originally caused by:
 Started by upstream project "JavaAppCI" build number 6
 originally caused by:
  Started by user admin
Started by upstream project "JavaAppCI" build number 6
originally caused by:
 Started by user admin
Running as SYSTEM
Building in workspace /home/jenkinsuser/.jenkins/workspace/Deploy-With-Ansible
[Deploy-With-Ansible] $ /bin/sh -xe /tmp/jenkins16768368287599997222.sh
+ ansible-playbook /etc/ansible/playbooks/playbook.yml
[WARNING]: No inventory was parsed, only implicit localhost is available
[WARNING]: provided hosts list is empty, only localhost is available. Note that
the implicit localhost does not match 'all'

PLAY [Deploy SimpleToDoList application] ***************************************

TASK [Gathering Facts] *********************************************************
ok: [localhost]

TASK [Copy SimpleToDoList artifact to Tomcat webapps directory] ****************
changed: [localhost]

TASK [Output copy result] ******************************************************
ok: [localhost] => {
    "copy_result": {
        "changed": true,
        "checksum": "7a1d631c51de9733d91892f44bb79277b86c2a55",
        "dest": "/var/lib/tomcat9/webapps/SimpleToDoList-1.0-SNAPSHOT.jar",
        "diff": [],
        "failed": false,
        "gid": 1002,
        "group": "jenkinsuser",
        "md5sum": "96aa3858693c4e49dd9fabd75482ec4b",
        "mode": "0644",
        "owner": "jenkinsuser",
        "size": 2461,
        "src": "/home/jenkinsuser/.ansible/tmp/ansible-tmp-1705665592.095874-2291-64324059918499/source",
        "state": "file",
        "uid": 1001
    }
}

TASK [Restart Tomcat] **********************************************************
changed: [localhost]

PLAY RECAP *********************************************************************
localhost                  : ok=4    changed=2    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

Finished: SUCCESS
