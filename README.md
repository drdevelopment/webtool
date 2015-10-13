# Welcome to WebTool
WebTool is a new tool to setup and edit your website (in only 5 minutes) written in Java and Javascript. This is one of the goals of this project. The other goal is to create a Core which can be used to create micro-services. Due to its pluggable components it is easy to extend.
The core is also an integration of several powerfull Java frameworks, like **Jetty**, **Angular**, **RestEasy**, **Jackson**, **H2**, **JDbi**, **Appache Commons** and security (JAAS). When I start to create a new web-application, it always costs me a lot of time to find and integrate these frameworks.

This is also free-of-anything and is delivered with the **MIT-license**. Hopefully, you will enjoy WebTool and if you are interested, help me to improve it! Please, click :star: (on top of the screen) to star the project or fork this project. 

## Build and run
If you have installed Maven and Java, please execute the follow command from the parent directory.
```
mvn clean install -DskipTests
```
After you build the project, the folder distribution is created. Go to this folder and start WebTool with the following command:
```
java -jar drdevelopment-core-0.2-SNAPSHOT.jar
```
The application will start and will create more folders like: data, logs and configuration. After the database is created and the webserver is started, open a browser and go to *http://localhost:8080*

## Welcome to WebTool
When you started the application, go to url *http://localhost:8080*
You will see the setup-screen:

![Setup with WebTool](http://www.drdevelopment.org/static/images/setup.png)

![Setup with WebTool](http://www.drdevelopment.org/static/images/login.png)

After you logged in, you are able to enter content for your website:

![Setup with WebTool](http://www.drdevelopment.org/static/images/paragraph.png)

And after 5 minutes dragging and uploading images and entering content, you can display your website in the browser:

![Setup with WebTool](http://www.drdevelopment.org/static/images/website.png)

The website is made with Bootstrap and Angular and is fully mobile. The background image / fonts and colors can be configured.

## Architecture

This project contains several plugins which are loaded during startup. New plugins can be made and attached to extend the system.

The following frameworks are used in WebTool:

| Name                 | Description                                             | Link                                    |
| -------------------- | ------------------------------------------------------- | --------------------------------------- |
| Logback              | Ultra fast logging framework                            | https://github.com/qos-ch/logback       |
| Appache Commons CLI  | Library for command line interfaces                     | https://github.com/apache/commons-cli   |
| Appache Commons IO   | Library for additional IO                               | https://github.com/apache/commons-io    |
| Appache Commons Lang | Library for language support                            | https://github.com/apache/commons-lang  |
