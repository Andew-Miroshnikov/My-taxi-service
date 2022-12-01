# <h1 align="center">:oncoming_taxi: Taxi-Service :oncoming_taxi:</h1>
:taxi: **Taxi-Service** is a simple web-application that supports <em>registration</em>, <em>authentication</em> and other <em>CRUD</em> operations. Application compile
with <i>SOLID</i> principles, Dependency <i>Injection</i> and other ***OOP*** principles.

:dart: Features
---
+ [X] registration like a driver
+ [X] authentication like a driver
+ [X] login like a driver
  + [X] add driver to car
  + [X] display list of driver's all cars
+ [X] create/update/remove manufacturer
+ [X] display list of all manufacturer
+ [X] create/update/remove car
+ [X] display list of all car
+ [X] create/update/remove driver
+ [X] display list of all drivers

## :pancakes: Structure
----
|<img src="https://spaces-cdn.clipsafari.com/cehwijh0e7m9jv1r9g7hrgz5u70i" alt="comp" width="30"/>|
|----------|
|<div align="center">:arrow_double_down::arrow_double_up:</div>|
|<div align="center">Filter</div><div align="center">Controller</div>|
|<div align="center">:arrow_down::arrow_up:</div>|
|<div align="center">Service</div>|
|<div align="center">:arrow_down::arrow_up:</div>|
|<div align="center">Dao</div>|
|<div align="center">:arrow_double_down::arrow_double_up:</div>|
|<div align="center"><img src="https://spaces-cdn.clipsafari.com/bsu2nc68wv4cpli10l62sotq9ma4" alt="database" width="30"/></div>|

## :key: Entity relations in DB
---
<img src="https://user-images.githubusercontent.com/112484426/204644103-7ec41c09-05e6-4f3b-9341-47ddeaf81d3b.png" alt="drawing" width="400"/>

## :electron: Technologies
---
+ ![JDK](https://img.shields.io/badge/JDK-11-red)
+ ![maven](https://img.shields.io/badge/Maven-3.8.1-blue)
+ ![JDBC](https://img.shields.io/badge/JDBC-API-orange)
+ ![mysql](https://img.shields.io/badge/Mysql-8.0.22-lightgrey)
+ ![servlet](https://img.shields.io/badge/ServletAPI-4.0.1-brightgreen)
+ ![JSP](https://img.shields.io/badge/JSP-html%2Fcss-yellow)
+ ![Jstl](https://img.shields.io/badge/JSTL-1.2-blue)
+ ![Tomcat](https://img.shields.io/badge/Tomcat-9.0.69-green)
+ ![war](https://img.shields.io/badge/WAR-3.3.2-red)
+ ![herocu](https://img.shields.io/badge/Heroku-%40deprecated-lightgrey)

## :rocket: Run the app
---
+ [ ] Clone the project from the GitHub
+ [ ] Copy [init_db](https://github.com/Andew-Miroshnikov/My-taxi-service/blob/hww/src/main/resources/init_db.sql) configuration to create schema
+ [ ] Create connection in [**taxi/util/ConnectionUtil.java**](https://github.com/Andew-Miroshnikov/My-taxi-service/blob/hww/src/main/java/taxi/util/ConnectionUtil.java) class
  + [ ] write your **URL**
  + [ ] write your **USERNAME**
  + [ ] write your **PASSWORD**
  + [ ] write your **JDBC_DRIVER**
    + :warning: if you have problems with this punkt you can easely find it in internet, just write "***YOUR DATABASE NAME*** *driver class name*"
  + :eyes: pay attention for this part `?serverTimezone=UTC`
  + :warning: if u use not [MySql](https://dev.mysql.com/downloads/installer/) database , don't forgot to change dependency in **pom.xml**
    ```java
    <dependencies>
      <dependency>
          <groupId>mysql</groupId>
          <artifactId>mysql-connector-java</artifactId>
          <version>8.0.22</version>
      </dependency>
      ```
+ [ ] Configure [Tomcat](https://tomcat.apache.org/download-90.cgi) local server
  + :warning: not recommended to use tomcat 10 version , cause you can need extra settings
+ [ ] Run Tomcat feel free to push buttons and write your data in query :octocat:   
