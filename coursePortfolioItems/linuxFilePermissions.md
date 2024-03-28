**File permissions in Linux:**

**Project description**

We navigated to the directory, viewed all permissions as is, then adjusted permissions of files and directories. This is to show proficiency in managing Linux file permissions. 

**Check file and directory details**

Yes - we can see below the rw permissions for the user, group, and others. 
* `ls -l` to show permissions 
* `ls -la` to show permissions including hidden files/directories <br>

```
researcher2@2e0ed848a3b8:~/projects$ ls
drafts  project_k.txt  project_m.txt  project_r.txt  project_t.txt
researcher2@2e0ed848a3b8:~/projects$ ls -l
total 20
drwx--x--- 2 researcher2 research_team 4096 Mar 28 18:21 drafts
-rw-rw-rw- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
-rw-r----- 1 researcher2 research_team   46 Mar 28 18:21 project_m.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_r.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_t.txt
researcher2@2e0ed848a3b8:~/projects$ ls -a  
.  ..  .project_x.txt  drafts  project_k.txt  project_m.txt  project_r.txt  project_t.txt
researcher2@2e0ed848a3b8:~/projects$ ls -la 
total 32
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 18:21 .
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 19:22 ..
-rw--w---- 1 researcher2 research_team   46 Mar 28 18:21 .project_x.txt
drwx--x--- 2 researcher2 research_team 4096 Mar 28 18:21 drafts
-rw-rw-rw- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
-rw-r----- 1 researcher2 research_team   46 Mar 28 18:21 project_m.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_r.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_t.txt
```

**Describe the permissions string**

Permissions are user, group, and others. RWX for read, write, and execute (if `-` is showing, the permission is not provided for that user, group, or other). <br>

* `-rw-rw-rw- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt` <br>
   For example, the user, groups, and others here all have read and write permissions but not executable permission. 

**Change file permissions**

```
researcher2@2e0ed848a3b8:~/projects$ chmod o-w project_k.txt
researcher2@2e0ed848a3b8:~/projects$ chmod g-rw project_m.txt 
researcher2@2e0ed848a3b8:~/projects$ chmod gu-rw .project_x.txt 
researcher2@2e0ed848a3b8:~/projects$ ls -la
total 32
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 18:21 .
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 19:22 ..
---------- 1 researcher2 research_team   46 Mar 28 18:21 .project_x.txt
drwx--x--- 2 researcher2 research_team 4096 Mar 28 18:21 drafts
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
-rw------- 1 researcher2 research_team   46 Mar 28 18:21 project_m.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_r.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_t.txt
```

**Change directory permissions**

```
researcher2@2e0ed848a3b8:~/projects$ chmod g-x drafts/ 
``` 

**Summary**

The above commands show proficiency in handling Linux permissions on files, adding and removing execution, read, and write ability permissions to files and directories. This ability allows for adjusting permissions to ensure confidentiality and security as per requirements. 
