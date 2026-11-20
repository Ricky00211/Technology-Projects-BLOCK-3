# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)

### Questions

1.  How many users exist on the system? Ans: 37 
2.  Which accounts appear to be system accounts? ans: Apart from the root and the 2 other users i.e (Automationaces and iotinvestigators) all the other accounts are system accounts.
3.  Why do operating systems create system accounts?ans: To protect the main user accounts such as root and the 2 other users . so when the attacker hacks into the account it can only access to some limited accounts of system accounts.


### Reflection

Explain why understanding system users is important for cybersecurity.
ANS: Understanding systme users is important for cybersecurit because knowing which accounts should be on the system helps me spot unexpected accounts and check who has access to sensitive files.
------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
Ans: all the processes with USER as root is being runned as root. 
2.  Why can processes running as root be dangerous?
ANs: Because the root has unrestricted access to the whole system so if the attacker exploits a vulnerability in a root process, they inherit that full control which means they can edit anything and even delete the account if they want to. so it can be dangerous to  run the process as a root. 
3.  What could happen if a malicious program ran with root privileges?
ANs: If a malicious program ran with root privilages then it can access all the files, passwords and everything that is in the computer. They can edit or delete anything they want with root privilages.

### Reflection

What did you learn about system processes and security?
I learned that system processes run under differernt account like root process which are privileged and can access, edit and delete any file, so if one is compromised an attacker gets full access to it. And apart from root process there are also services that run as unprivileged which limits the access to full control over files so it is less dangerous. 
------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)

### Questions

1.  Which ports are open?
ANS: all ports listed by ss -tuln. 
2.  Which services appear to be listening?
ANS: 
3.  Why might open ports represent a security risk?
ANS: An open port lets a service receive network traffic. If the service is reachable and has a vulneribility or weak authentication, someone could use it to gain unauthorized access.
### Reflection

Explain the relationship between open ports and potential attack
surfaces.
