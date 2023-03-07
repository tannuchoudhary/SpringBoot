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
# Controller layer
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
