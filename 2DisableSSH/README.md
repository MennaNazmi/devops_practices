# Day 2
Disable SSH root to prevent Brute-Force Attacks : like a robot trying every possible combination to guess your password.

#### Following security audits, the xFusionCorp Industries security team has rolled out new protocols, including the restriction of direct root SSH login. Your task is to disable direct SSH root login on all app servers within the Stratos Datacenter. ####


- vi is case sensetive 
- search on vi using /word

# SOLUTION #

1 - login to the server itself using SSH 
2- get into --> sudo vi /etc/ssh/sshd_config
3- change PermitRootLogin yes to no
4- sudo systemctl restart sshd

to check using cmd 
```
sudo cat /etc/ssh/sshd_config | grep -i "permitrootlogin"
```