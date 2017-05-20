# Requirements For Email Client

### 1.Document Introduction  
This document will cover the requirements of an email client system. It will cover user and system requirements, as well as functional and non-functional requirements. In addition to that UML diagrams will be used to support the email client system. 


### 2.System Overview
The system will allow a user to access an email client through the web. This system will be suitable for a wide variety of people who use email, as a means of communication. It will mostly be used be adults who are in an educational establishment or by an average working person, who may use it in an office environment. The system itself will enable a user to securely login to the email client over the internet, were they will then be able to view, access and manage their emails. 

##### System Context Diagram
The system context diagram below shows the different systems that the email client interacts with in order to work. 
 
 ![Email System Context.jpg](Email System Context.jpg "System Context")
 

The email client that I will design, relates to my understanding of how a no-digital domestic mail service works. In this case the mail arrives somewhere near your front door, similarly in the email client email arrives either in the inbox or junk mail folder. Then the mail gets collected, similarly in the email client new mail is marked as unread, in order to notify the user that it has just arrived. After that mail gets placed in an appropriate location that reflects its action status, for example important mail is placed where it can be noticed very easily ,whilst junk mail might be put in a low priority area, such as a notice board. Similarly in the email client emails that are not from a verified sender or regarded as spam get moved to the junk mail, whilst important emails are kept in the inbox. Emails that might need further action taken at a later point can be flagged by the user, so that they can easily refer to it at a  later stage, which is similar to placing mail on a notice board. If unimportant promotional mail is received then it can be binned, similarly if junk email is received then it can be deleted.          


### 3.User Requirements

1. Users should be able to securely access their emails. 
2. Users should be able to send and receive emails.
3. Users should be able to include file attachments in their emails. 
4. Users should be able to forward an email to multiple peoples. 
5. Users should be able to organise emails into folders. 
6. Users should be able to delete emails.
7. Users should be able to change account settings. 

##### User Stories
The user stories diagram below shows the users ability to attach files to an email.

 ![Email Use Stories.jpg](Email User Stories.jpg "User Stories ")


### 4.Non-functional requirements of the system

  
1. **_Interface_** 

    1.1 The system should have an easy to use interface, that allows the user to easily perform any task they require.
   
    1.2 The colour scheme of the email client should be neutral and should not be too  bright, so that all users can easily see the different features. 
    
2. **_Performance_** 
    
    2.1 Once an email is sent, it should arrive in the recipients mailbox within a few seconds. The email client must also be able to allocate the relevant memory, in order view big emails that contain a lot of data.
    
3.  **_Reliability_** 
    
    3.1 The email client should be able to send and receive emails without any errors or delays.
    
    3.2 The email client should allow the user to send email to multiple recipients, without any error or delays. 
    
    3.3 The email client should work as normal at any time of the day. 
    
4.  **_Availability_**
    
    4.1 The client can be accessed on any device with an internet connection. It is a web application so it should work on any operating system, such as Windows, Mac, Linux etc. 
    
5.  **_Security_**
    
    5.1 The user account details and password should be encrypted and securely stored within the email client.
    
    5.2 The email client should warn the user, if they attempt to open a malicious file within an email.  
    
    
6.  **_Maintainability_**
   
     6.1 The email client should allow the user to maintain and manage all emails.
     
     6.2 The users profiles/account settings must be maintained, along with any software updates/security patches that may be released in the future. 


 


### 5.Functional requirements of the system


