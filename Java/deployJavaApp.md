0202206112029
Status: #idea
Tags:[[Java]]


# Deploying Java App
1.  Set up visual studio code for java
	1.  Install Microsoft Java extension pack-
		VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack
	2. Install Microsoft Java Debugger:
		VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-debug
1.  Download and install Apache Maven
	1.  Check to ssee if it's installed or not, in terminal type:
	```
	mvn -version
	```
	2. Go to: https://maven.apache.org/download.cgi
	3. Click on Binary tar.gz archive file and download
	4. Unzip file
	5. Open terminal and cd into downloads folder:
		```
		mv apache-maven-3.8.6 /Applications/
		```
	6. CD into Applications and ls to see if folder was moved sucessfully
	7. CD into apache-maven folder
	8. In new terminal:
	```
	cd /Users/username
	ls -al
	```
	9. Look to see if `.bash_profile` exists in directory
	10. If doesn't exist `touch .bash_profile`
	11. In terminal `open -e .bash_profile`
	12. In .bash_profile file add:
	```
	export M2_HOME=/Applications/apache-maven-3.8.6
	export PATH=$PATH:$M2_HOME/bin
	```
	12. `clear` terminal
	13. refresh bash profile in terminal `source .bash_profile`
	14. `mvn -version` to see maven version installed
	15. Alternative: https://maven.apache.org/install.html
4.  Create free Azure account
https://azure.microsoft.com/en-us/free/
5.  Install azure app service extension:
	VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azureappservice
1.  Create new web app on azure
	1.  Sign in to azure through vs code.
2.  Once you have signed in, you can open the command prompt or terminal window and build the project using Maven commands <---- this i have no idea what it means:
```
mvn clean package
```
4.  last step will generate a war or jar file in the target directory
5.  After building the project, open the `target` directory in VS Code Explorer. Right-click on the file and choose Deploy to Web App, and follow the prompts to choose the Web App for your deployment.
6.  open output window in vs code once deployment is completed it will print out a url for your web app.
7.  copy and paste to browswer to see it running on Azure



# References
Full guide:
https://code.visualstudio.com/docs/java/java-webapp
Maven Download & Insall guide:
https://www.youtube.com/watch?v=uZ1yNWKd7zM