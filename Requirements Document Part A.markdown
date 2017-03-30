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
  
- Interface- The system should have an easy to use interface, that allows the user to easily perform any task they require.  
- Performance - Once an email is sent, it should arrive in the recipients mailbox within a few seconds. The email client must also be able to allocate the relevant memory, in order view big emails that contain a lot of data.
- Reliability - The email client should be able to send and receive emails without any errors or delays.

```diff
-remove between about platform independent.
```

-Availability - The client must be platform independent, i.e. it should work on windows, mac, line or any other operating system. 
- Security - The user account details and password should be encrypted and securely stored within the email client. 
- Maintainability- The email client should allow the user to maintain and manage all emails. Also the users profiles/account settings must be maintained, along with any software updates/security patches that may be released in the future. 
- Portability - The user should be able to access their email anywhere on any computer. 


 


###4.Functional requirements of	the	system
- Once logged in they can view any email they have received, send emails, delete      
  emails, forward emails and perform any other tasks usually found in any email client.  
- Additional security features are provided, such as being able to mark suspicious emails as spam or being able to an unverified block a sender. 
- The email client should also allow the secure transfer of any media files.
- The user must be able to add contacts to their address book. 
- Important emails can be flagged, so they appear at the top of the Inbox.
- Junk mail that does not require an immediate action, will be stored in the junk folder.
- Emails that may require attention at a later stage can be archived.
- Emails can also be organised into folders.
- When writing emails spell check should automatically recognise any incorrect spellings or grammatical errors. 
- The user must be able to attach a file to an email, by using the drag and drop interface or by manually selecting the file in the directory in which it is stored. 
- Users must be able to print emails.
- An auto-response feature may be added, in the event the user is on a vacation and is unable to respond to an email. 
- The user must be able to view emails, send emails, delete emails and forward emails.
- 
```diff
+describe pop protocol and then use tcp/ip 
-not necessary to focus on server side, i.e. mail delivery failures. 
```
- Use standard TCP/IP protocol to manage network of the email client. 
- Notifications can be provided, when new mail arrives. 
- The email client should not interfere with any other programs that are running. 
- Outgoing mail should be authenticated, so that the sender'd identity cannot be falsified. 
- Users should be able to search and view stored emails. 
- User can change their password or account settings.
- If email is unable to be sent, due to technical errors, then a delivery failure email should be sent to the sender. 
- Once the user has finished using the email client, they can then securely log out. 


###5.Formal	description	of the system behaviour
```  
 
 
 

```
###6.Examples of system	usage
```  
 
 
 

```