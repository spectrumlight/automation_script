# automation_script.sh

This bash script monitors your processes on Linux systems. 
If a process isn't running, it automatically initiates it, making sure it's always up and running.
Otherwise it will output the message "Process $process_name is running."

Usage
1. Specify the name of your script. If it's a hidden script (e.g "/home/admin/.script) then add a period before its name
   Example: process_name=".script"
2. Specify the path where the script resides
3. Use "crontab -e" to schedule this automation script
   For example: * * * * * /home/admin/automation_script.sh
