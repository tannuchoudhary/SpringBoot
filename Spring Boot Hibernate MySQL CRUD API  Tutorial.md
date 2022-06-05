
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
















































