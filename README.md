# AWS-Webapp-in-Cloud9
Project Title: Building a Web App and IDE in AWS

Presented by: Shivani Gondi

Introducing Today's Project
What is AWS Cloud9 and Why is it Useful?
AWS Cloud9 is an Integrated Development Environment (IDE) that allows you to write, run, and debug your code with just a browser. It’s useful for:

Code Commit: Easily manage your source code.
Code Build: Automate the process of building your code.
Code Execution: Run your applications directly in the cloud.
Accessibility: Accessible from anywhere, even on mobile devices.
How I'm Using Cloud9 in This Project
I have:

Created a web app.
Set up the Cloud9 environment.
Configured IAM (Identity and Access Management) users with specific permission policies.
Unexpected Discovery: Using mvn commands to create the web app was surprisingly easy, achievable with just a single command.


Setting Up an IAM User
What is an IAM User?
An IAM user is a way to grant access to AWS resources. It allows you to specify detailed access levels to your account's resources and services.

Importance of IAM Users
Creating IAM users is crucial because:

The root user is vulnerable to security breaches.
IAM users can be assigned specific permissions to enhance security.
Setup: I created an IAM user with Administrator Access, allowing full control over all resources in my AWS account.

Environments & IDEs
What is an Environment?
An environment in this context refers to a set of resources and configurations required to run and build your software application. It’s akin to a chef needing specific tools and ingredients to cook a meal.

What is an IDE?
An IDE (Integrated Development Environment) is a software application that provides comprehensive facilities to computer programmers for software development. It typically includes:

A source code editor
Build automation tools
A debugger
Launching a Cloud9 IDE
Benefits of Using Cloud9
The Cloud9 environment comes pre-configured with essential tools like Git, which saves time and simplifies the setup process.

Maven & Java
What is Apache Maven?
Apache Maven is a powerful build automation tool used primarily for Java projects. It manages project builds, documentation, and dependencies.

Roles of Maven:

Compiling
Testing
Linking
Packaging
What is Java?
Java is a versatile and widely-used programming language. It is essential for building various types of applications, from mobile apps to large enterprise systems.

Role of Java in the Project:

Building the web app's backend.
Creating the Application
To create a simple Java web application, I used the following Maven command:

sh
Copy code
mvn archetype:generate \
  -DgroupId=com.nextwork.app \
  -DartifactId=nextwork-web-project \
  -DarchetypeArtifactId=maven-archetype-webapp \
  -DinteractiveMode=false
Once the web app was created, the IDE automatically generated a README file.
