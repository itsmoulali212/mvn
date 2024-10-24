What is maven? 
Prerequisites:
1.	Jenkins Installed
2.	Maven Installed
3.	Java Project with Maven

Step #1: Install GitHub Integration and Maven Plugins in Jenkins To build Java project with maven we need to install some plugins like,
•	GitHub Integration Plugin
•	Maven Integration Plugin

Step #2: Create a New Freestyle Project in Jenkins 

Step #3: Configure Source Code Management 

Step #4: Configure the Build
Add Build Step: In the "Build" section, click on "Add build step" and choose "Invoke top-level Maven targets."
Configure Maven Build: In the "Goals" field, enter the Maven goals you want to execute (e.g., clean install). Specify the path to your pom.xml file.

Step #5: Configure Post-Build Actions 
Archive Artifacts: In the "Post-build Actions" section, click on "Add post-build action" and select "Archive the artifacts." 
In the "Files to archive" field, enter the relative path to the JAR or WAR file that Maven generates (e.g., target/.jar or target/.war). 

Step #6: Monitor Build Progress 
View Console Output: Click on the build number in the "Build History" section to view the console output. You can monitor the progress and identify any issues during the build process. 
Check Artifacts: if the build is successful, you can go to the "Build Artifacts" section in the job page to download the archived artifacts.
