[vsCodeStartupCs]: img/vsCodeStartupCs.png " "
[vsCodeFortuneControllerCs]: img/vsCodeFortuneControllerCs.png " "
[vsCodeFortuneCs]: img/vsCodeFortuneCs.png " "



# Lab 01 - Clone Source and Push Apps

## Clone Source

1. Download the .NET app source code, by cloning Git Repo or download the zip
```

> git clone https://github.com/jennymclaughlin/DotNetAttendees

```
2. Download the Java app source code, by cloning Git Repo or download the zip
```

> git clone https://github.com/pivotal-education/pcf-articulate-code

```
3. Download the Node.js app source code, by cloning Git Repo or download the zip
```

> git clone https://github.com/Pivotal-Field-Engineering/cf-workshop-node

```

## Push The .NET App
1. Unzip pcf-asp.net-mvc-attendees.zip, open command prompt and navigate to the app directory.
```
> cd ~\pcf-asp.net-mvc-attendees\pcf-asp.net-mvc-attendees\PivotalWorkshop
```
2. Confirm the API target is set
```
> cf target

API endpoint:   <PROVIDED_BY_INSTRUCTOR>
User:           <STUDENT-X>
Org:            Hyvee
Space:          <STUDENT-X>
```
3. Push the app
```
> cf push <dotnetappName>-studentX -s windows2012R2 
```
4. The cf cli will provide feedback about each step it takes to create the App Container and deploy.

## View The .NET App
1. Verify your app in the apps manager
2. Question: What buildpack does it use?

## Push The Java App
1. Open command prompt and navigate to the app directory.
```
> cd pcf-articulate-code
```
2. Confirm the API target is set
```
> cf target

API endpoint:   <PROVIDED_BY_INSTRUCTOR>
User:           <STUDENT-X>
Org:            Hyvee
Space:          <STUDENT-X>
```
3. maven build
```
> mvn clean packate 
```
4. Push the app
```
> cf push <javaAppName>-studentX -p target\articulate-0.0.1-SNAPSHOT.jar
```
** No need to specifiy the windows stack

5. The cf cli will provide feedback about each step it takes to create the App Container and deploy.

## View The Java App
1. Verify your app in the apps manager
2. Question: What buildpack does it use?

## Push The Node.js App
1. Open command prompt and navigate to the app directory.
```
> cd cf-workshop-node
```
2. Confirm the API target is set
```
> cf target

API endpoint:   <PROVIDED_BY_INSTRUCTOR>
User:           <STUDENT-X>
Org:            Hyvee
Space:          <STUDENT-X>
```
3. Push the app
```
> cf push <nodeAppName>-studentX 
```
** No need to specifiy the windows stack

4. The cf cli will provide feedback about each step it takes to create the App Container and deploy.

## View The Java App
1. Verify your app in the apps manager
2. Question: What buildpack does it use?

___

___
| **[Prev Lab](../AppMgr-Login/README.md)** |_______________________________________________________________________________| **[Next Lab](../Lab-02/README.md)** |
