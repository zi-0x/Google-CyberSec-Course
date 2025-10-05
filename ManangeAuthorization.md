Authorization is the concept of granting access to specific resources in a system. It's important because without authorization any user could access and modify all files belonging to other users or system files. This would certainly be a security risk.<br><br>

drwxrwxrwx: d for directory | "-" for a regular file<br>
u : indicates changes will be made to user permissions<br>
g : indicates changes will be made to group permissions<br>
o : indicates changes will be made to other permissions<br>
+ : adds permissions to the user, group, or other<br>
- : removes permissions from the user, group, or other<br>
= : assigns permissions for the user, group, or other<br><br>

Task 1. Check file and directory details<br>
1. List the contents and permissions of the directory.<br>
```ls -l```<br>
2. Check whether any hidden files exist in the directory.<br>
```ls -la```<br><br>

Task 2. Change file permissions<br>
1. Change the permissions of the file identified in the previous step so that the owner type of other doesn’t have write permissions.<br>
```chmod o-w project_k.txt```<br>
2. Use the chmod command to change permissions of the project_m.txt file so that the group does have read or write permissions.<br>
```chmod g+r project_m.txt```<br><br>

Task 3. Change file permissions on a hidden file<br>
```chmod u-w,g-w,g+r .project_x.txt```<br><br>

Task 4. Change directory permissions<br>
```chmod g-x drafts```