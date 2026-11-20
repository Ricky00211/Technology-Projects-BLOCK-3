# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who owns the file?
ANS: iotinvestigators.
2.  What are the default permissions?
ANS: read and write by the owner and the group while users can only read.

### Reflection

Why is file ownership important in Linux systems?
: because Linux uses file ownership and permissions to control who can read or modify a file. this helps to protect private files from unauthorized acess.
------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can read the file now?
The owner, iotinvestigators 
2.  Who cannot access it?


------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can access the file now?
2.  Why might this configuration be dangerous?

