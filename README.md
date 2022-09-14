# Computer Networks

## About The Project
The goal of this project is to develop a simple networking application that allows users to backup the contents of a specified local directory using a cloud service. The cloud storage can be done incrementally, meaning that if some of the files in the directory have the same name, size and date, they don’t need to be copied.

It was developed one user application and two server applications:
* the user application (user)
* a Central Server (CS)
* a Backup Server (BS). 

The user application and the various servers are intended to operate on different machines connected to the Internet.
The operation is as follows. To perform any cloud backup operation the user first needs to authenticate itself. For
this, the user application establishes a TCP session with the CS, which has a wellknown URL, providing the user identity (the IST student number – a 5 digit number) and a password (composed of 8 alphanumerical characters, restricted to letters and numbers). The CS will confirm the authentication.

The user can then decide to perform one of the operations:
1. Register as a new user.
2. Request the backup of a selected local directory.
3. List the previously stored directories and files.
4. Retrieve a previously backed up directory.
5. Delete the backup for a selected directory.
6. Delete the registration as a user. 

## How to run

~~~~
$ ./CS.py [-p a_port]
$ ./BS.py [-n cs_ip_address] [-p cs_pors] [-b my_port]
$ ./user.py [-n cs_ip_address]
~~~~

## Contributors
This project was developed by Diogo Ramalho, Manel Manso and Rafael Pestana de Andrade.




