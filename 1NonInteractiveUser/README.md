# **Day 1**
Create non interactive user to prevernt access control
1- ssh the server 
2- create a user in nologin folder using 
    sudo useradd -s /sbin/nologin siva
3- list all users just to validation

# **Create Expiry User**

Create expiry user using cmd
>sudo useradd -e 2027-03-28 rose

## more explanation
first we will check if the user existed or not 
```
cat /etc/passwd | grep mennauser 
```

create a non interactive user
```
sudo useradd rose --shell /sbin/nologin 
```
