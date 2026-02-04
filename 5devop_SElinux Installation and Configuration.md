# DAY 5

ssh steve@172.16.238.11  
Am3ric@

SELinux (Security-Enhanced Linux) is a security module built into the Linux kernel that enforces Mandatory Access Control (MAC).
Instead of relying only on standard Linux permissions (owner, group, others), SELinux uses policies to decide which processes can access which files, sockets, and other system resourceseven if standard permissions would normally allow it.


Install the required SELinux packages. >> sudo yum install selinux-policy selinux-policy-targeted policycoreutils

Permanently disable SELinux for the time being; it will be re-enabled after necessary configuration changes