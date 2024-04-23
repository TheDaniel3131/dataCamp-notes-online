---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-data-science/chapter-2/","noteIcon":"","created":"2024-04-23T16:22:07.830+08:00","updated":"2024-04-23T21:04:44.911+08:00"}
---

# Data Collection & Storage
## Lesson 1 - Data Sources

Hi, I'm Sara! Welcome back. Previously, you learned about the data science workflow. In this chapter, we'll focus on the first step: data collection and storage.

## 2. The data science workflow

00:13 - 00:22

Before we can start deriving insights from data, we first need to collect the data from different sources. That's what we'll talk about in this video.

## 3. Sources of data

00:22 - 01:02

We are generating vast amounts of data on a daily basis simply by surfing the internet, tracking a run, or paying by card in a shop. The companies behind these services that we use, collect this data internally. They use this to help them make data-driven decisions. On the other hand, there are also many free, open data sources available. This means the data can be freely used, shared and built-on by anyone. Note that sometimes companies share parts of their data with a wider public as well. Let's first take a look at company data sources.

## 4. Company data

01:02 - 01:15

Some of the most common company sources of data are web events, survey data, customer data, logistics data, and financial transactions. Let's dive a bit deeper into web data.

## 5. Web data

01:15 - 01:45

When you visit a web page or click on a link, usually this information is tracked by companies in order to calculate conversion rates or monitor the popularity of different pieces of content. The following information is captured: the name of the event, which could mean the URL of the page visited or an identifier for the element that was clicked, the timestamp of the event, and an identifier for the user that performed the action.

## 6. Survey data

01:45 - 01:58

Data can also be collected by asking people for their opinions in surveys. This can be, for example, in the form of a face-to-face interview, online questionnaire, or a focus group.

## 7. Net Promoter Score

01:58 - 02:14

You've likely answered a question as shown in the image before. This is a very common type of survey data used by companies: the Net Promoter Score, or NPS, which asks how likely a user is to recommend a product to a friend or colleague.

## 8. Open data

02:14 - 02:22

There are multiple ways to access open data. Two of them are APIs and public records.

## 9. Public data APIs

02:22 - 02:47

Let's begin with APIs. API stands for Application Programming Interface. It's an easy way of requesting data from a third party over the internet. Many companies have public APIs to let anyone access their data. Some noteable APIs include Twitter, Wikipedia, Yahoo! Finance, and Google Maps, but there are many, many more.

## 10. Tracking a hashtag

02:47 - 03:28

Let's look at an example of the Twitter API. Suppose we want to track Tweets with the hashtag DataFramed, DataCamp's wonderful podcast on Data Science. We can use the Twitter API to request all Tweets with this hashtag. At this point, we have many options for analysis. We could perform a sentiment analysis on the text of each Tweet and get an idea of how people like our podcast. We could simply track how often hashtag DataFramed appears each week. We could also combine this data with our downloads data and see if positive Tweets are correlated with more downloads.

## 11. Public records

03:28 - 04:08

Public records are another great way of gathering data. They can be collected and shared by international organizations like the World Bank, the UN, or the WTO, national statistical offices, who use census and survey data, or government agencies, who make information about for example the weather, environment or population publicly available. For example, in the US, data-dot-gov has health, education, and commerce data available for free download. In the EU, data-dot-europa-dot-eu has similar data.

## 12. Let's practice!

04:08 - 04:17

You now know some common sources of data that can be used when working on a Data Science project, let's practice!

![Pasted image 20240423172158.png](/img/user/Pasted%20image%2020240423172158.png)

![Pasted image 20240423172213.png](/img/user/Pasted%20image%2020240423172213.png)

## Lesson 2 - Data types

## 1. Data types

00:00 - 00:09

You now know where to collect data. But what does that data look like? In this video we'll talk about the different types of data.

## 2. Why care about data types?

00:09 - 00:45

You might wonder why it's important to know what type of data you have collected. This will be essential later on in the data science process. For instance, it's especially relevant when you want to store the data, which we'll talk about in the next video as not all types of data can be stored in the same place. Furthermore, when you're visualizing or analyzing the data it's important to know the type of data you are dealing with. Not all visualizations or analyses can be performed with all data types. So, let's dive in.

## 3. Quantitative vs qualitative data

00:45 - 01:15

There are two general types of data: qualitative and quantitative data. It’s important to understand the key differences between both. 

```
Quantitative data can be counted, measured, and expressed using numbers. 

Qualitative data is descriptive and conceptual. Qualitative data can be observed but not measured. 
```

Now that we know the differences, let’s dive into each type of data with a real-world example.

## 4. Quantitative data

01:15 - 01:27

Quantitative data can be expressed in numbers. For example, the fridge is 60 inches tall, has two apples in it, and costs 1000 dollars.

## 5. Qualitative data

01:27 - 01:40

Qualitative data, on the other hand, are things that can be observed but not measured like: the fridge is red, was built in Italy, and might need to be cleaned out because it smells like fish.

## 6. Other data types

