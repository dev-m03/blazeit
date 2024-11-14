# Blazeit Tool

Blazeit is a command-line tool designed to quickly generate boilerplate files for a Spring Boot project. Using Blazeit, developers can automatically create essential components like Controllers, Services, and Repositories with minimal setup.  
  
Just setup once with three commands and use it all the time with just **one command** everytime you want quick setup.

## Setting Up Blazeit Using Scoop

Follow the steps below to set up **Blazeit** and start using it for generating Spring Boot files in your project. This guide assumes you are on **Windows** and using **PowerShell**.  
Here are steps to install scoop,jbang to setup once .

Scoop is a command-line installer for Windows that helps you install and manage software easily.

1. **Open PowerShell/IntelliJ Terminal** and run the following command to install Scoop:
   ```terminal
   iwr -useb get.scoop.sh | iex
2. **Install JBang** :
   ```terminal
   scoop install jbang
3. **Add the catlog** :
    ```terminal
    jbang catalog add --name mdev https://raw.githubusercontent.com/dev-m03/blazeit/main/jbang-catalog.json
The above three simple steps will setup blazeit on your system .

4. **The Final Command** to run blazeit everytime you want to setup the project :  
    ```terminal
    jbang blazeit@mdev <class name> <package name>
Provide the class and package names when prompted. Blazeit will automatically generate the following files in your project:

Controller class in src/main/java/{packageName}/controller/  
Service class in src/main/java/{packageName}/service/  
Repository interface in src/main/java/{packageName}/repository/  

The generated files will include boilerplate code for the Controller, Service, and Repository based on the names you provided.  

By following these steps, developers will be able to easily set up Blazeit on their local machine using Scoop, and generate Spring Boot files automatically in their projects.
    
  



      

   
  
