# 1. Overview

![Screenshot from 2022-02-06 18-29-23](https://user-images.githubusercontent.com/42698268/153379293-ed8c4265-a90b-473d-9508-4c709301bf65.png)

![Screenshot from 2022-02-06 18-29-49](https://user-images.githubusercontent.com/42698268/153379301-6e9b2eca-956b-42a3-8f91-399ead8b1bf5.png)
what 
# 2. Selecting Dependencies which our project need
* Spring web
* Spring data JPA for connecting through database using JPA and Hybernet
* PostgreSQL Driver : for connecting to real database

![Screenshot from 2022-02-10 15-07-12](https://user-images.githubusercontent.com/42698268/153379538-a64443f4-820f-497e-8e85-49a44709d3ba.png)

![Screenshot from 2022-02-10 15-08-45](https://user-images.githubusercontent.com/42698268/153379781-9329be14-f5c3-40c7-8bcd-3ec1cafeec5c.png)

![Screenshot from 2022-02-10 15-09-10](https://user-images.githubusercontent.com/42698268/153379825-8eda224e-8b9d-46fc-a6cc-3e07ddd73170.png)

# 3. Download and extract selected dependencies

![Screenshot from 2022-02-10 15-14-17](https://user-images.githubusercontent.com/42698268/153380692-b7396d55-2a8b-4b25-881e-17c4a6ea47c1.png)
![Screenshot from 2022-02-10 15-14-04](https://user-images.githubusercontent.com/42698268/153380699-4dd8b245-6326-4c03-b928-cd4ba838c1bb.png)

# 4. Import this project in your IDE

![Screenshot from 2022-02-10 15-15-18](https://user-images.githubusercontent.com/42698268/153380866-1a42193f-6e87-4ba3-8231-3482d5fb3c07.png)

# 5. Starting the server
Run the DemoApplication.java, you will get an error because application will try to connect to the database
* Open pom.xml
* and comment the dependecy of spring-boot-starter-data-jpa
* This dependency will be added back once we are ready to connect it with database

![Screenshot from 2022-02-10 15-25-24](https://user-images.githubusercontent.com/42698268/153382722-6fb7ae9f-25e7-423e-887d-e861ac65311b.png)
* Now run the application
* Open localhost:8080 , you can find your web server running on this port and it will have nothing as we haven't implemented anything


![Screenshot from 2022-02-10 15-26-54](https://user-images.githubusercontent.com/42698268/153383043-da5d2ba6-74d1-49a3-b351-d56636f4987a.png)


# 5. Let us create a simple API


## a.

![Screenshot from 2022-02-10 15-53-55](https://user-images.githubusercontent.com/42698268/153387665-e77de8e8-7c40-4dd5-a333-c73bb9442b9b.png)

![Screenshot from 2022-02-10 15-53-48](https://user-images.githubusercontent.com/42698268/153387743-04f61857-faa3-4011-9eff-6d0a43264bc8.png)


## b. We can see that json is back

![Screenshot from 2022-02-10 15-51-51](https://user-images.githubusercontent.com/42698268/153387247-6c49ceb6-aaf4-4fec-a844-d4ac1fd5c4a5.png)
 
![Screenshot from 2022-02-10 15-51-59](https://user-images.githubusercontent.com/42698268/153387317-89e77448-b61f-4c23-a197-7ec3b77a1b01.png)

