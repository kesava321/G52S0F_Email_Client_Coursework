#Requirements For Email Client

###1.Document Introduction  
```  
This document will cover the requirements of an email client system. It will cover user and system requirements as well as functional and non-functional requirements. In addition to that UML diagrams will be used to support the email client system. 

```  
###2.System	Overview

```  
The system will allow a user to access an email client through the web. This system will be suitable for a wide variety of people who use email, as a means of communication. It will mostly be used be adults who are in an educational establishment or by an average working person, who may use it in an office environment. The system itself will enable a user to securely login to the email client over the internet, were they will then be able to view, access and manage their emails. 
```


###3.Non-functional	requirements of	the	system
  
- **_Interface_** - The system should have an easy to use interface, that allows the user to easily perform any task they require.  
- **_Performance_** - Once an email is sent, it should arrive in the recipients mailbox within a few seconds. The email client must also be able to allocate the relevant memory, in order view big emails that contain a lot of data.
- **_Reliability_** - The email client should be able to send and receive emails without any errors or delays.
- **_Availability_** - The client can be accessed on any device with an internet connection. It is a web application so it should work on any operating system, such as Windows, Mac, Linux etc. 
- **_Security_** - The user account details and password should be encrypted and securely stored within the email client. 
- **_Maintainability_** - The email client should allow the user to maintain and manage all emails. Also the users profiles/account settings must be maintained, along with any software updates/security patches that may be released in the future. 
- **_Portability_** - The user should be able to access their email anywhere on any computer. 


 


###4.Functional requirements of	the	system

1. **_Main Features:_**
  * The user should be able to search/view emails, send emails, delete emails and forward emails.
  * Notifications can be provided, when new mail arrives. 
  * The user should be able to add contacts to their address book. 
  * Important emails can be flagged, so they appear at the top of the Inbox.
  * Junk mail that does not require an immediate action, will be stored in the junk folder.
  * Emails that may require attention at a later stage can be archived.
  * Emails can also be organised into folders.
  * When writing emails spell check should automatically recognise any incorrect spellings or grammatical errors. 
  * Users should be able to print emails.
  * An auto-response feature may be added, in the event the user is on a vacation and is unable to respond to an email. 
  * The email client should not interfere with any other programs that are running.    


2. **_Multimedia:_**
  * The user should be able to attach a file to an email, by using the drag and drop interface or by manually selecting the file in the directory in which it is stored. 
  * The user be able to send and receive images, videos , music or any other multimedia files.  


3. **_Security:_**
  * Additional security features are provided, such as being able to mark suspicious emails as spam or being able to an unverified block a sender. 
  * The email client should also allow the secure transfer of any media files.
  * User can change their password or account settings.
  * Allow the user to securely log out of the email client.
  * Outgoing mail should be authenticated, so that the sender'd identity cannot be falsified. 


4. **_Protocol:_**
  * IMAP protocol may be used for downloading messages from your Inbox to your local computer. The advantage of using IMAP over POP is that it allows the users to view the email client on a multitude of devices, such as their laptop, phone or tablet. 
  * TCP/IP protocol can be used to manage requests by the client over a network. 





###5.Formal	description	of the system behaviour
```  
Firstly the user accesses the email client though the web. The user will then be required to enter  the login details, in order to gain secure access to their email. The system responds appropriately, by either accepting or rejecting the login details. If successful the user will be directed to the main page, which is their Inbox. The user can now do various tasks, such as view an email or write a new email. Once the email is sent the system will send it to the server and then relay it to the receiving client, where the email can then be viewed.    
```




###6.Examples of system	usage
```  
 
 
 

```