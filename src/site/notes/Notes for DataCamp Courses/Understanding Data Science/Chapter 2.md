---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-data-science/chapter-2/","noteIcon":"","created":"2024-04-23T16:22:07.830+08:00","updated":"2024-04-23T18:38:29.664+08:00"}
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

### Quantitative data can be counted, measured, and expressed using numbers. 

### Qualitative data is descriptive and conceptual. Qualitative data can be observed but not measured. Now that we know the differences, let’s dive into each type of data with a real-world example.


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
