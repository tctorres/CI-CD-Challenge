# CI-CD-Challenge
---
In this practice we are going to develop a simple Continuous Integration workflow, we are going to use Jenkins. The actions to perform are:
- Clone the repository and fetch the latest version of the source code.
- Create a Stage to Compile the application.
- Create a Stage to Execute the application (make sure pass the parameter in the command line to run the code properly)
---
## About the Project
### Topic: Web Automation
We are automating the  https://www.saucedemo.com/ web application. 
Creating a new Selenium - Java - TestNG project, and configuring it to launch  and test the required webpage on chrome browser. Implementing on our framework the following scenarios, each one as a different test:

- Purchase a product: Follow the complete buyflow of the page, selecting a random product, adding it to the cart, adding the personal data, and check you are successfully arriving at the “Thank you for your purchase” page.
- Removing elements of the shopping cart: Add 3 different elements to the shopping cart, enter to the cart page, remove them and check the shopping cart is empty.
- Logout: try to log out and check if you are correctly redirected to the login page.

For this implementation, follow the rules described next:
	
- Page Object Model should be correctly implemented, making sure to reuse certain elements and define base pages as needed for common methods and elements.
- Page factory is required.
- Before annotations should be used to manage preconditions. Any other required annotations can be implemented as needed.
---
## Run tests with Jenkins
1. Configure the project in the IDE.
 - Make sure these dependencies are added in the pom: TestNG, Selenium, Allure.
 - Create a jenkins file and configure it adding the parameters, tools, stages required, and post.
 - Save the changes and push it to the remote repository on github.
2. Create new Pipeline project:
 - Select the definition as **Pipeline script from SCM**.
 - Choose the SCM **Git**.
 - Copy and paste the repository URL.
 - Select the branch to build.
 - Provide the script path were is the jenkins file in the project.
 - Save and run.
---
## Allure report
- We need to configure the Allure commandLine in the option **Tools**
- Once we have it uploaded we will receive a report with all the behaviors that occurred during tests

 






