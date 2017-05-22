# Architecture Diagrams for an Email Client 

### 1.Architecture for Managing an Email

The diagram below is a group of package of components. These are high level modules of the system.  The blue boxes represent the controllers for specific tasks, for example the move and delete email controllers, control the physical location of the email. The email selection system and email system are grouped together as they allow the user to select specific emails from the email system. The view and edit email system are grouped together, as they allow they user to open an email and modify the content of it. The arrows represent data flow, so in this diagram we start with the clients account, which has an inbox. The inbox then sends data to the three controllers, which allows the user to perform specific tasks. The move/delete email controller is linked with the email selection system, as the email needs to be selected in order for it to be move or deleted. The server controller is used to retrieve the email data. 
 
![Architecture for Managing an Email.jpg](Architecture for Managing an Email.jpg "Architecture for Managing an Email")   


### 2.Client Server Architecture 

This diagram shows the various protocols and servers that are needed in order to provide an email service, address book and directory service. The first outer blue box represents the email client system. The second inner blue box represents the connectors for the the email client. The reason for this is that it shows the interaction between the server, the connectors and the email client. The arrows represent the protocols that are used for transferring information from a server to the component. In addition to that some of the protocols used are new, as these protocols are more appropriate for describe the interactions between the server and the email client, than the protocols mentioned in the requirements specification.

     
**_Diagram 1_**

![Client Server Architecture.jpg](Client Server Architecture.jpg "Client Server Architecture") 

#### Protocol Definitions
- Messaging Application Programming Interface (MAPI)- This allows a client program to become email messaging enabled. 
- Internet Message Access Protocol (IMAP)- This is used to store email messages on a mail server. It also allows the end user to view and manipulate the messages. 
- Simple Mail Transfer Protocol (SMTP)- This is used for sending and receiving emails. 
- Representational State Transfer (REST)- This specifies constraints that allow the service to work best on the web. 
- Lightweight Directory Access Protocol (LDAP)- This runs above the TCP/IP protocol, as mentioned in functional requirements 3.2. This protocol allows users to connect, search and modify internet directories.  


**_Diagram 2_**


#### Definitions of Technical Terms
- Nullmailer is a mail queue in which emails are placed and sent from.  
- Procmail is a mial processing tools for Unix, which helps you to filter and sort email. 
- LMDA refers to Linux Mail Delivery Agent, which is simply responsible  for sending and receiving mail.
- ISP is the internet service provider.

The diagram below shows the process of a user sending an email to a recipient. As you can see it it divided up into four sectors, this is to show the process taking place at the senders computer and the senders ISP, as well as the recipients computer and recipients ISP. The arrows represent data flow, so the double headed arrow allows data to flow both ways, meanwhile the single headed arrow allows to flow one way.   
 
![Client Server Architecture2.jpg](Client Server Architecture2.jpg "Client Server Architecture2") 



### 3.Model View Controller (MVC) Architectural Pattern 

The diagram shows the authentication process, when a user logs into their account. This relate to functional requirements 2.9. The blue box in the scenario represents the email client system. First the users enters details and then clicks sign in, then the MVC controller sends the result to the middleware, which verifies the end-user. After this the data is relayed to the Account authentication server, where it verifies the account. It the sends a account validated token back to the controller, which as a result allows a successful login. The arrows in this case represent moving from one state to another, so at the start user clicks sign in and at the same time the authentication process begins. It also represents data flow from the MVC controller to the Account authentication server.      

![MVC Architectural Pattern.jpg](MVC Architectural Pattern.jpg "MVC Architectural Pattern")


### 4.Layered Architecture

The diagram below shows the different layers of the software. As you can see the web email client is at the top, underneath that is the authentication layer, which provides security for the users email account, which satisfies functional requirements 2.9 and 3.0. Underneath this layer is the functionality layer that provides the various features of the email client. The last layer at the bottom provides the email management system, support system and accounts database, which satisfy function requirements 2.8.

![Layered Architecture.jpg](Layered Architecture.jpg "Layered Architecture")



### 5.Class Diagram


The class diagram below shows the relationships between the different classes of the email client. The main class provides functionality that could be implemented in a graphical interface. The shaded diamond arrows represents a composition relationship, this means that a class " is a part" of another class. This shows a binary association, which in simple terms means that if the main class is deleted all of its connected classes will also be deleted. For example if main is deleted create email will also be deleted. The unshaded diamond arrow represents a aggregation relationship, this means that a class "has a" another class associated with it. In this diagram the folder class has several other classes, which are associated with it. This interaction between the folders class and its associated classes, could also be regarded as an inheritance relationship if all of its associated classes shared the same attribute as the folders class. In simple terms to make it an inheritance relationship I could add the delete operation to the folders class. This would have been represented with a solid line with a triangular arrow head. The dotted arrows shows a dependency, so for example in order for the user database class to work, the profile management class has to present.            

![Email Class.jpg](Email Class.jpg "Email Class")


### 6.Description of Classes

- **_Account Login_** - This class contains the login form, which has two  input boxes for the username and password. It has satisfied the functional requirements 2.9, as a secure method of logging in has been provided. 

- **_Main_** - This is the main class, which calls the other classes on compile time. It is essentially the user interface class. It has satisfied the non-functional requirements 1.1, as a user interface that is easy to use has been provided. 

- **_Profile Management_** - This class simple allows the user to edit or delete their profile. It has satisfied the non-functional requirements 6.1, as users are able to maintain and manage all emails. 


- **_TbProfile_** - This class contains all the relevant information regarding the users profile. It has satisfied the functional requirements 2.8, as a user account settings feature has been provided that allows the user to change profile information.  

- **_User Database_** - This class provides a secure connection to the database, where the user accounts are stored. 

- **_Inbox Management_** - This class allows the users to manage their emails that are located within the inbox.

- **_TbInbox_** - his class contains all the relevant information regarding the users inbox. 

- **_Create Email_** - This class simply contains the functions that allow the user to create a new email. It has satisfied the functional requirements 1.2, as  the user is able to create and send an email.
 
- **_Folders_** - The class contains all the other additional functionalities of the email client. It also allows the user to manage and organise any folders that they may have created. It has satisfied the functional requirements 1.9, as  the user is able to organise emails into folders. 

- **_Junk_** - This class simply contains junk email, where the user can perform an appropriate action. It has satisfied the functional requirements 1.7, as  the user is able to move emails into the junk email folder. 

- **_Drafts_** - This class simply contains drafts, where the user can perform an appropriate action.

- **_Sent Email_** - This class simply contains sent emails, where the user can perform an appropriate action. It has satisfied the functional requirements 1.2, as  the user is able to send an email.

- **_Deleted Email_** - This class simply contains deleted emails, where the user can perform an appropriate action. It has satisfied the functional requirements 1.2, as  the user is able to delete an email.
