# Team-Cards
Unit 10 homework

# Project Description
The Team Cards Generator is a command-line-input application run in Node that requests information from the user about members of an engineering team and generates an HTML file displaying that information.  Before running the application the user must perform an npm install to install all required dependencies.

Upon launching the app, the user is prompted for multiple inputs that populate into an HTML via inquirer and fs. 

A screenshot showing an example user input is shown below:

![Screenshot of user input](images/teamcards1.png)

When all information on the team member has been entered, the user is asked whether there are any more members they would like to add.  If so, the user is asked the same questions about the new team member.  If not, an HTML file is created with cards displaying the information on all the team members entered by the user in the "outputs" folder titled "team.html."  A screenshot of an example team profile is shown below:

![Screenshot of HTML output](images/teamcards.png)

# Techniques and Technologies Used
This app was created using Object-Oriented Programming concepts, namely using classes and constructors to create "team member" objects based on information entered by the user.  The app is run using Node.js, and uses the "Inquirer" and "FS" node modules.  Files for different objects are also stored in separate .js files and passed among one another using module.exports and require.

This app uses concepts from Test-Driven Development.  Jest is used to perform tests on all the class constructors to ensure that they behave as expected.  The FS node module is used to generate an HTML file from strings written in JavaScript.  