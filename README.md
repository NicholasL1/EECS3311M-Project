# SamePage
Software Design Project

# ABOUT THIS PROJECT:

Same Page (SP) will be used to seek and maintain a community-based library of books that are personalized for each member.
Like a digital library, readers can search for, be recommended and learn more about their favorite books as well as view
the latest releases. Extra features that allow the reader's data to be stored will be available for those readers
registered as members with Same Page including writing book reviews, joining the same book clubs as other interested readers and tracking
reading progress.  

For the foreseeable future, the system is envisioned as a desktop application, however, it will be extensible so that
future releases can have a web and mobile interface.

# HOW IT WAS BUILT:

The functionality of the application is programmed entirely on java, and the GUI was created by using Java Swing
components. In the future iterations, a database will be added to store the book information and user profiles,
allowing SamePage to login and register users. This application follows SOLID principles, and utilizes the MVP design
architecture.

###### Landing Page
<img width="1436" alt="image" src="https://user-images.githubusercontent.com/77363160/224367792-0f39a261-1921-4d84-bbe7-a5871604678e.png">

###### Login Page
<img width="1436" alt="image" src="https://user-images.githubusercontent.com/77363160/224368285-1612bcc9-177a-4496-95f6-d102422d1e31.png">

###### Register Page
<img width="1437" alt="image" src="https://user-images.githubusercontent.com/77363160/224368361-79183cfc-e3e2-461d-b849-d8e1c8a18fb6.png">

###### Profile Page
<img width="1436" alt="image" src="https://user-images.githubusercontent.com/77363160/224367905-6b4c1518-5878-4d2f-bd82-0720b16d0f0d.png">

###### Book Information
<img width="1247" alt="image" src="https://user-images.githubusercontent.com/77363160/224368622-9e2edd3e-fa96-45fb-a081-5a4f8984d645.png">

# BUILD LOCALLY
To build this project locally, you will need access to the database credentials. Make sure to have MySQL downloaded and its 
required drivers to run the application. This <a href="https://www.youtube.com/watch?v=8aTpDfsYTNQ&ab_channel=ComputerClicks">video tutorial</a> can help with the download process. Save your MySQL password 
and username in a secure location. Once you have MySQL downloaded
- Go to ***SamePage/src/main/resources/config.properties***
- Replace the username and password fields with your username and password
  - ```shell
      db.driver=${db.driver}
      db.url=${db.url}
      db.username=${username}
      db.password=${password}
      ```
- Go to ***SamePage/src/main/java/com/eecs3311***
- There will be 4 Packages and one Java File called ***App.java***
- Click on the App.java file and run the application from there







# Stub Data
If you want to run the application with stub data only, refer to src/main/java/com/eecs3311/persistence/Database.java and turn the stub data flag on: 
```shell
private static boolean isUsingStubDB = true;
```

# TESTING NOTES
Testing is done using both Stub and Database, ensure you have a schema created and the correct credentials, refer to resources/data/samepageschema.sql