| ID    | Title               | Description           | Rational               |
| :---- | :------------------ | :-------------------- | :--------------------- |
| 1.1   | Search/view emails  | The user should be able to search or view emails. | This allows the user to easily filter out a specific email from a long list of unsorted emails.      |
| 1.2   | Send/delete emails  | The user should be able to send/delete emails.                     | This is a simple functionality that is necessary in order for the email client to work as intended.          |
| 1.3   | Forward emails      | The user is able to forward emails to other people. | This reason for this requirement is that users may want to share the contents of the email they received with another user.|
| 1.4   | Notifications       | The user should be notified when a new email arrives.                      | This is similar to placing a non-digital mail in a place that someone can easily identify it. In this case a notification is used to get the users attention.   |   
| 1.5   | Contacts            | The user should be able to add contacts to their address book.                 | The reason for this requirement is that it ensure that mail gets sent to the inbox by users in their contact list, rather than it being sent to the junk mail.                  |
| 1.6   | Flagged emails      | The user should be able to flag emails, so they appear at the top of the list.                        | This is similar to placing a non-digital mail on a notice board that requires attention at a later date. Flagging an email has the same purpose.         |
| 1.7   | Junk emails         | Junk mail that does not require an immediate action, will be stored in the junk folder.            | This is similar to non-digital mail that does not require any action, for example promotional mail being thrown away. In this case junk email has a similar purpose, as emails that are unimportant and do not require an immediate action are stored here.        |
| 1.8   | Archived emails     | Emails that may require attention at a later stage should be archived.     | This allows email to be stored that may be required in the future. This is similar to flagging an email, however when archiving emails they can be stored for a longer time and are only reopened when needed.                       |
| 1.9   | Folders             | The email client should allow users to organise emails into folders.          | This is similar to sorting non-digital mails into importance and priority. However in this case email is sorted into any category the user chooses, for example the user may want a sports folder, to store email regarding sports and a shopping folder, to store emails form e-commerce sites, such as Amazon or Ebay.               |
| 2.0   | Spell/grammar check | When writing emails spell check should automatically recognise any incorrect spellings or grammatical errors.         |                        The reason for this requirement is to simply ensures there are no errors in the email the user is sending.    | 
| 2.1   | Print emails        | Users should be able to print emails.          |                        The reason for this requirement is that the user may want to print out something important, so that they have a physical copy, for example they may want to print out an invoice or a household bills statement.        |
| 2.2   | Auto-response       |  An auto-response feature may be added, in the event the user is on a vacation and is unable to respond to an email.          |                        This allows users to not constantly have the need of responding to emails, if they are busy with something else or simply not available.                     |
| 2.3   | Interference        | The email client should not interfere with any other programs that are running.                      | This ensures that the email client functional normally without causing disruption to other applications that are also being used by the user.    |
| 2.4   | File attachments    | The user should be able to attach a file to an email, by using the drag and drop interface or by manually selecting the file in the directory in which it is stored.                  | The user may want to send files another user, therefore this feature is necessary.                  |
| 2.5   | Multimedia          | The user be able to send and receive images, videos, music or any other multimedia files.          | The user may want to share media with another user, therefore this feature is necessary.            |
| 2.6   | Spam emails         | Additional security features should be provided, such as being able to mark suspicious emails as spam or being able to an unverified block a sender.    | This ensures that the security of emails are maintained.                   |
| 2.7   | Secure file transfer| The email client should also allow the secure transfer of any media files.  | This ensures that files that are sent within an email securely arrive in the recipients email box, without being tampered with.|
| 2.8   | Account settings    | User should be able to set their password or account settings.             | This is necessary as users may want to change their passwords every now and then, they may also want to change they're account settings.                     |
| 2.9   | Log in/out          | Allow the user to securely log in/out of the email client.                 | This ensures that other people can not access the users email account, therefore this is necessary.                          |
| 3.0   | Email authentication| Outgoing mail should be authenticated, so that the sender's identity cannot be falsified.             | This ensures the email being sent by the user is verified and safely arrives in the recipients inbox. |
| 3.1   | IMAP protocol       | IMAP protocol may be used for downloading messages from your inbox to your local computer.       |                        The advantage of using IMAP over POP is that it allows the users to view the email client on a multitude of devices, such as their laptop, phone or tablet. |
| 3.2   | TCP/IP protocol     | TCP/IP protocol can be used to manage requests by the client over a network. | This ensures user can communicate with each other over the internet, therefore this is necessary.  |



### 6.Formal description of the system behaviour


Firstly the user accesses the email client though the web. The user will then be required to enter  the login details, in order to gain secure access to their email. The system responds appropriately, by either accepting or rejecting the login details. If successful the user will be directed to the main page, which is their Inbox. The user can now do various tasks, such as view an email or write a new email. Once the email is sent the system will send it to the server and then relay it to the receiving client, where the email can then be viewed.    


##### Use Case
The use case diagram below shows that the user and administrator can manage the email account. It also shows how a user can download media files and send or view their emails. 
 ![Email Use Case.jpg](Email Use Case.jpg "Use Case ")
 


##### Activity 
The activity diagram below shows the login process of the email client. 

 ![Email Activity.jpg](Email Activity.jpg "Activity")
 
 
##### Sequence  
 
The sequence diagram below shows the various features that the email client has, this includes marking an email as junk, flagging an email, reporting a scam, pinning an email, adding contacts and organising emails into a folder.  

![Email Sequence.jpg](Email Sequence.jpg "Sequence")

The sequence diagram below shows the process of logging in, then sending and receiving emails with file attachments.  

![Email Sequence Adv.jpg](Email Sequence Adv.jpg "Sequence Adv")



### 7.Examples of system usage

##### Scenario 1 
Manager sends work email with meeting invitation to employee, expecting an email response.  

![Example Systems Usage 1.jpg](Example Systems Usage 1.jpg "Example Systems Usage 1")

##### Scenario 2
Mum needs to send proof of address documents to school in order to register her child. 

![Example Systems Usage 2.jpg](Example Systems Usage 2.jpg "Example Systems Usage 2")