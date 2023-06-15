<p align="center">
    <img src="img/taxi.webp" />
</p>

# Taxi-Service

<img src="img/icon.png" align="right" />

## ⚡ _Project description:_

```
A simple web-application that supports authentication, registration and other CRUD operations.
```

> [Demo link](http://java-web-security.us-east-1.elasticbeanstalk.com/) - deploying on Amazon Web Services (AWS)

## 🎯 Features:

<img src="img/taxi-service.gif" align="right" width="240">

- `registration` like a driver;
- `authentication` like a driver;
- `create/remove` a manufacturer;
- `create/remove` a car;
- `create/remove` a driver;
- `display` list of all manufacturers;
- `display` list of all cars;
- `display` list of all drivers;
- `display` list of my cars;
- `add` driver to car.

## Used technologies

`Java 11`, `Servlet`, `JDBC`, `JSP`, `JSTL`, `Maven`, `HTML`, `CSS`

## ⚙️Installation:

### _To run this project you need to install:_

- [IntelliJ IDEA Ultimate](https://www.jetbrains.com/lp/intellij-frameworks/)
- [Java 11](https://jdk.java.net/java-se-ri/11)
- [Tomcat 9.0.50](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
- [MySQL Installer](https://dev.mysql.com/downloads/installer/)
- [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

## 🧬 Settings

### _After installation, you should do the following:_

- Add this project to IntelliJ IDEA Ultimat
- [Configure Tomcat](https://javarush.ru/quests/lectures/questservlets.level11.lecture04)
- [Connecting to the database with MySQL Workbench](https://javarush.ru/quests/lectures/questhibernate.level05.lecture03)
- To get the actual parameters of the database tables, run script from the `resources/init_db.sql` file in the Workbench
- Insert sql query to have registered user (Login: `root` Password: `1234`)
```mysql
INSERT INTO drivers (name, license_number, login, password) VALUE ('Admin', 'ABB123456', 'root', '1234');
```

- Establish a database connection using the file `java/taxi/util/ConnectionUtil`, replace with your settings

**Example:**
```java
private static final String URL = "YOUR_URL";
private static final String USERNAME = "YOUR_USERNAME";
private static final String PASSWORD = "YOUR_PASSWORD";
private static final String JDBC_DRIVER = "YOUR_JDBC_DRIVER";
```

- Run the project using Tomcat 9.0.50

<img src="img/run.png" />

#### ☕ P.S. To create a car, you must first create a manufacturer 

**Enjoy**  💛💙
