Using the root (super) user gives full control to manage authorization and authentication, but it’s risky because it can cause irreversible mistakes, hide who ran commands, and be exploited if compromised. Instead of logging in as root, it’s safer to use sudo to run specific commands with elevated privileges when needed.<br><br>

The sudo command temporarily grants elevated permissions to specific users. The name of this command comes from “super user do.”<br><br>

Task 1. Add a new user<br>
1. Write a command to add a user called researcher9 to the system.<br>
```sudo useradd researcher9```<br>
2. Use the usermod command and -g option to add researcher9 to the research_team group as their primary group.<br>
```sudo usermod -g research_team researcher9``` || ```sudo useradd researcher9 -g research_team```<br><br>

Task 2. Assign file ownership<br>
1. Use the chown command to make researcher9 the owner of /home/researcher2/projects/project_r.txt.<br>
```sudo chown researcher9 /home/researcher2/projects/project_r.txt```<br><br>

Task 3. Add the user to a secondary group<br>
1. Use the usermod command with the -a and -G options to add researcher9 to the sales_team group as a secondary group.<br>
```sudo usermod -a -G sales_team researcher9```<br><br>

Task 4. Delete a user<br>
1. Run a command to delete researcher9 from the system:<br>
```sudo userdel researcher9```<br>
2. Run the following command to delete the researcher9 group that is no longer required:<br>
```sudo groupdel researcher9```