# Day 6

You should be able to log in to every app server without typing a password, as a normal user, and use sudo when you need admin access.

we need thor user to login to app1,2,3 as a sudo without password

>> ssh-keygen -t rsa
Make me a digital key so I can enter servers without a password

we create a key in my server then copy it to the 3 servers so i can sign in directly    without password


verify login 
ssh tony@stapp01


