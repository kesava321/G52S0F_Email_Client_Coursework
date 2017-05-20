# Architecture Diagrams for an Email Client 

### 1.Architecture for Managing an Email

The diagram below is a group of package of components. These are high level modules of the system.  The blue boxes represent the controllers for specific tasks, for example the move and delete email controllers, control the physical location of the email. The email selection system and email system are grouped together as they allow the user to select specific emails from the email system. The view and edit email system are grouped together, as they allow they user to open an email and modify the content of it. The arrows represent data flow, so in this diagram we start with the clients account, which has an inbox. The inbox then sends data to the three controllers, which allows the user to perform specific tasks. The move/delete email controller is linked with the email selection system, as the email needs to be selected in order for it to be move or deleted. The server controller is used to retrieve the email data. 
 
![Architecture for Managing an Email.jpg](Architecture for Managing an Email.jpg "Architecture for Managing an Email")   


### 2.Client Server Architecture 

This diagram shows the various protocols and servers that are needed in order to provide an email service, address book and directory service. The first outer blue box represents the email client system. The second inner blue box represents the connectors for the the email client. The reason for this is that it shows the interaction between the server, the connectors and the email client. The arrows represent the protocols that are used for transferring information from a server to the component. In addition to that some of the protocols used are new, as these protocols are more appropriate for describe the interactions between the server and the email client, than the protocols mentioned in the requirements specification.

     
**_Diagram 1_**

![Client Server Architecture.jpg](Client Server Architecture.jpg "Client Server Architecture") 

#### Protocol Definitions

- Internet Message Access Protocol(IMAP)- This is used to store email messages on a mail server. It also allows the end user to view and manipulate the messages. 
- Simple Mail Transfer Protocol (SMTP)- This is used for sending and receiving emails. 
- Representational State Transfer (REST)- This specifies constraints that allow the service to work best on the web. 
- Lightweight Directory Access Protocol (LDAP)- This runs above the TCP/IP protocol, as mentioned in functional requirements 3.2. This protocol allows users to connect, search and modify internet directories.  


**_Diagram 2_**


#### Definitions of Technical Terms
- Nullmailer is a mail queue in which emails are placed and sent from.  
- Procmail is a mial processing tools for Unix, which helps you to filter and sort email. 
- LMDA refers to Linux Mail Delivery Agent, which is simply responsible  for sending and receiving mail.
- ISP is the internet service provider.

The diagram below shows the process of a user sending an email to a recipient. As you can see it it divided up into four sectors, this is to show the process taking place at the senders computer and the senders ISP, as well as the recipients computer and recipients ISP. 
 
![Client Server Architecture2.jpg](Client Server Architecture2.jpg "Client Server Architecture2") 



### 3.MVC Architectural Pattern 
```diff
-Explain what openID connect middleware is
-Either change specification or change diagram to reflect requirements. 
-Justify diagrams.
-explain acronyms and describe diagrams.  
```
![MVC Architectural Pattern.jpg](MVC Architectural Pattern.jpg "MVC Architectural Pattern")


### 4.Layered Architecture
```diff
-Justify diagrams.
-explain acronyms and describe diagrams.  
```
![Layered Architecture.jpg](Layered Architecture.jpg "Layered Architecture")


### 5.Software Architecture
```diff
-Justify diagrams.
-explain acronyms and describe diagrams.  
```
![Software Architecture.jpg](Software Architecture.jpg "Software Architecture")


### 6.Class Diagram

```diff
-Two type of relationship aggregation and inheritance 
-change functions to folders
-add inheritance relationship for folders 
-aggregation between main class and main menu would be appropriate.
-profile manager is aggregation. 
-main class provides functionality that could be implemented in a graphical interface. 
```


![Email Class.jpg](Email Class.jpg "Email Class")


### 7.Description of Classes

```diff
-In explanation relate back to requirements.  
-allows users to manage their mail within the inbox.
-this class provides these functionalities, which have satisfied these requirements. 
```
- **_Account Login_** - This class simply contains the login form, which has two  input boxes for the username and password. 

- **_Main_** - This is the main class, which calls the other classes on compile time. It is essentially the user interface class. 

- **_Profile Management_** - This class simple allows the user to edit or delete their profile.

- **_TbProfile_** - This class contains all the relevant information regarding the users profile. 

- **_User Database_** - This class provides a secure connection to the database, where the user accounts are stored. 

- **_Inbox Management_** - This class allows the users to manage their emails that are located within the inbox.

- **_TbInbox_** - his class contains all the relevant information regarding the users inbox. 

- **_Create Email_** - This class simply contains the functions that allow the user to create a new email. 

- **_Functions_** - The class contains all the other additional functionalities of the email client.

- **_Junk_** - This class simply contains junk email, where the user can perform an appropriate action.

- **_Drafts_** - This class simply contains drafts, where the user can perform an appropriate action.

- **_Sent Email_** - This class simply contains sent emails, where the user can perform an appropriate action.

- **_Deleted Email_** - This class simply contains deleted emails, where the user can perform an appropriate action.

- **_Manage Folders_** - This class allows the user to manage and organise any folders that they may have created.
