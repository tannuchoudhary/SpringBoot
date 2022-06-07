
#  API
![Screenshot from 2022-04-23 23-18-29](https://user-images.githubusercontent.com/42698268/164937909-d6ac8c6c-d7c8-4b40-8396-2d830f26b574.png)


![Screenshot from 2022-04-23 23-18-41](https://user-images.githubusercontent.com/42698268/164937940-0c8b1bd2-65f4-4db2-a9cd-f0bf73770838.png)

# REST API
![Screenshot from 2022-04-23 23-30-28](https://user-images.githubusercontent.com/42698268/164937967-0e0fd0d5-4a14-4ca7-8d84-ee073744b829.png)



![Screenshot from 2022-04-23 23-30-55](https://user-images.githubusercontent.com/42698268/164937998-236895b3-96ce-4530-accc-92ec0477b44a.png)


![Screenshot from 2022-04-23 23-31-48](https://user-images.githubusercontent.com/42698268/164938031-11a85172-01b0-44aa-8d4d-8b13d301fd6f.png)


![Screenshot from 2022-04-23 23-33-03](https://user-images.githubusercontent.com/42698268/164938090-5babaf1e-aba6-4d33-ac6a-b84922c1ec47.png)

![Screenshot from 2022-04-23 23-33-19](https://user-images.githubusercontent.com/42698268/164938118-82a7f19f-d650-44ae-8f48-349974b6e16a.png)

![Screenshot from 2022-04-23 23-33-46](https://user-images.githubusercontent.com/42698268/164938152-890f1bf2-c3c6-49fc-8df3-3dec6373973a.png)

#  Three tier architecture

![Screenshot from 2022-04-24 00-17-31](https://user-images.githubusercontent.com/42698268/164949972-725984cf-b2ba-453e-b05b-c4e7145dfdfd.png)
* In controller we call a service and in service we call a DAO or repository
* In spring base applications, we inject service class or service interface in controller and we call service class methods in a controller and then in service class we inject DAO or repository and then we call DAO or repository methods in a service class.
* These three layers are independent to each other and we inject the dependencies and call its methods

# Step 1 - Create Spring boot Project
* You can use spring Initializr or eclipse STS(Spring Tool Suite)
* Create a dummy project and generate itfrom spring initializr
* Import it to eclipse IDE

# Step 2- Create Packaging structure

![Screenshot from 2022-05-31 11-18-52](https://user-images.githubusercontent.com/42698268/172036978-8bac93a1-d54a-4e13-aaef-ee33dd708b23.png)

# Step 3 - Configure MySQL Workbench



### To enter into mysql
``` mysql -u username -p ``` 

Now enter ```Password```

### To create a database
``` CREATE DATABASE db_name ```

### To enter into database
``` USE db_name ```

### To create table
``` CREATE TABLE table_name(id int, name varchar(30), email varchar(30)); ```

### To delete the whole table from database
``` DROP TABLE table_name ```

### To view all tables in a DB
```SHOW TABLES```

### To view content of the table
``` SELECT * FROM tableName ```

### To describe table
``` DESCRIBE tableName ```
* Field – Indicates column name.
* Type – Specifies data type for the column (varchar for characters, int for numbers).
* Null – Indicates whether the column can remain with null values.
* Key – Displays the primary column.
* Default – Displays the column’s default value.
* Extra – Indicates additional information about the columns.


![Screenshot from 2022-06-05 12-47-32](https://user-images.githubusercontent.com/42698268/172040046-7426aee5-84b6-4ac0-92f8-d02377f50479.png)


# Step 4- Setting application.properties

```python3
# this is to connect the jdbc to mysql database,
# we will provide port no for mysql which is generally 3306
# followed by name of database which is movies in our case
# we will provide a property to turn ssl(secure socket layer) off

# SSL stands for Secure Sockets Layer and, in short, it's the standard technology for keeping an 
# internet connection secure and safeguarding any sensitive data that is being sent between two systems,
# preventing criminals from reading and modifying any information transferred, including potential 
# personal details

spring.datasource.url=jdbc:mysql://localhost:3306/ems?useSSL=false

spring.datasource.username=tannu
spring.datasource.password=Tannu@#3


# HIBERNATE PROPERTIES


# This is the property to configure hibernate dialect
# this is the dialect which hibernate requires to generate database queries
#if you are using postgresql database then you have to use postgresql hibernate
# hibernate needs a dialect to generate database vendor specific sql queries
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5InnoDBDialect

# create, create-drop
# we are configuring one more property i.e hibernate auto ddl,

# this property is needed to automatically create the tables in a database if they do not exist and to
# update the existing table
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.show_sql=true
spring.jpa.properties.hibernate.format_sql=true
```
# Step 5- Run your spring boot project and check whether it is working or not

# Step 6- Create Employee [JPA Entity](https://www.baeldung.com/jpa-entities#:~:text=Entities%20in%20JPA%20are%20nothing,a%20row%20in%20the%20table.) for employee

![Screenshot from 2022-05-28 14-16-41](https://user-images.githubusercontent.com/42698268/171099023-ce327121-0e61-4d9d-a249-78170598202b.png)

![Screenshot from 2022-05-31 10-51-18](https://user-images.githubusercontent.com/42698268/171099028-f7accdd0-a420-456d-a1f8-13a3e8c55a1b.png)

![Screenshot from 2022-05-31 10-51-34](https://user-images.githubusercontent.com/42698268/171099037-dbbbcc0b-449f-4819-b58d-19ee92ab9e67.png)

* Go to net.javaguides.springboot.model
* Create a class Employee
* Mention Employee entities inside a class

![Screenshot from 2022-05-31 11-23-55](https://user-images.githubusercontent.com/42698268/172037254-94b43277-5bc0-467c-acab-79f26792d4d5.png)


## @Data 
* @Data is a lombok annotation 
* Lombok is a very useful java library
* It internally uses free annotations to generate required methods

![Screenshot from 2022-05-31 11-24-49](https://user-images.githubusercontent.com/42698268/172037380-6bd0c53a-7fec-409d-84c3-ac09c4ddb9e7.png)

* Now we can see that Employee is a simple java class, we need to make this java class as JPA entity, for that we are going to use JPA annotation

## @Entity
* Use @Entity annotation from javax.persistence package
* Now the Employee entity becomes JPA entity

![Screenshot from 2022-05-31 11-36-48](https://user-images.githubusercontent.com/42698268/172037505-40b50bce-f308-41d1-8dc3-c3bd1280de16.png)

## @Table
* We provide table name using @Table annotation
* @Table has a property called name, which help us to provide the name for the table 
* If you don't provide @Table annotation then JPA is smart enough to provide table name as the name of the class, which is "Employee" in this case

![Screenshot from 2022-05-31 11-40-46](https://user-images.githubusercontent.com/42698268/172037675-4d4d2cf0-593e-4e7d-bede-05a0c307dab1.png)

![Screenshot from 2022-05-31 11-41-22](https://user-images.githubusercontent.com/42698268/172037985-85f90a64-4b8b-4139-9c28-3d04164361d4.png)


## @Id
* @Id annotation is used to define the primary key 
*  make sure that you choose Id from javax.persistence package
  

![Screenshot from 2022-05-31 11-57-32](https://user-images.githubusercontent.com/42698268/172037991-25862375-916f-4aab-8b59-abf39577fe34.png)

* Once we get a primary key, we need to generate a primary key generation strategy for that we will use @GenerateValue

## @GeneratedValue
* Used to generate a primary key generation strategy

![Screenshot from 2022-05-31 11-59-54](https://user-images.githubusercontent.com/42698268/172038771-4e972dfa-6e41-45e8-9ddd-fa58e2abe958.png)

## @Column
* After defining primary keys, we can define column details using JPA annotations
* You can define column name and the attribute as not nullable by nullable=false

![Screenshot from 2022-05-31 12-01-48](https://user-images.githubusercontent.com/42698268/172038802-c0a828ed-5151-49ef-b267-6e89561fe8af.png)

# Step 7- Run your spring boot application
* Run your spring boot application and check whether an Employee table gets created or not
* Hibernate will automatically generate this table because we have added ddl auto property in application.properties
* Now Employee JPA entity is successfully created


# Step 8- Create EmployeeRepository Interface

* we want it because we need to perform CRUD operation on employee jpa repository
* Create an interface in net.javaguides.springboot.repository named EmployeeRepository
* We will extend this interface to JpaRepository
* JpaRepository will require two parameters, first is the type of the enitity which is Employee in our case and second is the type of the primary key i.e long in our case
* Now EmployeeRepository will get CRUD methods for employee JPA entity
* Here we don't need to add @Repository annotation to our EmployeeRepository interface because JpaRepository internally provides @Repository annotation, i.e SimpleJpaRepository provides @Repository annotation internally
* We also don't need to add @Transactional annotation in service layer because SimpleJpaRepository provides @Transactional annotation internally


![Screenshot from 2022-06-05 13-05-35](https://user-images.githubusercontent.com/42698268/172040635-b2e0d604-2389-4b0e-b3b5-fbbd96ad75de.png)


![Screenshot from 2022-06-05 13-07-01](https://user-images.githubusercontent.com/42698268/172040642-2f8732aa-9b58-4c1c-8c89-9c9da7776d01.png)
* Before building REST APIs, first we will create some exception classes 

# Step 9- Create Custom Exceptions
* Create ResourceNotFoundException class inside exception package
* This is to handle the exception if exception occurs
* Now define the properties for this exception class
* resourceName - we are going to return the resource name that is not exising in the database to the client, similarly the fieldName and fieldvalue
* filedValue will be defined as object type, because fieldValue can be of any type


![Screenshot from 2022-06-05 13-41-17](https://user-images.githubusercontent.com/42698268/172041718-08948bd3-8711-4b77-bb6d-c3c045c2dc4b.png)


* Now we will extend our exception class from RuntimeException
* And then we will generate constructors for all the fields mentioned in the ResourceNotFoundException class
* Right click->source->Generate constructors using fields->select all fields ->Generate
* Now pass message to the super class constructor, e.g

``` super.(String.format("%s not found with %s : '%s'", resourceName, fieldName, fieldValue));```
* generate getters for all the field values
* Now we have forgotten to add serialId, so add ``` private static final long serialVersionUID=1L; ```
* @Response status annotation can be used on the top of the REST API, but instead of repeating this annotation for each and every REST API that returns status, we will use it above the exception class itself



![Screenshot from 2022-06-06 12-33-45](https://user-images.githubusercontent.com/42698268/172112097-c90f6363-c4fa-419e-ae6d-143c29d684ab.png)




* ```@ResponseStatus(value = HttpStatus.NOT_FOUND)```, whenever our REST API throw ResourceNotFoundException then REST API will send NOT_FOUND status to the client.

# Step 10- Build Create Employee REST API
* To save the data into employees table
* To do that, first we are going to implement service layer because controller layer is dependent on service layer
* Create a package net.javaguides.springboot.service and an interface EmployeeService inside it
* To implement it, create a class in service.impl called EmployeeServiceImpl 
* Now implement the EmployeeService interface
* Whenever you add service class make sure to add @Service annotation
* make sure to choose @Service annotation from org.springframework.stereotype.Service
* declare saveEmployee() method in the EmployeeService interface, and define it in the impl class, it will save the employee information in database
![Screenshot from 2022-06-07 12-39-49](https://user-images.githubusercontent.com/42698268/172318139-a7c436ae-d2fe-44ad-bebb-13a4e7a93c22.png)
* Go to the impl class and click on add unimplemented methods 
![Screenshot from 2022-06-07 12-39-27](https://user-images.githubusercontent.com/42698268/172318164-91481979-c097-42ed-ba00-98b3177f30a6.png)
```diff
- Before implementing this method, we need to inject dependency, i.e EmployeeService dependency

```


![Screenshot from 2022-06-07 12-41-48](https://user-images.githubusercontent.com/42698268/172318512-d8399f34-abcf-4f6d-b58b-56819404d42e.png)

* We use constructor-based dependency injection when we have mandatory parameters
* And we use setter-based dependency injection when we have optional parameters
* As we are going to use EmployeeRepository as mandatory so we are going to choose constructor-based dependency injection



![Screenshot from 2022-06-07 12-51-58](https://user-images.githubusercontent.com/42698268/172322042-cf05a2c9-e325-4990-9ea1-880c7d7e8aa2.png)



![Screenshot from 2022-06-07 13-01-25](https://user-images.githubusercontent.com/42698268/172322057-0e0a995e-7358-496b-8854-cb81fc12f340.png)

* Whenever spring bean finds only one constructor therefore the spring automatically configures it, we don't need to write @Autowire annotation 

### 3 Important things are:
1. You don't need to add @Repository annotation for EmployeeRepository interface as spring data JPA has already taken care of it by adding it in its declaration
2. You don't need to add @Transaction in impl file above EmployeeServiceImpl class as spring data JPA internally provides transactions to all its methods
3. We don't need to provide @Autowire annotation to the constructor in the impl file whenever spring boot finds spring bean, it has only one constructor then it autowires the dependency 

* Now we will use employeeRepository and its method save and save employee entity to the database
* Now let us create a controller class called EmployeeController
* Use @RestController, @RestController = @Controller + @ResponseBody

![Screenshot from 2022-06-07 13-15-04](https://user-images.githubusercontent.com/42698268/172325607-31b5b981-34f5-4d30-90d6-9f394aac8d4d.png)

```diff
- Now inject EmployeeService dependency into the EmployeeController class
```

![Screenshot from 2022-06-07 13-26-11](https://user-images.githubusercontent.com/42698268/172327300-861a0c50-229e-4ec7-9a9d-e32abb861f31.png)

* We will use constructor-based dependency injection
* Now we will generate Response for the REST API
* For that we will use ResponseEntity, beacuse we can provide complete reponse details in that class
* We will use @PostMapping annotatation as this will handle post http request
* This post request contains employee json object and that we need to bind to the java object i.eemployee object













