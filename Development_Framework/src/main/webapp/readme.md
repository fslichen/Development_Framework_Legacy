In order to craete a war file, right click on your project and select run as maven build. 
And the goal is as always, clean package. 
Make sure you are running on jdk rather than jre if you are using windows. 
Once there is no corrupted jar files, the build should be successful. 
Go to your project folder and file the target folder, go inside and you will find a war file. 
Copy the war file and then dump to the webapps folder under tomcat, and you should probably need to rename it cause the file name under maven is pretty long.
Suppose you rename your war file as run.war.
Then go to the bin folder under tomcat9, fire up the startup.bat file if you are using windows.
You will find that run.war file is extracted, and a new folder called run is created. 
Go inside the run folder, and go inside the WEB-INF folder, you will find classes folder, lib folder and web.xml
Now, open your browser and type in http://localhost:8080/run/get.do
You will be greeted by Hello World.