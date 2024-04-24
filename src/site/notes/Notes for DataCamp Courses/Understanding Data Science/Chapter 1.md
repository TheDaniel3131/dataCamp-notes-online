---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-data-science/chapter-1/","created":"2024-04-22T13:42:12.207+08:00","updated":"2024-04-23T18:17:24.501+08:00"}
---

# Lesson 1 - Understanding Data Science:

https://campus.datacamp.com/courses/understanding-data-science/introduction-to-data-science-1?ex=1

Transcript:
## 1. What is data science?

00:00 - 00:12

Welcome! My name is Lis. In this course, we'll unpack the what, why, and how of data science. By the end of this course, you'll have a better grasp of how data is being used around you and how you can use data.

## 2. Let's ask Google!

00:12 - 00:17

If we Google "What is data science?", we'll see a huge amount of confusing information.

## 3. Making data work for you

00:17 - 00:38

But data science is actually simple. It's a set of methodologies for taking in thousands of forms of data that are available to us today, and using them to draw meaningful conclusions. Data is being collected all around us. Every like, click, email, credit card swipe, or tweet is a new piece of data that can be used to better describe the present or predict the future.

## 4. What can data do?

00:38 - 01:39

So what can data do? Data can describe our current state, like our energy consumption. This can be accomplished with dashboards or alerts, simplifying time-intensive reporting processes. It can help detect anomalous events, such as fraudulent purchases. If we have data on what has happened previously, we can increase efficiency by automatically detecting a new event that is unexpected or abnormal. Data can also diagnose the causes of observed events and behaviors, for instance your activity on Spotify or Netflix. Rather than determining correlations between small numbers of events, data science techniques help us understand complex systems with many possible causes. Finally, data can predict future events, such as forecasting population size. We can use techniques to take various causes into account and predict potential outcomes. Further, we can evaluate the probability of our prediction mathematically to clarify our level of uncertainty.

## 5. Why now?

01:39 - 01:56

So now we know what data science is. The next question is why is it so popular? The answer is pretty obvious: we're collecting more data than ever before. Suppose that you visit a car dealership and fill out some information.

## 6. Why now?

01:56 - 02:04

All of that data is automatically entered into a computer, and combined with the data from hundreds of dealerships into one big database.

## 7. Why now?

02:04 - 02:40

Once we have that data, it's easy to use the email address that you provided when you bought that car to tie your car purchase data with your data from social media or web browsing. Suddenly, we have a very complete picture about everyone who purchased a car in the last year: their ages, their likes and dislikes, their families, their friends. This additional data can be used to predict what price you can pay for your car, and what other purchases you're likely to make, or how best to sell you insurance for that new car. Data is everywhere, and it's incredibly valuable information for businesses, organizations, and governments.

## 8. The data science workflow

02:40 - 03:01

So, how do we start to use data? In data science, we generally have four steps to any project. First, we collect data from many sources, such as surveys, web traffic results, geo-tagged social media posts, and financial transactions. Once collected, we store that data in a safe and accessible way.

## 9. The data science workflow

03:01 - 03:14

At this point, data is in its raw form, so the next step is to prepare data. This includes "cleaning data", for instance finding missing or duplicate values, and converting data into a more organized format.

## 10. The data science workflow

03:14 - 03:25

Then, we explore and visualize the cleaned data. This could involve building dashboards to track how the data changes over time or performing comparisons between two sets of data.

## 11. The data science workflow

03:25 - 03:38

Finally, we run experiments and predictions on the data. For example, this could involve building a system that forecasts temperature changes or performing a test to find which web page acquires more customers.

## 12. Let's practice!

03:38 - 03:50

Now, you know why data science is important and the first four steps in the data science workflow. Let's explore these themes in some practical exercises.


![Pasted image 20240422134422.png](/img/user/Pasted%20image%2020240422134422.png)

![Pasted image 20240422134529.png](/img/user/Pasted%20image%2020240422134529.png)

# Lesson 2 - Application of Data Science

## 1. Applications of data science

00:00 - 00:10

Previously, you learned the definition of data science and the steps in a data science workflow. In this lesson, you'll learn how data science can be applied to real-world problems.

## 2. More case studies

00:10 - 00:20

Let's take a deep dive into three exciting areas of data science: traditional machine learning, the Internet of Things, and deep learning.

## 3. Case study: fraud detection

00:20 - 00:30

Suppose you work in fraud detection at a large bank. You'd like to use data to determine the probability that the transaction is fake.

## 4. Case study: fraud detection

00:30 - 01:11

To answer this question, you might start by gathering information about each purchase, such as the amount, date, location, purchase type, and card-holder address. You'll need many examples of transactions, including this information, as well as a label that tells you whether each transaction is valid or fraudulent. Luckily, you probably have this information in a database. These records are called "training data", and are used to build an algorithm. Each time a new transaction occurs, you'll give your algorithm information, like amount and date, and it will answer the original question: What is the probability that this transaction is fraudulent?

## 5. What do we need for machine learning?

01:11 - 01:53

Before we can answer that question, let's walk through our example and highlight what we need for machine learning to work its magic. First, a data science problem begins with a well-defined question. Our question was "What is the probability that this transaction is fraudulent?" Next, we need some data to analyze. We have months of old credit card transactions and associated metadata, like date and location, that have already been identified as either fraudulent or valid. Finally, we need additional data every time we want to make a new prediction. We need to have the same type of information on every new purchase so that we could label it as either "fraudulent" or "valid".

## 6. Case study: smart watch

01:53 - 02:29

