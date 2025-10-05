<b>Scenario:</b><br>
In this scenario, you need to obtain information contained in server log and user data files. You also need to find files with specific names.<br><br>

Task 1. Search for error messages in a log file<br>
1. Use grep to filter the server_logs.txt file, and return all lines containing the text string error.<br>
```grep error server_logs.txt```<br><br>

Task 2. Find files containing specific strings<br>
1. Using the pipe character (|), pipe the output of the ls command to the grep command to list only the files containing the string Q1 in their names.<br>
```ls | grep Q1```<br><br>
