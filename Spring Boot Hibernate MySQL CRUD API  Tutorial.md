

![Screenshot from 2022-04-23 23-18-29](https://user-images.githubusercontent.com/42698268/164937909-d6ac8c6c-d7c8-4b40-8396-2d830f26b574.png)


![Screenshot from 2022-04-23 23-18-41](https://user-images.githubusercontent.com/42698268/164937940-0c8b1bd2-65f4-4db2-a9cd-f0bf73770838.png)

![Screenshot from 2022-04-23 23-30-28](https://user-images.githubusercontent.com/42698268/164937967-0e0fd0d5-4a14-4ca7-8d84-ee073744b829.png)



![Screenshot from 2022-04-23 23-30-55](https://user-images.githubusercontent.com/42698268/164937998-236895b3-96ce-4530-accc-92ec0477b44a.png)


![Screenshot from 2022-04-23 23-31-48](https://user-images.githubusercontent.com/42698268/164938031-11a85172-01b0-44aa-8d4d-8b13d301fd6f.png)


![Screenshot from 2022-04-23 23-33-03](https://user-images.githubusercontent.com/42698268/164938090-5babaf1e-aba6-4d33-ac6a-b84922c1ec47.png)

![Screenshot from 2022-04-23 23-33-19](https://user-images.githubusercontent.com/42698268/164938118-82a7f19f-d650-44ae-8f48-349974b6e16a.png)

![Screenshot from 2022-04-23 23-33-46](https://user-images.githubusercontent.com/42698268/164938152-890f1bf2-c3c6-49fc-8df3-3dec6373973a.png)

# Three tier architecture

![Screenshot from 2022-04-24 00-17-31](https://user-images.githubusercontent.com/42698268/164949972-725984cf-b2ba-453e-b05b-c4e7145dfdfd.png)

# Step 1 - setting application.properties

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
# Create Movies JPA Entity
