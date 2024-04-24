---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-data-science/chapter-3/","created":"2024-04-23T18:59:42.359+08:00","updated":"2024-04-23T22:29:34.736+08:00"}
---


# Lesson 1 - Data Preparation

## 1. Data preparation

00:00 - 00:00

Great job so far! I'm Hadrien, and I will now tell you about data preparation.

## 2. Data workflow

00:00 - 00:00

Data preparation happens after collecting and storing the data.

## 3. Why prepare data?

00:00 - 00:00

Data rarely comes in ready for analysis. Real-life data is messy and dirty. It needs to be cleaned. Skipping this step may lead to errors down the way, incorrect results, or throw off your algorithms. You would not use vegetables without cleaning, peeling and dicing them, as your soup would taste weird and no one would eat it. Well, if you don't clean, peel and dice your data, your results will look weird, and no one will use them!

## 4. Let's start cleaning

00:00 - 00:00

Let's take a simple, but dirty, dataset, and clean it together. Maybe you can already notice a few things.

## 5. Tidy data

00:00 - 00:00

One fundamental aspect of cleaning data is "tidiness". Tidy data is a way of presenting a matrix of data, with observations on rows and variables as columns. This is not the case here. Our observations (people) are in columns, and their features are on rows. Let's take care of that. It's easy to do that programmatically with Python or R. They also help with the other cases you're about to see.

## 6. Tidy data output

00:00 - 00:00

The data looks much clearer this way.

## 7. Remove duplicates

00:00 - 00:00

In general, you want to remove duplicates. Python and R make them easy to identify. Here we can see that Lis appears twice.

## 8. Remove duplicates | output

00:00 - 00:00

Let's remove the duplicate.

## 9. Unique ID

00:00 - 00:00

What if there's another person called Lis? Then, you want a way to uniquely identify each observation. It can be a combination of features (name plus last name plus year of birth, for example),

## 10. Unique ID | output

00:00 - 00:00

but the safest way is to assign a unique ID. Sara's ID is now 0, Lis' 1 and Hadrien's 2.

## 11. Homogeneity

00:00 - 00:00

Something fishy is going on in the size column. Lis simply can't be that tall (or Hadrien and Sara that small, depending where you're from). Lis is in the US, she inputted her size in feet. Sara and Hadrien are based in Europe, they use the metric system. All variables should use the same standard.

## 12. Homogeneity | output

00:00 - 00:00

Programmatically, you can filter values above 2.5 meters, and apply a division by 3.281 to get the metric value. Here we go.

## 13. Homogeneity, again

00:00 - 00:00

Similarly, countries should follow the same format. The United States and France are abbreviated, but Belgium is written in full. Let's fix that.

## 14. Homogeneity, again | output

00:00 - 00:00

Looking better already!

## 15. Data types

00:00 - 00:00

Another common issue relates to data types. The tools you use might be able to infer data types for each column, but you'd better make sure they are correct. Here, the Age column is encoded as text. If you try to get the mean, you'll get an error, because the average of two words doesn't make sense. You should change the type of this feature to numbers.

## 16. Data types | output

00:00 - 00:00

Ages are now numbers; you can see the quotes have disappeared.

## 17. Missing values

00:00 - 00:00

Last but not least, missing values. They are common and occur for various reasons: the agent doing the entry was distracted, the person surveyed did not understand the question, or it's on purpose, for example an event that has not happened yet. There are several ways to deal with missing values. You can substitute the exact value if you have access to the source. For example, you can take an aggregate value, like the mean, median or max depending on the situation. You can drop the observation altogether, but each observation you remove means less training data for your model. Or, you can keep it as is and ignore it, if your algorithm allows it.

## 18. Missing values | output

00:00 - 00:00

Here, we take the mean, 27.5, and round it up to get 28, which happens to be the correct value.

## 19. Let's practice!

00:00 - 00:00

Let's check your understanding!

![Pasted image 20240423202435.png](/img/user/Pasted%20image%2020240423202435.png)

Correct! There might be a good reason why this data is missing. If you investigate more, you will find the full report in the `report_link` column. You will find the event's date (April 12th, 2019) and location (Winnipeg, Canada). More importantly, you will see the report is about an abduction, not a sighting. You can keep the row if you want to include abductions. Otherwise, you can drop it; but you then need to investigate further to remove other abduction reports.


