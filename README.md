# Social-Fitness-Web
The interactive group fitness tracker is designed to tackle the common struggles of motivation and discipline by promoting social exercise. The app allows users to track their personal health changes, document workout schedules, and access workout guides. It also encourages users to form groups with friends, colleagues, or others to work out together and share achievements.

# Technologies
- Java Spring Boot
- React
- MySQL
- Websocket
- JUnit
- Third Party API

# How to Run?
### MySQL

**BEFORE running the application ensure the following is done in MySQL**

This is to ensure `application.properties` values are correct.

1. Inside a MySQL console complete the following commands your local machine...<br>
     `mysql> create database db_elec_project;` <br>
     `mysql> create user 'springelecuser'@'%' identified by 'ThePassword123';` <br>
     `mysql> grant all on db_elec_project.* to 'springelecuser'@'%';`

2. Before moving to gradle set up ensure the database `db_elec_project` is running on your local computer. 

### Gradle
Running `gradle bootRun` should install the correct dependencies and run the Spring Server <br>

    If using Intellij ensure inside your gradle settings the correct `Gradle JVM` is selected

**Once `gradle bootRun` is done you can now access the application**
`localhost:<port>/`

### There are 2 example users provided upon running the application

1. username: user@email.com <br>
password: '123'
2. username: user+1@email.com <br>
password: 'password'

Other data is written to the tables inside the database upon starting the application to demonstrate some features more easily

## Run Unit Tests

Run `gradle test`
