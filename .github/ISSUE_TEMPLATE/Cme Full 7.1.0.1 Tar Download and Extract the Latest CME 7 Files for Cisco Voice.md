
 
# How to Install CME Full 7.1.0.1 Tar File on Your Cisco Router
 
CME Full 7.1.0.1 Tar is a file that contains the Cisco Unified Communications Manager Express (CME) software and phone firmware files for version 7.1. This file can be downloaded from the [Cisco Software Download site](https://www.cisco.com/cgi-bin/tablebuild.pl/ip-iostsp) and extracted directly on to your router's flash memory using the CLI interface.
 
**Download Zip … [https://t.co/uXpzWnqngo](https://t.co/uXpzWnqngo)**


 
In this article, we will show you how to install CME Full 7.1.0.1 Tar file on your Cisco router and configure it to support various IP phone models.
 
## Step 1: Download and Extract CME Full 7.1.0.1 Tar File
 
To download CME Full 7.1.0.1 Tar file, you need to have a valid Cisco account and access to the Cisco Software Download site. Once you have logged in, go to the [IP Telephony - IOS Telephony Services - Unified Communications Manager Express](https://www.cisco.com/cgi-bin/tablebuild.pl/ip-iostsp) section and select the file **cme-full-7.1.0.1.tar**. Save it to your local computer or a TFTP server that is accessible by your router.
 
To extract CME Full 7.1.0.1 Tar file on your router's flash memory, you need to have enough free space available. The file size is about 40 MB and it contains 132 files, including the basic CME GUI files and phone firmware files for various models[^2^]. You can use the **show flash:** command to check the available space on your flash memory.
 
If you have enough space, you can use the following command to extract CME Full 7.1.0.1 Tar file from a TFTP server to your flash memory[^1^]:

    R1# archive tar /xtract tftp://10.0.0.10/cme-full-7.1.0.1.tar flash:
    Loading cme-full-7.1.0.1.tar from 10.0.0.10 (via FastEthernet0/0): !
    extracting APPS-1.2.1.SBN (2593969 bytes)!!!!!!!!!!
    extracting apps11.8-4-1-23.sbn (2925555 bytes)!!!!!!!!!!!
    ...
    extracting xmldefault.cnf.xml (131 bytes)
    extracting xmlDefault7975.cnf.xml (131 bytes)
    extracting xmlDefault7975G.cnf.xml (131 bytes)

The **archive tar /xtract** command tells the router to load the .tar file from the TFTP server and extract it directly on to the router's flash memory.
 
## Step 2: Enable HTTP Server and Authentication
 
To access the CME GUI interface, you need to enable the HTTP server on your router and configure the authentication method to use the local user accounts on your router[^2^]. You also need to create a local user account with privilege level 15 and lower the file privilege level required for file operations[^2^]. The following commands show an example of how to do this:
 
Cme Full 7.1.0.1 Tar download,  Cme Full 7.1.0.1 Tar installation guide,  Cme Full 7.1.0.1 Tar features and benefits,  Cme Full 7.1.0.1 Tar compatibility and requirements,  Cme Full 7.1.0.1 Tar troubleshooting and support,  Cme Full 7.1.0.1 Tar review and feedback,  Cme Full 7.1.0.1 Tar license and pricing,  Cme Full 7.1.0.1 Tar upgrade and update,  Cme Full 7.1.0.1 Tar alternatives and comparisons,  Cme Full 7.1.0.1 Tar demo and trial,  Cme Full 7.1.0.1 Tar documentation and tutorial,  Cme Full 7.1.0.1 Tar security and privacy,  Cme Full 7.1.0.1 Tar backup and restore,  Cme Full 7.1.0.1 Tar customization and configuration,  Cme Full 7.1.0.1 Tar integration and automation,  Cme Full 7.1.0.1 Tar best practices and tips,  Cme Full 7.1.0.1 Tar FAQ and Q&A,  Cme Full 7.1.0.1 Tar forum and community,  Cme Full 7.1.0.1 Tar webinar and training,  Cme Full 7.1.0.1 Tar case study and success story,  Cme Full 7.1.0.1 Tar video and podcast,  Cme Full 7.1.0.1 Tar blog and newsletter,  Cme Full 7.1.0.1 Tar ebook and whitepaper,  Cme Full 7.1.0.1 Tar infographic and presentation,  Cme Full 7

    R1(config)# ip http server
    R1(config)# ip http authentication local
    R1(config)# username admin privilege 15 secret cisco
    R1(config)# file privilege 0

The **ip http server** command enables the HTTP server on your router.
 
The **ip http authentication local** command configures the router to use its local user accounts for HTTP authentication.
 
The **username admin privilege 15 secret cisco** command creates a local user account named admin with privilege level 15 and password cisco.
 
The **file privilege 0** command lowers the file privilege level required for file operations to 0, which is necessary to avoid errors when accessing the CME GUI interface[^2^].
 
## Step 8cf37b1e13