![Pasted image 20240423204500.png](/img/user/Pasted%20image%2020240423204500.png)

# Lesson 2 - Exploratory Data Analysis

## Exploratory Data Analysis

00:00 - 00:07

Excellent job on data preparation! Let's keep going with Exploratory Data Analysis.

## 2. What is EDA?

00:07 - 00:26

Exploratory Data Analysis, or EDA for short, is a process that was promoted by John Tukey, a respected statistician. It consists in exploring the data and formulating hypotheses about it, and assessing its main characteristics, with a strong emphasis on visualization.

## 3. Data workflow

00:26 - 00:33

EDA happens after data preparation, but they can get mixed. EDA can reveal new things that need cleaning.

## 4. Let's dive right in

00:33 - 00:44

Let's dive right in. What can you say about these four different datasets? Well, from these lines of data, probably very little.

## 5. Surprise!

00:44 - 01:09

All four datasets have identical mean and variance both for the x and y features. They also have an identical correlation coefficient, and the same linear regression equation (the straight line that tries to go through all points). If you're not sure about some of the metrics listed, that's OK. The point is, they seem awfully similar! But is that the case?

## 6. Anscombe's quartet

01:09 - 01:18

No! Here are the four graphs. They all tell a different story, that pure metrics can't fully convey.

## 7. Anscombe's quartet

01:18 - 01:21

The first graph displays a linear relationship,

## 8. Anscombe's quartet

01:21 - 01:25

while the second one has a non-linear relationship.

## 9. Anscombe's quartet

01:25 - 01:31

In the third graph, we see the linear line is thrown off by one point that has an extreme y value.

## 10. Anscombe's quartet

01:31 - 02:02

A similar thing happens with the fourth dataset. We should have no correlation, but one extreme point is enough to display a strong one. In short, streaming through the data gives you little information. Descriptive statistics do better, but can be misleading; visualization teaches us the most. That's why EDA relies heavily on this last technique. This was an extreme example, to make a point. Let's now look at another dataset.

## 11. SpaceX launches

02:02 - 02:08

Let's look at SpaceX launches!

## 12. Knowing your data

02:08 - 02:19

I mean, let's look at the data behind SpaceX launches. The first thing to do is to know what features we're looking at. We have different information, such as the flight number or what the rocket transported. All have the correct data type.

## 13. Previewing your data

02:19 - 02:27

Looking at your tables helps make sense of your observations. Can you notice the missing payload mass for the first two rows?

## 14. Descriptive statistics

02:27 - 03:00

It's always a good idea to calculate descriptive statistics. The SpaceX dataset is mainly qualitative, but we still get a lot of information. We have a count of 55 pretty much everywhere, because we have 55 launches. The Payload Mass column shows 53 because of the two missing values we saw before. Only 1 mission failed. Most of the time, there is no attempt at landing. You could also calculate the average payload mass, or the count of launches per year. But do you know what would be best for this last option?

## 15. Visualize!

03:00 - 03:21

Visualization! In a glance we can see that there were no launches in 2011. The count of launches then gradually increased before doubling in 2017. 2018 is lower, but remember we only have 3 months of data for this year, so it actually looks like it's going to double again.

## 16. Ask more questions!

03:21 - 03:40

Now this launch count is informative, but you probably have a couple more. How about count by launch site? Rockets originally launched from Cape Canaveral Air Force Station, but in 2017 most rockets launched from Kennedy Space Center Launch Complex 39.

## 17. Ask more questions!

03:40 - 03:44

How about mission outcome? Just one failure in 2015!

## 18. Outliers

03:44 - 04:08

Another thing you do during EDA is look for outliers, that is, unusual values. Whether they are errors or valid, it's nice to know about them, as they can throw your results off. Here, we can see we have only 5 launches with a weight greater than 7,000 kg, when the average mass is closer 3800 kg.

## 19. Let's practice!

04:08 - 04:13

Let's check your understanding of the EDA process!

![Pasted image 20240423205815.png](/img/user/Pasted%20image%2020240423205815.png)

Right! There are 52 observations in this dataset, from 2009 to 2013. If you're used to looking at statistics, you may have noticed something curious about the numbers here. If not, no worries. You will investigate in the next exercise.

![Pasted image 20240423205949.png](/img/user/Pasted%20image%2020240423205949.png)

