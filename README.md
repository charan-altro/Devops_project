2. Create a Simple Java Web Application Using Spring Boot
Generate a Spring Boot Project:

Use Spring Initializr to generate a new Spring Boot project. You can use the web interface to select the necessary settings:

Project: Maven Project
Language: Java
Spring Boot: 3.x (latest stable version)
Group: com.example
Artifact: mywebapp
Dependencies: Spring Web
Click on Generate, which will download a ZIP file containing your project.

Upload and Extract the Project:

Upload the ZIP file to your Azure VM, then extract it:

bash
Copy code
unzip mywebapp.zip
cd mywebapp
3. Build and Run the Java Application Locally
Navigate to the Project Directory:

bash
Copy code
cd mywebapp
Build the Application:

Use Maven to build the project:

bash
Copy code
mvn clean package
This will compile the code and package it into a JAR file.

Run the Application:

Run the JAR file with Java:

bash
Copy code
java -jar target/mywebapp-0.0.1-SNAPSHOT.jar
By default, the application will be available at http://localhost:8080.

Verify the Application:

Open a web browser or use curl to check if the application is running:

bash
Copy code
curl http://localhost:8080
You should see the default Spring Boot welcome page or any other output you've configured.

4. (Optional) Set Up a Simple CI/CD Pipeline
If you want to practice DevOps further, you can set up a basic CI/CD pipeline for your Java application using Jenkins:

Install Jenkins:

Follow the Jenkins installation instructions for Ubuntu.

Create a Jenkins Job:

Open Jenkins in your browser (usually at http://localhost:8080).
Create a new Freestyle project.
Configure the job to pull your project from a Git repository.
Add a build step to execute mvn clean package.
Add a post-build action to archive the built JAR file.
Test the Jenkins Pipeline:

Trigger the build job in Jenkins.
Verify that the build completes successfully and the JAR file is created.
Summary
Install Java, Maven, and Git on your Ubuntu VM.
Create a Spring Boot project using Spring Initializr and build it with Maven.
Run and test the application locally.
Optionally, set up a Jenkins job to automate the build process.
This should give you a solid foundation for practicing DevOps on your Azure VM. Let me know if you need further details or run into any issues!


how to unzip Devops_project.git

