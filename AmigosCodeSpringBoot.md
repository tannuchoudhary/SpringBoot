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
 * 
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


## What are APIs used for?
A better question might be what are APIs not used for. Want to embed Instagram photos on your e-commerce app? There’s an API for that. Want to provide instant access to thousands of hotels on your travel blog? There’s an API for that. Want to integrate a Yoda translator on your Star Wars fan fiction site? If you can believe it, there’s an API for it.

Generally speaking, business applications of APIs include:

### 1. Data sharing:
Any time a program needs to get data from a third party (e.g., a travel app compiling flight times from airlines, an e-commerce site getting your payment information from a payment processor), data can be shared through an API.
### 2. App integrations: 
When two digital applications work in conjunction, — HubSpot and Gmail, for example — it's likely that an API is involved.
Embedded content: To embed a piece of content that is not hosted by the same company as the website itself – like a YouTube video or a third-party script like Google Analytics — a request is made to the owner of the embedded content to retrieve it.
### 3. Internal systems:
APIs aren't only for sharing data externally. Businesses frequently divide their software infrastructure into smaller components that communicate with each other through APIs, like in a microservice architecture.
These examples hit upon some of the most common reasons companies use APIs. Below, we dive into more examples of APIs and their business applications.

## API Examples
Without searching an API marketplace, or even knowing much about APIs, you’ve probably heard of a few. Below we’ll look more closely at several examples so you can understand what information and functionality is available through them.

### 1. Twitter APIs
If you work for a brand that loves Twitter, you can use the social media platform’s APIs to drive user engagement on your site.

Twitter has a whole platform offering APIs that allow you to dig through Twitter’s massive archive. You can use Twitter APIs to find old Tweets, embed Tweets and timelines within your website or app, programmatically create and manage ad campaigns, filter and stream Tweets in real time, deliver personalized customer service through direct messages, subscribe to the real-time activities of more than 15 accounts via webhooks, and more.

There’s also a ton of technical resources and tools available to help you harness the full potential of its global communication network.

### 2. Instagram APIs
Instagram’s platform offers a range of APIs to help your business with content publishing, metrics and analysis, and more.

One potential use case is to embed user-generated Instagram photos on your app. User-generated content, sometimes shortened to UGC, is a strong form of social proof that can entice leads to convert.

Developers plug into this platform to build apps and services that target three groups: individuals looking to share their own content with third-party apps; brands and advertisers needing to understand and manage their audience and media rights; and broadcasters and publishers wanting to discover content and get digital rights to media or share it with proper attribution.

### 3. YouTube APIs
YouTube APIs enable you to add a functionality to your site or app and access YouTube’s expansive library of videos.

Let’s walk through just a few reasons you might want to use one of the many YouTube APIs available: to play videos directly in your app; to let users search content, upload videos, and create and manage playlists; to gain insight into how users are interacting with your videos and channel; to schedule live broadcasts; and much more. You’ll need to get a YouTube API key to unlock its potential.

### 4. HubSpot APIs
HubSpot’s platform appeals to businesses with three main needs: those looking to build an app and put it in front of thousands of potential users, those looking to create a custom integration between their app and HubSpot’s application, and those looking to build or extend the functionality of their website.

Gathering data from different transactional software, storing contacts, and engaging with third-party tools and custom apps in one CRM are just a few ways that HubSpot APIs can help your business.

### 5. Spotify Web APIs
If you’re in the music industry, you may want to use the Spotify Web APIs to add music player functionalities to your website or application.

Using Spotify’s multitude of APIs, you can get complete access to the Spotify Data Catalogue, including albums, musical artists, and tracks. To retrieve user-related data such as private playlists, users must authorize your app to access their Spotify accounts.

The functionalities are nearly identical to what you would find on the native Spotify platform. With the Browse API, for example, your users can access genres, categories, new releases, and playlist recommendations. Spotify also offers Episodes, Follow, Library, and Playlists APIs.

Stuck? Spotify published a list of example apps so you can see how their APIs have been used in the past.

### 6. Google Maps APIs
The Google Maps APIs are an essential tool for anyone building a location-based app. If you’re building a real estate app, for example, you can use the Google Maps APIs to include a street view of the property.

The Google platform has an expansive library of APIs with an unlimited amount of uses. Want to allow users to request directions? How about including Places on your website? There’s even an API for you if you’re building a ridesharing app. Google has divided the APIs by usage and platform (web, iOS, or Android), so be sure to choose the correct one for your project.

Like most of the examples listed here, these APIs are paid based on monthly usage. The high level of functionality they offer makes them well worth the price.

### 7. PayPal APIs
The PayPal platform has an expansive library of APIs that you can use to integrate PayPal functionality into your website or app without requiring users to access the PayPal website.

Some APIs that are available to you include the Billing Plans API, the Catalog Products API, the Disputes API, and the familiar Invoicing, Orders, and Payments APIs.

