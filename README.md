
# :taxi: Taxi Service :taxi:
![image](https://user-images.githubusercontent.com/33402912/179487860-57038d45-5c95-49cf-978c-80dbdd571ba7.png)

## :technologist:General overview 

This is a simple program that demonstrates standard web service server operations and layer-to-layer communication.

## :desktop_computer:Used technologies 

- Java 11
- Maven
- MySQL 8.0.28
- JDBC
- Java Servlet API 4.0.1
- Tomcat 9.0.64
- JSTL 1.2

## :building_construction:Architecture

- Data presentation level
- Application level
- Data management level

## :classical_building:Data presentation level contains several JSP forms: 

- **Registration**, which allows you to register in the service as a driver
- **Authentication**, which allows you to login in the service
- **Display My Current Cars**, which shows cars, which are used by authenticated driver
- **Display All Drivers**, which shows all registered drivers
- **Diplay All Cars**, which shows all registered cars
- **Display All Manufacturers**, which shows all registered car manufacturers
- **Create new Car**, which allows you to register new car in the service
- **Create new Manufacturer**, which allows you to register new car manufacturer in the service
- **Add Driver to Car**, which allows you to designate registered car for registered driver

## :ladder:Application level contain 3-layer design itself: 

- **Controllers**: communicators between JSP and Services via HTTP
- **Services**: business logic operations
- **DAOs**: communicators between Services and DB via JDBC

## :bricks:Data management level structure 
![image](https://user-images.githubusercontent.com/33402912/179483689-ba7fbaa4-e32a-47b2-839a-f9a2f61dcaeb.png)

## :runner:How to run this project on your local computer 

1. Download and install MySQL, Apache Tomcat 9 (10 is not supported), Git, Maven, JDK 11.
2. Clone the project from GitHub
3. Configure Apache Tomcat and MySQL
4. Initialise database. Use for that src/main/resources/init_db.sql
5. Set URL, USERNAME, PASSWORD, JDBC_DRIVER in src/main/java/taxi/util/ConnectionUtil.java
6. Configure Tomcat library Application path in Edit configurations
7. Start Tomcat
8. Enter the browser and input the appropriate url

## :rocket:This project also has deployed at Heroku 

You could check it remote via [link](https://supermarche-monsieur-43317.herokuapp.com)