Now, suppose you're trying to build a smart watch to monitor physical activity. You want to be able to auto-detect different activities, such as walking or running. Your smart watch is equipped with a special sensor, called an "accelerometer", that monitors motion in three dimensions. The data generated by this sensor is the basis of your machine learning problem. You could ask several volunteers to wear your watch and record when they are running or walking. You could then develop an algorithm that recognizes accelerometer data as representing one of those two states: walking or running.

## 7. Internet of Things (IoT)

02:29 - 03:04

Your smart watch is part of a fast growing field called "the Internet of Things", also known as IoT, which is often combined with Data Science. IoT refers to gadgets that are not standard computers, but still have the ability to transmit data. This includes smart watches, internet-connected home security systems, electronic toll collection systems, building energy management systems, and much, much more. IoT data is a great resource for data science projects!

## 8. Case study: image recognition

03:04 - 03:16

Let's tackle another example. A key task for self-driving cars is identifying when an image contains a human. What would be the dataset for this problem?

## 9. Case study: image recognition

03:16 - 03:32

We could express the picture as a matrix of numbers where each number represents a pixel. However, this approach would probably fail if we fed the matrix into a traditional machine learning model. There's simply too much input data!

## 10. Deep learning

03:32 - 04:03

We need more advanced algorithms from a subfield of machine learning called deep learning. In deep learning, multiple layers of mini-algorithms, called "neurons", work together to draw complex conclusions. Deep learning takes much, much more training data than a traditional machine learning model, but is also able to learn relationships that traditional models cannot. Deep learning is used to solve data-intensive problems, such as image classification or language understanding.

## 11. Let's practice!

04:03 - 04:10

You're now familiar with several different applications of Data Science. Let's practice!

#### Assigning data science project

![Pasted image 20240422143038.png](/img/user/Pasted%20image%2020240422143038.png)

![Pasted image 20240422143428.png](/img/user/Pasted%20image%2020240422143428.png)


# Lesson 3 - Data Science Roles & Tools

## 1. Data science roles and tools

00:00 - 00:00

In this lesson, you'll learn about the different data roles and the tools they use.

## 2. Roles in data science

00:00 - 00:00

You might be surprised to learn that there isn't a single job within data science. Generally, there's four jobs: Data Engineer, Data Analyst, Data Scientist, and Machine Learning Scientist. Let's explore each one.

## 3. Data engineer

00:00 - 00:00

Data engineers control the flow of data: they build custom data pipelines and storage systems. They design infrastructure so that data is not only collected, but easy to obtain and process. Within the data science workflow, they focus on the first stage: data collection and storage.

## 4. Data engineering tools

00:00 - 00:00

Data engineers are proficient in SQL, which they use to store and organize data. They also use one of the following programming languages like Java, Scala, or Python to process data. They use Shell on the command line to automate and run tasks. Finally, data engineers, now more than ever, need to be comfortable with cloud computing to ingest and store large amounts of data.

## 5. Data analyst

00:00 - 00:00

Data analysts describe the present via data. They do this by exploring the data and creating visualizations and dashboards. To do these tasks, they often have to clean data first. Analysts have less programming and stats experience than the other roles. Within the workflow, they focus on the middle two stages: data preparation and exploration and visualization.

## 6. Data analyst tools

00:00 - 00:00

Data analysts use SQL, the same language used by data engineers, to query data. While data engineers build and configure SQL storage solutions, analysts use existing databases to retrieve and aggregate data relevant to their analysis. Data analysts use spreadsheets to perform simple analyses on small quantities of data. Analysts also use Business Intelligence, or BI Tools, such as Tableau, Power BI, or Looker, to create dashboards and share their analyses. More advanced data analysts may be comfortable with Python or R for cleaning and analyzing data.

## 7. Data scientist

00:00 - 00:00

Data Scientists have a strong background in statistics, enabling them to find new insights from data, rather than solely describing data. They also use traditional machine learning for prediction and forecasting. Within the workflow, they focus on the last three stages: data preparation and exploration and visualization, and experimentation and prediction.

## 8. Data scientist tools

00:00 - 00:00

Similar to analysts, data scientists have strong skills in SQL. Data scientists must be proficient in at least Python on R. Within these languages, they use popular data science libraries, such as pandas or tidyverse. These libraries contain reusable code for common data science tasks.

## 9. Machine learning scientist

00:00 - 00:00

Machine learning scientists are similar to data scientists, but with a machine learning specialization. Machine learning is perhaps the buzziest part of Data Science; it's used to extrapolate what's likely to be true from what we already know. These scientists use training data to classify larger, unrulier data, whether its to classify images that contain a car, or create a chatbot. They go beyond traditional machine learning with deep learning. Within the workflow, they do the last three stages with a strong focus on prediction.

## 10. Machine learning tools

00:00 - 00:00

Machine learning scientists use either Python or R to create their predictive models. Within these languages, they use popular machine learning libraries, such as TensorFlow, to run powerful deep learning algorithms.

## 11. Review: members of your team

00:00 - 00:00

Here's a slide to recap what we've covered. It may be intimidating to see all these tools and languages, but they aren't as difficult to learn as spoken languages. If you know English, it may take you years to learn French. Programming languages are more similar to power tools. If you know how to use a power drill, you don't necessarily know how to use an electric saw, but you can learn with a little training!

## 12. Let's practice!

00:00 - 00:00

Alright, time for some exercises!

![Pasted image 20240422212445.png](/img/user/Pasted%20image%2020240422212445.png)

![Pasted image 20240422213036.png](/img/user/Pasted%20image%2020240422213036.png)

![Pasted image 20240423150009.png](/img/user/Pasted%20image%2020240423150009.png)