![Pasted image 20240423205931.png](/img/user/Pasted%20image%2020240423205931.png)

# Lesson 3 - Visualization

## 1. Interactive dashboards

00:00 - 00:06

We finished the last lesson looking at some graphs, so let's talk a little more about visualization.

## 2. One picture...

00:06 - 00:22

One picture is worth a thousand words, they say. Based on what we saw in the previous lesson, we would tend to agree. However, there are a few things to pay attention to, to ensure your chart is easily understandable and straight to the point.

## 3. Use color purposefully

00:22 - 00:31

For example, you should use color purposefully. Remember this graph? Count of launches by year, pretty straightforward.

## 4. Use color purposefully

00:31 - 00:33

What about this one?

## 5. Use color purposefully

00:33 - 00:36

So colorful, so much better!

## 6. Use color purposefully

00:36 - 00:50

Wrong! Granted, it's aesthetically pleasing, but it's also confusing. What do the colors correspond to? Nothing. We're just counting launches per year. One color is enough.

## 7. Colorblindness

00:50 - 01:07

You should also be mindful of colorblindness. You may distinguish red and green very well, but some people don't, and more than you think. You can find a lot of information on colorblindness online, as well as palettes of colors that are accessible to colorblind people.

## 8. Readable fonts

01:07 - 01:19

You should also use readable fonts. Sans-serif ones are easier to read. There are nicer fonts available, sure, but your readers should focus on your viz message, not on the font.

## 9. Label, label, label

01:19 - 01:40

An image is worth a thousand words, but words do help. Your graphs should always have a title, so we know what we're looking at; the x and y axis should have labels, otherwise they could be anything; and you should provide a legend if you use colors and patterns, so that we know what they refer to.

## 10. Axes

01:40 - 01:55

There are some cases when you can start your axes higher than zero, if you want to zoom in on evolution, for example. But it can be misleading. Here, it looks like Obamacare enrollment is far from the goal,

## 11. Axes

01:55 - 01:58

when it's actually close.

## 12. And the award goes to...

01:58 - 02:05

Follow these advises, and you should prevent your readers the confusion that comes with badly designed graphs like this one,

## 13. Honorable mention

02:05 - 02:09

Or this one. I don't know where to start.

## 14. Question

02:09 - 02:15

If a picture is worth a thousand words, then what is worth a thousand pictures?

## 15. A dashboard!

02:15 - 02:48

A dashboard! Well, technically, a dashboard of a few pictures is enough already. My point is, showing several pictures together can be more insightful than looking at them separately, or trying to pack all the insights in one graph. Your car dashboard indicates the car speed, the motor rotation speed and the proportion of gas left. Individually, these pieces of information are useful. But together, they paint a much bigger picture and make your trip more safe and more comfortable.

1. 1 Photo by Marek Szturc on Unsplash

## 16. Dashboards

02:48 - 03:23

That's what dashboards do: group all the relevant information in one place to make it easier to gather insights and act on them. On this dashboard, any sales person can see not only how sales are progressing this quarter, but also how this progression compares to previous quarters. On top of that, they can keep track of transactions and opportunities, as well as of customer count. They can filter all of this data by software, service or maintenance sales. All of that in one place, customized for their needs!

## 17. BI tools

03:23 - 03:43

Business Intelligence tools let you clean, explore, visualize data, and build dashboards, without requiring any programming knowledge. Such tools are Tableau, Looker, or Power BI. Of course, you can also do that programmatically using Python, R, or even JavaScript.

## 18. Next level

03:43 - 04:08

The next level is to make your visualization interactive, which BI tools make really easy. It lets you display more targeted information when hovering over an element, like you can see here. We also talked about filters: here the user can filter on the type of sales and the quarter. Giving power to the user is a great way to engage them.

## 19. Let's practice!

04:08 - 04:12

Home stretch to Chapter 4!


![Pasted image 20240423210309.png](/img/user/Pasted%20image%2020240423210309.png)

Nice! Pretty handy, right? Interactivity allows us to plot more without having to show all the values clearly at once.


![Pasted image 20240423222804.png](/img/user/Pasted%20image%2020240423222804.png)

Nice job! In the video, we saw cases of misleading axes, but this isn't the case here. We know that average speed is going to be more than 0 and by starting at 52, we can better see the changes in speed as they occur between 52 and 62.