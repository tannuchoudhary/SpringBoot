# Creating REST API using spring boot


![Screenshot from 2022-02-13 21-14-11](https://user-images.githubusercontent.com/42698268/153760978-bf9b3917-f116-42a0-b07b-6aa9740ca518.png)

### SERVER:  where we deploy our application, it consists of various layers

![Screenshot from 2022-02-13 21-16-21](https://user-images.githubusercontent.com/42698268/153761047-bd7aa726-e970-4dd0-a3ba-b90ab2a23486.png)

### CLIENT : Who sends request to the server(e.g mobile phone, browser)

### LAYERS OF SERVER

### 1. Presentation layer {Controllers}

![Screenshot from 2022-02-13 21-13-31](https://user-images.githubusercontent.com/42698268/153761140-b21bca0e-c839-4ea8-b3db-7da84d88c83a.png)


* Controllers are the front-fighters which accepts the request made by client


### 2. Service layer or Business layer


![Screenshot from 2022-02-13 21-26-31](https://user-images.githubusercontent.com/42698268/153761423-8a67220a-d5b4-445d-b285-5cf80bd180c0.png)


* Service layer provides services to our controllers
* Also while doing any work, if it needs any data then it will contact the next layer i.e Repository layer to bring the data(just like chef in the kitchen does not brings raw material from store room but there are persons assigned for this task, he just asks them to bring the material) similarly service layer asks the repository layer to bring the data from database and then repository layer will give the data to service layer.

### 3. DAO(Data Access Object)/Repository Layer
* Brings data from database and gives to service layer

# API URLs for course App

![Screenshot from 2022-02-13 13-10-56](https://user-images.githubusercontent.com/42698268/153766968-0d7b29be-1f82-4708-9d9d-665772d06d3d.png)

* We are going to handle backend, in this project if request would be made then data of courses would be displayed, new courses would be added using these commands

# Coding























 
