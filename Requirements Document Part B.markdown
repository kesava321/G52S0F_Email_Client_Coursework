# Architecture Diagrams for an Email Client 

### 1.Architecture for Managing an Email

![Architecture for Managing an Email.jpg](Architecture for Managing an Email.jpg "Architecture for Managing an Email")   


### 2.Client Server Architecture 

**_Diagram 1_**

![Client Server Architecture.jpg](Client Server Architecture.jpg "Client Server Architecture") 


**_Diagram 2_**

![Client Server Architecture2.jpg](Client Server Architecture2.jpg "Client Server Architecture2") 

### 3.MVC Architectural Pattern 

![MVC Architectural Pattern.jpg](MVC Architectural Pattern.jpg "MVC Architectural Pattern")


### 4.Layered Architecture

![Layered Architecture.jpg](Layered Architecture.jpg "Layered Architecture")


### 5.Repository Architecture

![Repository Architecture.jpg](Repository Architecture.jpg "Repository Architecture")


### 6.Software Architecture

![Software Architecture.jpg](Software Architecture.jpg "Software Architecture")


### 7.Class Diagram

![Email Class.jpg](Email Class.jpg "Email Class")


### 8.Description of Classes

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