If you’re building an ecommerce website or creating a website for a membership-based organization, the PayPal APIs will help you manage every step of all transactions. Should you ever feel stuck, PayPal has a strong support base where you can access frequently asked questions and procure the help of other developers working on PayPal integration projects.

There is a vast wealth of APIs available today. Some for operating systems, others for websites, and so on, but to fully appreciate their potential in the digital economy, let’s take a closer look at how APIs are classified by who they are shared with and why.

## 3. Types of APIs
APIs can be categorized by their intended audience and scope. There are four main types of APIs that developers work with:

### A. Private APIs: 
These APIs are only made available to a company's internal team in order to boost productivity and transparency. Developers working for the company can use these APIs as needed but third-party developers can’t.
### B. Partner APIs: 
These APIs are shared externally, but only with those who have a business relationship with the company providing the API. Some businesses use partner APIs because they want control over who can access their resources and how those resources get used.
### C. Open APIs:
Open APIs, also known as public APIs, are available for external use. While some open APIs are free, others require a subscription fee to use, which is often tiered based on usage.
### D. Composite APIs: 
These APIs allow you to bundle calls or requests to get one unified response from different servers. If you need data from different applications, you would use a composite API. Or, instead of making five separate API calls in succession, you can make one using a composite API.
For a more detailed explanation, see our guide to the types of APIs.

## 4. Why use an API?
Now that we know that businesses can use APIs to securely request and share content, services, and functionalities with both internal and external audiences, you might be thinking why would a company pay another for access to resources that it could create on its own? Why would that company agree to share its assets, particularly with competitors? Or why would it put in all the work of making an API just so its own workforce could use it?

All good questions. Before we dive into the answers, let’s split up the benefits of APIs into two groups: API consumers and API providers.

* Benefits to API consumers

You may use APIs to request access to another server’s resources or you may use your own APIs to automate certain tasks. Either way, you fall under the mantle of API consumers. These consumers benefit from using each type of API in several ways.

* Productivity

Many companies consume their own APIs. Why? Using APIs internally enables the workforce to streamline operations, foster collaboration, and strengthen transparency across the company. Amazon founder and CEO, Jeff Bezos, understood the vast potential of internal APIs back in 2002 when he sent an email instructing every team to communicate through APIs moving forward. Following what has been coined “The Bezos Mandate,” developers built or turned their well-developed software components into APIs, establishing consistent and well-managed ways of exchanging data and capabilities across the company as a result.

* User Satisfaction

Companies want to provide the best experience for their users. Rarely can one product satisfy and anticipate every need and expectation. That is why they use APIs to extend the functionality of their products. For example, OpenTable uses the Maps JavaScript API to embed an interactive map on its site, making it possible for users to get directions from their homes to nearby restaurants in just a few clicks. If you’re not familiar with the site, check out this screenshot showing an overview of a steakhouse in Indiana.


* Innovation

By allowing developers — whether third-party or internal members of your workforce — to reuse software components, APIs empower them to focus on developing new solutions rather than repeat work that’s already been done. Let’s revisit the example above. Without the Google Maps API, developers at OpenTable would have to dedicate their time and resources to drawing their own map and providing real-time map data to include this feature on its site. Worse still, no matter how much time they put in, it would be nearly impossible to make it as detailed or reliable as Google’s existing solution. So, instead of wasting their time trying to reinvent the wheel, APIs enable developers to focus on creating new tools and functionality that deliver more value to their users.

* Benefits to API Providers

Now that you’re convinced of the benefits of using APIs, let’s turn our attention to why you might want to create and then share one with partners or the general public.

Simply put, becoming an API provider unlocks business opportunities and other benefits that build upon those of simply consuming APIs. Let’s look into each one below.

* Revenue

The easy answer is money. Google, Yelp, Facebook, and thousands of other companies make their APIs public and monetize them so that they become additional lines of revenue. In fact, at some companies, APIs are the major source of revenue. According to a recent report by MuleSoft Inc., 35 percent of today’s technology leaders generated more than a quarter of their organizations’ revenue as a direct result of APIs.

* Scale


By sharing what you do really well with the broadest possible audience, a network of users beyond your employees and customers—including third-party developers and consumers—will become reliant on the data and functionality provided by your APIs. Ultimately, this will improve the usage and adoption of your main platform. In other words, APIs not only expand your customer base, they generate new market opportunities in the digital economy.

Amazon Web Services (AWS) is among the most notable examples. This platform, which essentially allows any company or developer to run its applications on top of Amazon’s technology infrastructure platform via APIs, is used by millions of customers around the world and is credited with transforming Amazon from an online bookstore to a global digital giant.

* Even More Innovation


Yes, I’m listing this again, but with a twist. Above, we discussed how API consumers benefit from using third-party solutions that allow them to focus their time and resources on making their own products better rather than reinventing the wheel.

