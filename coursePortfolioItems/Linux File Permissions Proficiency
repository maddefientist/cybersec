<h1>File permissions in Linux:</h1>

<h2>Project description</h2>

We navigated to the directory, viewed all permissions as is, then adjusted permissions of files and directory. This is to show proficiency in managing linux file permissions. 

<h2>Check file and directory details</h2>

Yes - we can see below the rw permissions for user, group and others. 
Ls -l and ls -la to show permissions and permissions including hidden files/directories respectively. 
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
researcher2@2e0ed848a3b8:~/projects$ ls -la -a
total 32
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 18:21 .
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 19:22 ..
-rw--w---- 1 researcher2 research_team   46 Mar 28 18:21 .project_x.txt
drwx--x--- 2 researcher2 research_team 4096 Mar 28 18:21 drafts
-rw-rw-rw- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
-rw-r----- 1 researcher2 research_team   46 Mar 28 18:21 project_m.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_r.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_t.txt

<h2>Describe the permissions string</h2>
Permissions are user, group and others. RWX for read, write and execute (if - is showing, the perimssions is not provided for that user,group or other)
-rw-rw-rw- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
For example , the user, groups and others here all have read and write permissions but not executable permission. 
<h2>Change file permissions</h2>
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

<h2>Change file permissions on a hidden file</h2>
researcher2@2e0ed848a3b8:~/projects$ chmod gu-rw .project_x.txt 
researcher2@2e0ed848a3b8:~/projects$ chmod gu+r .project_x.txt 
researcher2@2e0ed848a3b8:~/projects$ ls -la
total 32
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 18:21 .
drwxr-xr-x 3 researcher2 research_team 4096 Mar 28 19:22 ..
-r--r----- 1 researcher2 research_team   46 Mar 28 18:21 .project_x.txt
drwx--x--- 2 researcher2 research_team 4096 Mar 28 18:21 drafts
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_k.txt
-rw------- 1 researcher2 research_team   46 Mar 28 18:21 project_m.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_r.txt
-rw-rw-r-- 1 researcher2 research_team   46 Mar 28 18:21 project_t.txt

<h2>Change directory permissions</h2>
researcher2@2e0ed848a3b8:~/projects$ chmod g-x drafts/

<h2>Summary</h2>
The above commands show proficiency in handling linux permissions on files, adding and removing execution, read and write ability permissions to files and directories. <br>This ability allows for adjusting permissions to ensure confidentiality and security as per requirements 

