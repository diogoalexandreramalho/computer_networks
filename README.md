# Computer Networks

## How to run

~~~~
$ ./CS.py [-p a_port]
$ ./BS.py [-n cs_ip_address] [-p cs_pors] [-b my_port]
$ ./user.py [-n cs_ip_address]
~~~~


2. Q: What are these .pickle files?

A: These .pickle files are information kept by the CS and the BS. If you do not
want to use this info in the next invocation of the CS or the BS, just remove
those files. To remove them, you can use the command:

~~~~
$ make clean
~~~~

You will also have to remove any folders uploaded by users. Those folders are
tipically named as a 5 digit number, and have subdirectories.


3. Q: The CS/BS is using information from the previous execution. How do I stop
them from doing so?

A: Vide (2).




