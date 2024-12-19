# Food-Redistribution-system
Food redistribution system
FoodBridge
<img src="src/main/webapp/assets/Banner.png">
FoodBridge is a web application designed to connect Food and Beverage (F&B) organizations with charities, enabling efficient redistribution of excess food. The primary goal is to minimize food wastage and alleviate hunger by redirecting surplus food to those in need.

Watch the live demo and explore the project proposal.

Motivation
Food wastage, hunger, and food insecurity remain critical global issues that directly impact the quality of life. Excess food often ends up in landfills, requiring additional waste disposal facilities and contributing to unnecessary energy consumption.

By redistributing surplus food to individuals and communities in need, FoodBridge aims to improve their standard of living and address these problems sustainably—without increasing overall food production.

Key User Groups
Food and Beverage organizations.
Charities focused on food redistribution.
Core Features
User Authentication: Secure login for F&B organizations and charities.
Main Dashboard:
Display of matched donations.
Dedicated sections for charities and restaurants.
Donation Form and Inbox:
Easy-to-use interface for creating, managing, and tracking donations.
Development Overview
FoodBridge is built as a Google App Engine Standard Java application, ensuring reliability, scalability, and integration with Google Cloud services.

Setup Guide
Prerequisites
Java 8.
Maven 3.5+.
Google Cloud SDK.
Initial Configuration
Initialize the Google Cloud environment:
bash
Copy code
gcloud init  
gcloud auth application-default login  
Running Locally
To start the application on a local development server:

bash
Copy code
mvn appengine:devserver  
Deploying to Google Cloud
Deploy the application with the following command:

bash
Copy code
mvn appengine:update  
Testing
To verify the application’s functionality, run:

bash
Copy code
mvn verify  
For improved reliability, add unit tests to the src/main/test/... directory. Utilize tools like JUnit 4, Mockito, and Truth for robust testing.

Maintaining Up-to-Date Dependencies
To ensure the project uses the latest libraries and tools, leverage the Maven Versions Plugin:

bash
Copy code
mvn versions:display-plugin-updates  
mvn versions:display-dependency-updates  
mvn versions:use-latest-versions  
Note: Be cautious when updating javax.servlet dependencies, as App Engine Standard uses Servlet 3.1 for Java 8 and 2.5 for Java 7.

Team
The project team consists of dedicated developers and advisors committed to building impactful solutions for food waste management.

