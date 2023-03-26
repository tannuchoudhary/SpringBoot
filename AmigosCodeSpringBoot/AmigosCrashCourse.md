# 1. Overview

![Screenshot from 2022-02-06 18-29-23](https://user-images.githubusercontent.com/42698268/153379293-ed8c4265-a90b-473d-9508-4c709301bf65.png)

# 2. API
![image](https://user-images.githubusercontent.com/42698268/217210610-053b54cf-c3dc-42e5-8a38-02c5fdbc65dc.png)
![image](https://user-images.githubusercontent.com/42698268/217210881-d9c6663e-a429-4342-b101-acd4871344e1.png)
![image](https://user-images.githubusercontent.com/42698268/217212176-0dc556c2-f18c-4aff-99d4-3ebd7f6f9709.png)
![image](https://user-images.githubusercontent.com/42698268/217212902-04c1755c-a1c5-40e0-87e7-1889cffc2a58.png)
![image](https://user-images.githubusercontent.com/42698268/217529097-7b0f3098-6618-49aa-b31e-d284e1fee46b.png)

* checkout more about the api's [here](https://aws.amazon.com/what-is/api/)


![Screenshot from 2022-02-06 18-29-49](https://user-images.githubusercontent.com/42698268/153379301-6e9b2eca-956b-42a3-8f91-399ead8b1bf5.png)
 * security modules: for security in spring boot project
 * for logging you can use logging
 * you can connect to postgresql, mongodb, mysql, you can connect to any databases
 * Metrics: helps us to check how the application is behaving in production
 * Also it is production ready, so you have microservices, dependency injection, built in configuration etc
# 3. Selecting Dependencies which our project need
* Spring web
* Spring data JPA for connecting through database using JPA and Hybernet
* PostgreSQL Driver : for connecting to real database

![Screenshot from 2022-02-10 15-07-12](https://user-images.githubusercontent.com/42698268/153379538-a64443f4-820f-497e-8e85-49a44709d3ba.png)

![Screenshot from 2022-02-10 15-08-45](https://user-images.githubusercontent.com/42698268/153379781-9329be14-f5c3-40c7-8bcd-3ec1cafeec5c.png)

![Screenshot from 2022-02-10 15-09-10](https://user-images.githubusercontent.com/42698268/153379825-8eda224e-8b9d-46fc-a6cc-3e07ddd73170.png)

# 4. Download and extract selected dependencies

![Screenshot from 2022-02-10 15-14-17](https://user-images.githubusercontent.com/42698268/153380692-b7396d55-2a8b-4b25-881e-17c4a6ea47c1.png)
![Screenshot from 2022-02-10 15-14-04](https://user-images.githubusercontent.com/42698268/153380699-4dd8b245-6326-4c03-b928-cd4ba838c1bb.png)

# 5. Import this project in your IDE

![Screenshot from 2022-02-10 15-15-18](https://user-images.githubusercontent.com/42698268/153380866-1a42193f-6e87-4ba3-8231-3482d5fb3c07.png)
* application.properties: This is where we configure all the properties for our application as well as environment specific properties
* Static and templates: Here we do all our web development
* 
# 6. Starting the server
Run the DemoApplication.java, you will get an error because application will try to connect to the database
* Open pom.xml
* and comment the dependecy of spring-boot-starter-data-jpa
* and reload the project, so that this dependency will be removed(imp)
* This dependency will be added back once we are ready to connect it with database

* We will use ```@GetMapping``` to get something out of our server
* ```@RestController``` makes this class to serve rest end points
* Now what is REST and rest API

# 7. REST API's - How they work and what you need to know
* In this age of integrations, sharing data between systems is more important than ever.
![image](https://user-images.githubusercontent.com/42698268/217535822-bae53788-2286-47c0-a35d-ad04bfec7213.png)

# 8. What API's are and how they work
![image](https://user-images.githubusercontent.com/42698268/217536657-a2bf1cfc-becc-46b2-b59d-76e71c743916.png)
![image](https://user-images.githubusercontent.com/42698268/217536761-34496067-2661-42b3-95d1-4a5218943172.png)
![image](https://user-images.githubusercontent.com/42698268/217545517-ce11a030-b192-4a79-9574-eefa23f4eeac.png)
![image](https://user-images.githubusercontent.com/42698268/217545615-a88c8076-748f-4765-bfeb-1efe5ee41a0a.png)
![image](https://user-images.githubusercontent.com/42698268/217545684-9accd995-ea1b-4c70-8d04-9525e6b88bdb.png)
![image](https://user-images.githubusercontent.com/42698268/217545817-14f40a32-8ae6-49af-a516-b094ff7bf892.png)
![image](https://user-images.githubusercontent.com/42698268/217545964-246f89d1-52d3-429d-b3e0-4ab01f2ba365.png)
![image](https://user-images.githubusercontent.com/42698268/217546128-ecabd4da-6821-4214-a7e0-394dfd1bf83d.png)
![image](https://user-images.githubusercontent.com/42698268/217546365-f117c8e5-8376-4a19-a9c9-cd15680eb438.png)


* [HERE](https://blog.hubspot.com/website/application-programming-interface-api?hubs_content=blog.hubspot.com%252Fwebsite%252Ftypes-of-apis&hubs_content-cta=guide%2520to%2520REST%2520APIs) IS GREAT ARTICLE ON API, THIS WILL CLEAR ALL YOUR DOUBTS ABOUT API FOR SURE

![Screenshot from 2022-02-10 15-25-24](https://user-images.githubusercontent.com/42698268/153382722-6fb7ae9f-25e7-423e-887d-e861ac65311b.png)
* Now run the application
* Open localhost:8080 , you can find your web server running on this port and it will have nothing as we haven't implemented anything


![Screenshot from 2022-02-10 15-26-54](https://user-images.githubusercontent.com/42698268/153383043-da5d2ba6-74d1-49a3-b351-d56636f4987a.png)


# 5. Let us create a simple API


## a.

![Screenshot from 2022-02-10 15-53-55](https://user-images.githubusercontent.com/42698268/153387665-e77de8e8-7c40-4dd5-a333-c73bb9442b9b.png)

![Screenshot from 2022-02-10 15-53-48](https://user-images.githubusercontent.com/42698268/153387743-04f61857-faa3-4011-9eff-6d0a43264bc8.png)


## b.we can also pass it as list

![Screenshot from 2022-02-10 15-51-51](https://user-images.githubusercontent.com/42698268/153387247-6c49ceb6-aaf4-4fec-a844-d4ac1fd5c4a5.png)
 
 
 
![Screenshot from 2022-02-10 15-51-59](https://user-images.githubusercontent.com/42698268/153387317-89e77448-b61f-4c23-a197-7ec3b77a1b01.png)

* let us implement this student class and implement all the functionalites with it
* Let us take a class and model it as a student with all the attributes

![image](https://user-images.githubusercontent.com/42698268/219276970-3a51cae4-908f-4d6d-9fcc-25e87fb5e458.png)
![image](https://user-images.githubusercontent.com/42698268/219277173-d2b6ffee-063e-4fe1-8fbd-e10a138b610e.png)

### Implementation:
* Define the fields of student and generate no arg constructor for class, constructors for each field, one constructor without id as it will be given by db, getters, setters and toString for each field

```java
package com.example.demo.student;

import java.text.DateFormat;
import java.time.LocalDate;

public class Student {
    private Long id;
    private String name;
    private String email;
    private LocalDate dob;
    private Integer age;


    public Student() {
    }

    public Student(Long id,
                   String name,
                   String email,
                   LocalDate dob,
                   Integer age) {
        this.id = id;
        this.name = name;
        this.email = email;
        this.dob = dob;
        this.age = age;
    }

    public Student(String name,
                   String email,
                   LocalDate dob,
                   Integer age) {
        this.name = name;
        this.email = email;
        this.dob = dob;
        this.age = age;
    }

    public Long getId() {
        return id;
    }

    public void setId(Long id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    public LocalDate getDob() {
        return dob;
    }

    public void setDob(LocalDate dob) {
        this.dob = dob;
    }

    public Integer getAge() {
        return age;
    }

    public void setAge(Integer age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "Student{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", email='" + email + '\'' +
                ", dob=" + dob +
                ", age=" + age +
                '}';
    }
}


```
* This will be your main function
```java
package com.example.demo;

import com.example.demo.student.Student;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

import java.time.LocalDate;
import java.time.Month;
import java.util.List;

@SpringBootApplication
public class DemoApplication {

	public static void main(String[] args) {
		SpringApplication.run(DemoApplication.class, args);


	}
	@GetMapping
	public List<Student> hello(){

		return List.of(
				new Student(
						1L,
						"Tannu",
						"tannu@gmail.com",
						LocalDate.of(1999, Month.JANUARY, 10),
						23
				)
		);
	}
}
```
# 6. Controller layer
* let us add a controller layer inside student package
* and add @RestController, @RequestMapping, path in request mapping and the method which returns the data of student in the controller class

```java
package com.example.demo.student;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.time.LocalDate;
import java.time.Month;
import java.util.List;

@RestController
@RequestMapping(path = "api/v1/student")
public class StudentController {
    @GetMapping
    public List<Student> getStudents(){

        return List.of(
                new Student(
                        1L,
                        "Tannu",
                        "tannu@gmail.com",
                        LocalDate.of(1999, Month.JANUARY, 10),
                        23
                )
        );
    }

}
```
# 7. Now let us add a service layer or also called as a business layer
![image](https://user-images.githubusercontent.com/42698268/223364449-281ff63e-c055-4168-83bd-12ad57583aef.png)

* Now understand that, api  layer should talk to service layer to get some data and service layer should talk to data access layer to get some data
* So create a StudentService class, and cut the getStudent method from controller and paste it in service method and now in controller we will just call that method
* to call the method from service, we need to create an object of service class in controller class, so create an object, instantiate it using constructor and then call the method getStudents here in controller
* this is a much better design approach and we are using the n tier design pattern
* right now, whatever we are returning from getStudents is a static list, we want it to come from a database, so we will connect it with db later

# 8. ANnotations and Dependency Injection
* now we have to create an instance of StudentService to run the code
* two ways to create an instance:
	* using new keyword
	* using dependency injection
* dependency injection is preferred to maintain loose coupling
* here we will use @Autowired which will tell the constructor to automatically instatiate the StudentService
* also we have to tell that this StudentService is a class that has to be instantiated and has to be a spring bean 
* so we will use @Component for that, now we can see that the error is gone, and code is running perfectly

### Controller class
```java
package com.example.demo.student;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.time.LocalDate;
import java.time.Month;
import java.util.List;


@RestController
@RequestMapping(path = "api/v1/student")
public class StudentController {

    private final StudentService studentService;
    @Autowired
    public StudentController(StudentService studentService){
        this.studentService = studentService;
    }

    @GetMapping
    public List<Student> getStudents(){
        return studentService.getStudents();
    }

}
```
### Service class
```package com.example.demo.student;

import org.springframework.stereotype.Component;

import java.time.LocalDate;
import java.time.Month;
import java.util.List;

@Component
public class StudentService {
    public List<Student> getStudents(){

        return List.of(
                new Student(
                        1L,
                        "Tannu",
                        "tannu@gmail.com",
                        LocalDate.of(1999, Month.JANUARY, 10),
                        23
                )
        );
    }
}
```
* but we don't want it to be any regular component, we want it to be a service component, so we will annotate it with @Service
* so service and component are basically same, but service is more for semantic and readabilty which tells that this class is meant to be a service class
* so for controller, we use ```@RestController``` and for service we use ```@Service```
![image](https://user-images.githubusercontent.com/42698268/223372919-f904cc20-807e-41f1-8e08-ab7a1d643605.png)
* so we can see that project is running fine and we have separated the layers as controller and service layer and controller layer is talkin gsuccesfully to service layer and service layer is giving back some data to the controller layer(API Layer)

# 9. Let us create a Data Access layer

## A. Properties file
* We will go here to take some code https://github.com/amigoscode/spring-data-jpa-course
* let us copy application.properties file from here and paste it in your own project
* The below is the configuration we need in order to connect to a DB

```java
spring.datasource.url=jdbc:postgresql://localhost:5432/student
spring.datasource.username=
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=create-drop
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.format_sql=true
```
* As we are using postgreSQL, the default port is 5432
* if you are using postgres app, then username password will not be required, else you have to provide it
* ```jpa.hibernate.ddl-auto=create-drop``` means we will have a clean sate everytime we run the application
* The master password of your postgresql is "tannu" or may be TLT@#3(complete words in small letter)


## B. Connection to Database
* How to setup postgreSQL in full detail - https://www.sqlshack.com/how-to-install-postgresql-on-windows/
* this got generated while creating a DB
```SQL
CREATE DATABASE student
    WITH
    OWNER = postgres
    TEMPLATE = postgres
    ENCODING = 'UTF8'
    TABLESPACE = pg_default
    CONNECTION LIMIT = -1
    IS_TEMPLATE = False;
```
* Now you can also use SQL Shell, as it gets automatically downloaded with pgAdmin, do the following settings and you are good to go
![image](https://user-images.githubusercontent.com/42698268/223468330-5e8cf6fd-8098-4924-b562-2b1de380d7b3.png)

![image](https://user-images.githubusercontent.com/42698268/223470639-20fcea5e-736e-4775-ab34-1cf7efef43f8.png)

* Now we are done with the setup of postgresql, and we have granted all the permissions
* now go to the pom file and uncomment the jpa and postgresql dependency
* now run the code, you can see that now you are connected with the DB
* But we haven't got any table created in the database

## C. JPA and @Entity
* Now what we need to do is to take the student details and using spring data jpa we are going to add them to the database by creating a table inside a db and then perform a crud operation against our database
* Now let us add @Entity for hibrnate and @Table for table in database


### 1. @Entity
* javax.persistence.Entity: Specifies that the class is an entity. This annotation can be applied on Class, Interface of Enums.

```java
import javax.persistence.Entity;

@Entity
public class Employee implements Serializable {
}
```

### 2. @Table
It specifies the table in the database with which this entity is mapped. In the example below the data will be stores in the “employee” table. Name attribute of @Table annotation is used to specify the table name.

```java
import javax.persistence.Entity;
import javax.persistence.Table;

@Entity
@Table(name = "employee")
public class Employee implements Serializable {
}
```

### 3. @Column
Specify the column mapping using @Column annotation. Name attribute of this annotation is used for specifying the table’s column name.

```java
import javax.persistence.Column;
import javax.persistence.Entity;
import javax.persistence.Table;

@Entity
@Table(name = "employee")
public class Employee implements Serializable {
 
  @Column(name = "employee_name")
  private String employeeName;
}
```

### 4. @Id
This annotation specifies the primary key of the entity.

```java
import javax.persistence.*;

@Entity
@Table(name = "employee")
public class Employee implements Serializable { 
  @Id
  @Column(name = "id")
  private int id;
}
```

### 5. @SequenceGenerator

The @SequenceGenerator annotation defines a primary key generator that may be referenced by name when a generator element is specified for the GeneratedValue annotation.A sequence generator may be specified on the entity class or on the primary key field or property.

* Target: Type, Method and Field
* Uses:@SequenceGenerator
* Argument:
	* name (Required): A unique generator name that can be referenced by one or more classes to be the generator for primary key values.
	* sequenceName (Optional): The name of the database sequence object from which to obtain primary key values.
	* initialValue (Optional): The value from which the sequence object is to start generating.
	* allocationSize (Optional): The amount to increment by when allocating sequence numbers from the sequence.


```java
import javax.persistence.*;

@Entity
@Table(name = "employee")
public class Employee implements Serializable {
  
  @Id
  @Column(name = "id")
  @GeneratedValue(strategy=SEQUENCE, generator="ID_SEQ")
  private int id;
}
```
### 6. @GeneratedValue

The @GeneratedValue consider the entry point for primary key generation, it provides the specification of generation strategies for the values of primary keys. The GeneratedValue annotation may be applied to a primary key property of field of an entity or mapped superclass  in a conjunction with the Id annotation. The values that can be used with the @GeneratedValue are those values defined inside the enum GenerationType. GenerationType.java

``` public enum GenerationType {TABLE,SEQUENCE,IDENTITY,AUTO};```

* TABLE: Is a generator type value indicates that the must assign primary keys for the entity using a Database Table to ensure uniqueness.
* SEQUENCE & IDENTITY: Are a generator types that specify the use of a database sequence or identity column respectively.
* AUTO: Is a generator type indicates that the persistence provider should select an appropriate strategy for the particular database.
### Anatomy of @GeneratedValue
* Target: Field and Method
* Uses:@GeneratedValue
* Argument:
	1. strategy(Optional): The primary key generation strategy that the persistence provider must use to generate the annotated entity primary key.
	2. generator (Optional): The name of the primary generator to use as specified in the SequenceGenerator or TableGenerator.

![image](https://user-images.githubusercontent.com/42698268/224113982-39938a29-41bf-468d-879c-f8d9c4acb370.png)

* Now we have mapped this student class to a table in our database

### For more details, you can visit this [site](https://www.digitalocean.com/community/tutorials/jpa-hibernate-annotations)


## D. JPA in Action

![image](https://user-images.githubusercontent.com/42698268/224539418-00f2800f-ac61-436a-8112-ff34b820b0e7.png)

* Let us connect to the postgreSQl and run the code and now check these commands in shell
![image](https://user-images.githubusercontent.com/42698268/224538509-f6bad6e6-c0da-400d-a0d3-05f046d55f75.png)
* we can see that we have created a table in student database in intellij
* We took a class and map that class to a table in database

## E. Data Access layer
* Now we are connected to the database, but the data access layer is missing 
* so let us create an interface called StudentRepository
* You can see the naming convention which is including ```Repository```, we are going to use this whenever we will be using JPA, and here we are
* Now let us extend this StudentRepository with JpaRepository
* now we have to pass generics as the type on which we are going to work upon and the type of the primary key, so we will pass Student and Id
* Now let us annotate the interface with @Repository as this is going to work as a data access layer
* Now this is all for this layer, now let us connect everything using dependency injection as we want to use this interface inside of our service
* inject the repo and define constructor and Autowire it and then instead of returning the static list, try to return the data using the method of jpaRepo

![image](https://user-images.githubusercontent.com/42698268/224544725-dafaba53-2b43-4151-86a0-e61079e73089.png)
* Now we will add data of few students to this repository

## F. Saving students data to database
* After saving students data to the database, we will see that everything starts working, from api layer, to service layer, to data access layer to db, everything.
* First of all, run the code before adding data and see what it will give
* ![image](https://user-images.githubusercontent.com/42698268/224545340-b297317c-276b-499e-af18-9f72dfe55472.png)
* it will give you an empty list
* Now let us run the query on shell and we can see that it is also showing 0 rows 
* ![image](https://user-images.githubusercontent.com/42698268/224545991-93e00f1e-85cf-4531-a2a0-4c28b73ba0ab.png)
* Now let us add some student into the database, for that we have to create one configuration class called StudentConfig 
* The @Configuration annotation indicates that the class is a source of bean definitions. We can also add it to multiple configuration classes.

* Configuration class:
```java
package com.example.demo.student;

import org.springframework.boot.CommandLineRunner;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

import java.time.LocalDate;
import java.time.Month;
import java.util.List;

import static java.util.Calendar.JANUARY;

@Configuration
public class StudentConfig {

    @Bean
    CommandLineRunner commandLineRunner(StudentRepository repository){
        return args -> {
           Student mariam = new Student(
                    "Mariam",
                    "mariam.jamal@gmail.com",
                    LocalDate.of(1998, Month.JANUARY, 11),
                    23
            );

            Student alex = new Student(
                    "Alex",
                    "alex@gmail.com",
                    LocalDate.of(1999, Month.FEBRUARY, 10),
                    23
            );
            repository.saveAll(List.of(mariam, alex));
        };
    }
}
```
* We have added data of the two students and saved them, now you can see both on browser and shell
* ![image](https://user-images.githubusercontent.com/42698268/224550661-e8fe8d2b-dbff-49ff-a520-826084223a22.png)
* ![image](https://user-images.githubusercontent.com/42698268/224550667-31240375-b42c-4884-adc6-acf22a02418f.png)

### 1. @Transient
@Transient annotation is used to mark a field to be transient for the mapping framework, which means the field marked with @Transient is ignored by mapping framework and the field not mapped to any database column (in RDBMS) or Document property (in NOSQL).
* Now we don't want to store age in db, as it can be calculated so we will mark it as @Transient, so we will remove age from student.java class and then from configuration class
* now we have to set the age by calculation it usin gdob, we will do it in student.java class in getter method i.e getAge method

```java
public Integer getAge() {
        return Period.between(this.dob, LocalDate.now()).getYears();
    }
```
* Now we can see that there is no field as age in our db
![image](https://user-images.githubusercontent.com/42698268/227465054-a2a6c877-12d9-4b05-aaf0-a3f3185ac6a3.png)

# 10. Coming back to the API layer
## Let us create POST, PUT and DELETE mapping



### A. @PostMapping
* Post mapping is used when we want to add new resources in our system, in our case when we want to add new student in our system
![image](https://user-images.githubusercontent.com/42698268/227466228-20d09d13-02b5-476e-b0ca-712d3cb17677.png)

* for post request, let us send above payload to our server and let us see if this email exists or not
* if it does not exists, then we will save it to the database
* if it does, then we are going to throw an exception
* Now let us got to the controller and implement that api which is going to take the payload and store it in our system

```java
 @PostMapping
    public void registerNewStudent(@RequestBody Student student){
        studentService.addNewStudent(student);
    }
```
* Now open the postman and post the message
* ![image](https://user-images.githubusercontent.com/42698268/227583352-0861759d-6ea1-4859-a4d3-817204dffc1d.png)

* you'll get something like this on your intellij console
* ![image](https://user-images.githubusercontent.com/42698268/227583490-a03cf0c5-4f69-436f-bd8d-857fd30af831.png)
* Here i was stuck for 2 hours because, i was posting wrong message having first name and last name(LOL)
* 




