More often than not, however, the relationship between API consumers and providers is much more give-and-take. You may recall that in the early days of Twitter, its user interface was a little clunky. Then TweetDeck, an independent app at the time, came along and built a better user interface on top of the Twitter platform using its public API so that all users could have better Twitter experiences. That’s called a win-win-win, my friends.

## 5. How to Use an API
So you’re ready to try your luck with APIs. Now what? Before implementing your own API at your company, it makes the most sense to use others' APIs. Let’s walk through the basics of how you’d get started using an API.

1. Select an API.
First things first, you’ll want to find an API you could incorporate into your business. You might already have your eye on an API, particularly if you’re interested in one of the big wigs like the Facebook API. You might also want to search by cost — you may want to start with a free API before exploring paid APIs, for example.

Once you have an API selected, get your reading glasses on. It’s time to look through the API documentation.

2. Get an API key.
As mentioned, an API key is used to identify yourself as a valid client, set access permissions, and record your interactions with the API.

Some APIs make their keys freely available, while others require clients to pay for one. Either way, you’ll most likely need to sign up with the service. You’ll then have a unique identifier assigned to you, which you will include in your calls.

Always key your key private, like you would a password. If your key leaks, a bad actor could make API requests on your behalf. You may be able to void your old key and get a new one if such a breach occurs.

3. Review the API documentation.
API Documentation is essentially an instruction manual about how to effectively use and integrate with an API. In addition to providing all the information required to work with the API, like whether or not you need an API key, it usually includes examples and tutorials.

Refer to the documentation for how to get your key, how to send requests, and which resources you can fetch from its server.

It’s hard to understate the importance of good API documentation — a company might offer a powerful API, but if developers can’t quickly learn how to use it, it’s not very valuable

4. Write a request to an endpoint.
Next up, you’ll write your first request. The easiest method is to use an HTTP client to help structure and send your requests. You’ll still need to understand and get some information from the API’s documentation, but you won’t need much coding knowledge to be successful.

At this stage, online tutorials can come to the rescue. For example, this YouTube video explains how to use an API to pull location data from Google Maps and then use those coordinates to find nearby photos on Instagram.

5. Connect your app.
Now that you understand how to make requests to your API of choice, you can sync your application with it. As a marketer, you don't need to worry about this stage of an API integration. This is the job of a developer, who will employ one or more languages like Python, Java, JavaScript (and NodeJS), PHP, and more.

Chances are, the API you're interacting with is a specific type of API that is considered easier to use than others. These APIs are called REST APIs.

## 6. REST APIs
REST APIs conform to the constraints of a software architectural style called “Representational State Transfer” that make the APIs relatively easy to use and discover. REST makes data and functionality available as resources, which are represented by unique URLs. To request a resource via a REST API, like the Open Weather Map API, you just need to provide its URL.

In a typical REST API, a resource will have two URL patterns assigned to it: a plural (to refer to all the resources) and a singular (to specify a single resource). These are also referred to as endpoints. Can you guess why? Because they go at the end of the URL.

Each endpoint is also assigned a list of actions the client can request of the server. So, a plural endpoint may be for listing or creating resources, and the singular endpoint may be for retrieving, updating, and canceling a specific resource. The client would have to include the correct HTTP verb (GET, POST, PUT, DELETE) in its request to tell the server what action to take.

The client and server can use three data formats to pass this information back and forth:

* HTML (Hypertext Markup Language)
* XML (Extensible Markup Language)
* JSON(JavaScript Object Notation)

### REST API Example
WordPress has a REST API that enables developers to create, read, and update WordPress content remotely by carrying JSON objects back and forth between clients and servers. In other words, by allowing developers to easily structure the way they want to get data into and out of a server, they can spend less time accessing the data they need and more time creating better user experiences.

### REST vs. SOAP
REST is usually put head-to-head with Simple Object Access Protocol (SOAP), another way to build applications that work over HTTP. REST is considered a simpler alternative to SOAP because it requires writing less code to complete tasks and follows a less rigid structure and logic than SOAP. Another reason people love REST: it provides plenty of conventions but leaves many decisions up to the person designing the API.

Here’s a simple test if you’re deciding between REST and SOAP for your API: if you want flexibility, go with REST. If you want standardization, go with SOAP.

The Future of the Digital Economy
There are many business advantages to both consuming and providing an API, but let’s keep it simple. The main reason? To connect your application to the rest of the software world. These connections can empower all types of organizations, from start-ups to government agencies, to create new business models that spur more innovation and ideas in today’s digital economy.

In this way, APIs are not only changing the way companies do business. They’re changing the way companies think about business.


* To read full article click [here](https://blog.hubspot.com/website/application-programming-interface-api?hubs_content=blog.hubspot.com%252Fwebsite%252Ftypes-of-apis&hubs_content-cta=guide%2520to%2520REST%2520APIs#what-are-APIs)


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

