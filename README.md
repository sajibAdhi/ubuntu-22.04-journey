# ubuntu-22.04-journey
Day-to-day use of Ubuntu 22.04 Journey

## Date: 2023-05-23

### Font Issue:
- I want to change the font of my GUI and use the font that Windows 10 uses.
- I searched: “What font does Windows 10 use”

### Mysql Issue: 
- Starting the `MySql` server from `Xampp` but it just stops. 
- So I clicked the `configuration` button of `xampp` GUI. 
- Then clicked the `Open Log` button to open the log file.
- There I noticed some errors:  [ERROR] Do you already have another mysqld server running on port: 3306?
- So then I tried checking If there is any process that running with port: 3306.
- Open the terminal.
- Type the following command to check if MySQL service is running or not: sudo systemctl status mysql.
- If MySQL service is running then stop the service by running the command: sudo systemctl stop mysql.
- Check if MySQL service port 3306 is still in use or not by running the command: sudo netstat -apn | grep 3306.
- Then I start the MySQL server again and It's working fine.

