# Apache Maven through Command Line
# Creating a Simple Java Project name: my-app

## Step 1: Create the java project
```
First go to the desired folder where you want to keep your app
Make sure maven is installed on the system, check using mvn –version.

Now run the below command to create the java project
Syntax: mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

Explanation: 
Only two things are of concern:
1) Group ID: This will be our package name (com.mycompany.app ; package names are defined under com by convention, package name -> mycompany.app. So our java file would be present under com -> mycompany -> app -> app.java)
2) Artifact ID: This is our project name (my-app)
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1606).png)

### Now after running the above command, our project structure got created.

## Step 2: Check the Directory Structure of above created project by going into the directory

```
At the source folder of the project:
1) src/ 
It contains two folders:
1.1) main/ 
It is used to create codes in java
1.2) test/
It is used to create JUnit Test cases
2) pom.xml

Pom.xml is the mail build file of the maven!
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1607).png)

## Step 3: Change the source code (and file name) as you want to make
```
Go to src/main/java/com/mycompany/app/
NOTE: app is the package name we defined while creating the project.
Always include package name in the code.
Modify the App.java file 
Rename to the file name you want.
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1608).png)

## Step 4: Clean the project area
### Syntax: mvn clean

```
Before start building a project, it is necessary to delete old configuration files.
mvn clean command is used to delete the target/ folder.
Before running the clean command, make sure to be in the my-app directory, where src and pom.xml file are present
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1609).png)

## Step 5: Compile the Project source code
### Syntax: mvn compile

```
This command is used to check whether the source code we wrote in java file is correct syntactically or not.
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1611).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1612).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1613).png)

## Step 6: Unit Testing
### Syntax: mvn test

```
This work is tricky. 
You must know how to create JUnit Test cases.
You need to define the Unit Test cases in /src/test/java/com/mycompany/app
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1614).png)

### Now run the mvn test command

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1616).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1617).png)

## Step 7: Install (Build the Project)

```
Checks the Maven Configuration in pom.xml file
Creates the project build.
Creates jar file in target/ folder which can be deployed
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1618).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1619).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1621).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1622).png)

## Step 8: Site 
### Syntax: mvn site

```
Maven Site command is used to create GUI reports
It creates reports in format of web pages in HTML+CSS format.
Site Reports are stored in /target/site
```

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1624).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1625).png)

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1626).png)

## To view the Web page of site report, go to target -> site -> index.html

![Image](https://github.com/srabhayraj/Maven-Using-CommandLine/blob/master/metadata/IMG/Screenshot%20(1627).png)

## How To Contribute

[Contribution Guidelines](CONTRIBUTING.md)

## Contributors

[@srabhayraj](https://github.com/srabhayraj)

## License

[GPL Licence](LICENSE)

