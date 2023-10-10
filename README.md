Software Requirements Specification (SRS) 

 

Project Name: Quoting Project 


1. Introduction 

1.1 Purpose 

The Quoting Project aims to provide a web application that allows both existing and new customers to request quotes. This Software Requirements Specification (SRS) document outlines the functional and non-functional requirements for the Quoting Project. 

1.2 Scope 

The scope of the Quoting Project encompasses the following features: 

User Authentication and Authorization 

Select Page 

Location Page 

Product Selection Page 

Configuration Page 

Billing Page 

Integration with the Catalog project for product information retrieval 

Data persistence in a PostgreSQL database 

API development and documentation using Swagger 

Utilization of Java concepts such as Streams and Lombok 

Use of one-to-many and many-to-one relationships between database tables 

1.3 Document Conventions 

UI: User Interface 

API: Application Programming Interface 

DB: Database 

1.4 Intended Audience 

The intended audience for this document includes: 

Developers and programmers responsible for implementing the Quoting Project 

Testers responsible for testing the system 

Project managers and stakeholders 

2. Overall Description 

2.1 System Overview 

The Quoting Project is a web-based application built using Angular 16 for the frontend, Java with Spring Boot for the middleware, and PostgreSQL for the database. It provides a seamless user experience for requesting and configuring quotes for various products. 

2.2 System Architecture 

The system follows a client-server architecture with Angular serving as the client, Spring Boot as the middleware, and PostgreSQL as the backend database. The communication between the client and server is facilitated through RESTful APIs. 

2.3 Technologies Used 

UI / Framework: Angular 16, HTML5 

Middleware: Java/Spring Boot 

Backend: PostgreSQL 

Server: Embedded Tomcat 

Build Tool: Maven 

3. Detailed Requirements 

3.1 User Authentication 

Users can log in if they are existing customers or sign up as new customers. 

Authentication will be implemented using a secure mechanism. 

Proper access controls and authorization mechanisms must be in place to ensure data security. 

3.2 Select Page 

Display customer name, account status, quote name, and quote owner. 

Generate a unique quote ID for each quote and store it in the database. 

Account status can be either "New" or "Existing Customer." 

3.3 Location Page 

Show a table of saved locations and allow users to add new locations. 

Implement location validation to ensure the correctness of provided location details, including name, street name, city, state, country, and pin code. 

Locations must be persisted in the database. 

3.4 Product Selection Page 

Display products created through the Catalog project in a tile format. 

Allow users to select products by clicking on the tiles. 

3.5 Configuration Page 

Show selected locations and products in dropdowns. 

Implement an "enable" button that displays product details, including associated features and parameters retrieved from the Catalog project. 

Allow users to enter values for parameters based on their types and restrictions. 

Persist configuration data to the database. 

3.6 Billing Page 

Calculate and display billing items and costs based on the selected products and configurations. 

 