01:40 - 02:12

Other than the traditional quantitative and qualitative data, there are many other data types that are becoming more and more important. There is image data, text data, geospatial data, network data, and many more. Note that these other data types aren't mutually exclusive with quantitative and qualitative data. Meaning often these other data types are a special mix of quantitative and qualitative data. Let's look at some examples.

## 7. Other data types: Image data

02:12 - 02:31

Digital images are everywhere. An image is made up of pixels. These pixels contain information about color and intensity. Typically, the pixels are stored in computer memory. In the example you can see that if we zoom in on the image we can distinguish the different pixels.

## 8. Other data types: Text data

02:31 - 02:49

Emails, documents, reviews, social media posts, and so on. As you can imagine, text data can be found in many places. This data can be stored and analyzed to find relevant insights. On the slide, you can see an example of a restaurant review.

## 9. Other data types: Geospatial data

02:49 - 03:13

Geospatial data are data with location information. In the example you can see that many different types of information can be captured using geospatial data. For a specific region we can keep track of where the roads, the buildings, and vegetation are. This is especially useful for navigation apps like Waze and Google maps.

## 10. Other data types: Network data

03:13 - 03:30

Network data consists of the people or things in a network, depicted by circles on the slide, and the relationships between them, depicted by lines on the slide. Here you can see an example of a social network. You can easily see who knows whom.

## 11. Recap

03:30 - 03:52

In this video we looked at the most common data types: quantitative data, qualitative data, image data, text data, geospatial data, and network data. These can all serve as inputs for your data science analysis. But before doing that, the data needs to be stored. That's what we'll cover in the next video.

## 12. Let's practice!

03:52 - 04:01

But first, let's see if you know the difference between the different types of data. Let's practice!

![Pasted image 20240423174958.png](/img/user/Pasted%20image%2020240423174958.png)

![Pasted image 20240423183749.png](/img/user/Pasted%20image%2020240423183749.png)

![Pasted image 20240423183828.png](/img/user/Pasted%20image%2020240423183828.png)


## Lesson 3 - Data storage and retrieval

## 1. Data storage and retrieval

00:00 - 00:00

Previously in this chapter, you learned about different data sources and data types.

## 2. The data science workflow

00:00 - 00:00

Now, let's discuss efficient ways of storing and retrieving the data that was collected. As you can see this is still part of the first step in the data science workflow we defined before.

## 3. Things to consider when storing data

00:00 - 00:00

When storing data there are multiple things to take into consideration. First, we need to determine where we want to store the data. Then, we need to know what kind of data we are storing. And lastly, we need to consider how we can retrieve our data from storage. Let's take a closer look.

## 4. Location: Parallel storage solutions

00:00 - 00:00

Data science projects could require large amounts of data. At this point the data probably can't be stored on a single computer anymore. In order to make sure that all data is saved and easy to access, it is stored across many different computers. Large companies often have their own set of storage computers, called a “cluster” or a “server”, on premises.

## 5. Location: The cloud

00:00 - 00:00

Alternatively, you could pay another company to store data for you. This is referred to as “cloud storage”. Common cloud storage providers include Microsoft Azure, Amazon Web Services, or AWS, and Google Cloud. These services provide more than just data storage; they can also help your organization with data analytics, machine learning, and deep learning. For now, we’ll just focus on data storage.

## 6. Types of data storage

00:00 - 00:00

Different types of data require different storage solutions. Some data is unstructured, like email, text, video and audio files, web pages, and social media messages. This type of data is often stored in a type of database called a Document Database.

## 7. Types of data storage

00:00 - 00:00

More commonly, data can be expressed as tables of information, like what you might find in a spreadsheet. A database that stores information in tables is called a Relational Database. Both of these types of databases can be found on the cloud storage providers that were mentioned earlier.

## 8. Retrieval: Data querying

00:00 - 00:00

Once data has been stored in a Document Database or a Relational Database, we’ll need to access it. At a basic level, we’ll want to be able to request a specific piece of data, such as “All of the images that were created on March 3rd” or “All of the customer addresses in Montana”. In addition, we might even want to do some analysis, such as summing, counting, or averaging data.

## 9. Retrieval: Data querying

00:00 - 00:00

Each type of database has its own query language; Document Databases mainly use NoSQL, while Relational Databases mainly use SQL. SQL stands for “Structured Query Language” and NoSQL stands for “Not only SQL”.

## 10. Putting it all together: Location

00:00 - 00:00

Storing your data is like building a library. First, you need to decide where to build your library. That corresponds to choosing a location: either an on-premises cluster or one of the cloud providers we discussed before: Azure, AWS, or Google Cloud.

## 11. Putting it all together: Data type

00:00 - 00:00

Next, you need to decide what types of shelves to install to store your books. The types of shelves will depend on the types of books.

## 12. Putting it all together: Data type

00:00 - 00:00

This is analogous to choosing between a Document Database for unstructured data or a Relational Database for tabular data. Just like a library might have multiple types of shelves, you might need to have some data stored in a Document Database and other data stored in a Relational Database.

