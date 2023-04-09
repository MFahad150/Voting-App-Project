# Microservices Application Project
Through this project I deploy Microservices application on Kubernetes cluster. I have explored and analyzed, how various Kubernetes components work together. How configured YAML for deployment service for any application in **Kubernetes cluster**.

# Project Details
This is simple Voting application which provides an interface for the users to vote and another interface to show the result. The application consists on various components such as the **Voting-App**, which is a web application developed in **Python** to provide user an interface to choose between two options. When we make a selection the vote is store in **redis**, the vote is then process by **Worker** which is an application written in **.NET** the worker application takes the new vote and update the persistent database which is a **PostgresSQL**. The PostgresSQL simply has a table with the number of votes for each category. Finally the result of the vote is displayed in a web interface which is another web application written in **NodeJS**, this resulting application reads the count of votes from the PostgresSQL database and displayed it to the user.

***Note:-*** This application is built with a combination of different services, differnet development tools and multiple different platform such as **Python**, .**NET**, **PostgresSQL** and **NodeJS**.

**Source: KodeKloud**