## 13. Putting it all together: Queries

00:00 - 00:00

Finally, you’ll need a system for referencing and checking out books. The way you locate and retrieve each book depends on how that book is stored.

## 14. Putting it all together: Queries

00:00 - 00:00

Similarly, you need a query language to speak to the database. For Document Databases, we generally use NoSQL, and for Relational Databases, we generally use SQL.

## 15. Let's practice!

00:00 - 00:00

Now that you understand different ways of storing data, let’s practice!

![Pasted image 20240423185039.png](/img/user/Pasted%20image%2020240423185039.png)

![Pasted image 20240423185120.png](/img/user/Pasted%20image%2020240423185120.png)

#### Which type of database?

It's important to understand what type of data you are dealing with because it will affect your storage decision. Some data is tabular and belongs in a **Relational Database**. Some is unstructured and belongs in a **Document Database**.

![Pasted image 20240423185254.png](/img/user/Pasted%20image%2020240423185254.png)

## Lesson 4 - Data Pipelines

## 1. Data Pipelines

00:00 - 00:00

Nice job so far! Let's learn about data pipelines. So far we've learned about data collection and storage, but how can we scale all this? This is where data pipelines come in.

## 2. Data collection and storage

00:00 - 00:00

Data engineers work to collect and store data, so that others, like analysts and data scientists can access data for their work, whether it's for visualization or building machine learning models.

## 3. How do we scale?

00:00 - 00:00

But how do we scale this? Consider the different data sources you learned about - what if we're collecting data from more than one data source? And then, what if these data sources have different types of data? For example, consider real-time streaming data, which is data that is continuously being generated, like tweets from all around the world. This makes storing this incoming data complicated, because as a data engineer, you want to make sure data is organized and easy to access.

## 4. What is a data pipeline?

00:00 - 00:00

Enter the data pipeline. A data pipeline moves data into defined stages, for example, from data ingestion through an API to loading data into a database. A key feature is that pipelines automate this movement. Data is constantly coming in and it would be tedious to ask a data engineer to manually run programs to collect and store data. Instead a data engineer schedules tasks whether it's hourly, daily, or tasks can be triggered by an event. Because of this automation, data pipelines need to be monitored. Luckily, alerts can be generated automatically, for example, when 95% of storage capacity has been reach or if an API is responding with an error. Data pipelines aren't necessary for all data science projects, but they are when working with a lot of data from different sources. There isn't a set way to make a pipeline - pipelines are highly customized depending on your data, storage options, and ultimate usage of the data. ETL, which stands for extract, transform, and load, is a popular framework for data pipelines. Let's explore it with a case study.

## 5. Case study: smart home

00:00 - 00:00

After learning about IoT devices and APIs, you decide to try out both. Specifically, you want to use APIs and devices in your house to better understand the status of your house and neighborhood. You gather a list of data sources and associated information. The first two are provided by APIs. Every 30 minutes, you get the weather conditions, and you get Tweets geotagged in your neighborhood whenever they are published. The remaining rows are IoT devices that send their sensor data over the internet at the specified frequencies.

## 6. Extract

00:00 - 00:00

How does it all come together? First, we begin with extracting all the data from the data sources we listed, whether it's an API or setting up an IoT device. However, a quick look at the frequencies and structures makes us realize that storing the raw data as is won't work.

## 7. Transform

00:00 - 00:00

This is where the transform phase comes in.

## 8. Transform

00:00 - 00:00

In this stage, we transform data to make sure data stays organized so that others can easily find relevant data and use it. A common transformation is joining data from different sources into one dataset. Another is converting the incoming data's structure to fit a database's schema. A database's schema informs us how data must be structured before loading it in. A transformation can also be removing irrelevant data. For example, the Twitter API, not only gives you a tweet but others details, like the number of followers the author has, which is not useful in our scenario, so we shouldn't store it. Data gets altered throughout the data science workflow, it's important to note that analytical tasks like data preparation and exploration don't occur at this stage - we'll see this in chapter 3.

## 9. Load

00:00 - 00:00

Finally, we load the data into storage so that it can be used for visualization and analysis.

## 10. Automation

00:00 - 00:00

Once we've set up all those steps, we automate. For example, we can say every time we get a tweet, we transform it in a certain way and store it in a specific table in our database. There are tools that specialized to do this, the most popular is called Airflow.

## 11. Let's practice!

00:00 - 00:00

Now, it's time for some exercises.

![Pasted image 20240423185753.png](/img/user/Pasted%20image%2020240423185753.png)

#### Extract Transform Load

Tech companies have complex large-scale data pipelines to deal with the huge amount of data coming from millions of users, whether it's incoming social media posts, viewership data of TV episodes, or recent online purchases.

Imagine the data pipeline of a music streaming service. In this exercise, there are several pipeline tasks listed. Classify those tasks within the steps of ETL.

![Pasted image 20240423185925.png](/img/user/Pasted%20image%2020240423185925.png)

