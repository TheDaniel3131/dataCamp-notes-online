---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-data-science/chapter-4/","noteIcon":"","created":"2024-04-24T12:03:07.502+08:00","updated":"2024-04-24T12:03:55.404+08:00"}
---


# Lesson 1 - A/B Testing

## 1. A/B Testing

00:00 - 00:02

Welcome back!

## 2. Data science workflow

00:02 - 00:06

This chapter covers the final stage, beginning with experiments.

## 3. What are experiments in data science?

00:06 - 00:19

Experiments help drive decisions and draw conclusions. Generally, they begin with a question and a hypothesis, then data collection, followed by a statistical test and its interpretation.

## 4. Case study: which is the better blog post title?

00:19 - 00:47

For instance, suppose we want to pick the best blog post title. Our question is: does blog title A or blog title B result in more clicks? We make the hypothesis that both blogs will result in the same amount of clicks. To collect data, we randomly divide our audience into two groups, each seeing a different title. We run the experiment until our sample size is reached - more on that later.

## 5. Case study: which is the better blog post title?

00:47 - 01:08

Then, we use a statistical test to see whether the difference between the titles' click-through rate is significant. Finally, we interpret results. In our case, we want to choose the better performing title. However, often, its inconclusive, leading to more questions and experiments.

## 6. What is A/B Testing?

01:08 - 01:17

This is called A/B Testing, often called Champion/Challenger testing, and it's used to make a choice between two options.

## 7. Terminology Review

01:17 - 01:43

Sample size is the number of data points used. In data science, you'll hear "Are your results significant?". A statistically significant result means that your result is probably not due to chance given the statistical assumptions made. Statistical tests help determine this and there are many to choose from. Let's take a closer look at A/B testing.

## 8. A/B Testing Steps

01:43 - 01:56

There are four steps in an A/B test: picking a metric to track, calculating sample size, running the experiment, and checking for significance. Let's examine each step.

## 9. Pick a metric to track: click-through rate

01:56 - 02:03

Our metric is click-through rate, the percent of people who click on a link after viewing the title.

## 10. Calculate your sample size

02:03 - 02:32

Next, we'll run the experiment until we reach a sample size large enough to be certain that results aren't due to random chance. The size depends on a "baseline metric" that helps gauge any changes. In our case, it's how often people click on a link to one of our blogs usually. If the rate is much larger or smaller than 50%, then we need a larger sample size. Click-rate is typically under 3%.

## 11. Calculate your sample size

02:32 - 03:12

The sample size depends on the sensitivity we want. A test's sensitivity tells us how small of a change in our metric we can detect. Larger sample sizes allow us to detect smaller changes. You might think that we want a high sensitivity, but we actually want to optimize for an amount that is meaningful for our question. For example, if the first and second title are clicked on by 5% and 5.01% of viewers respectively, an extra .01% clicks to our blog post won't make a difference to us. However, if this was comparing 100m race time, an .01 difference would be significant.

## 12. Run your experiment

03:12 - 03:20

We run our experiment until we reach the calculated size. Stopping the experiment before or after could lead to biased results.

## 13. Check for significance

03:20 - 03:41

Once we reach the target size, we check our metric. We see some difference between the titles, but how do we know if it's meaningful? We check by performing a test of statistical significance. If they are significant, we can be reasonably sure that the difference is not due to random chance, but to an actual difference in preference.

## 14. What if the results aren't significant?

03:41 - 04:06

What if the results aren't significant? If there are any differences in click rates, they're smaller than the threshold we chose when determining the sensitivity. Running our test longer won't help because it'll only detect a smaller difference and we've decided that smaller differences are irrelevant! There still might be a difference in click rates between the titles: but that difference isn't important to us for making decisions.

## 15. Let's practice!

04:06 - 04:10

Now, let's practice!

![Pasted image 20240423223409.png](/img/user/Pasted%20image%2020240423223409.png)

Well done! You've organized the tasks necessary for conducting an A/B test. By performing all steps in the correct order, we can trust that the results of our A/B test are not due to random chance.

![Pasted image 20240423223821.png](/img/user/Pasted%20image%2020240423223821.png)

That's right! Remember, this is all based on the statistical assumptions made along with the sensitivity chosen. If we change those, the result could become statistically significant


![Pasted image 20240423224941.png](/img/user/Pasted%20image%2020240423224941.png)

Correct! Until we have reached the desired sample size, we can't be sure that our results aren't significant. We might just not have enough data.

# Lesson 2 - Time series forecasting

## 1. Time series forecasting

00:00 - 00:06

Great job so far. Now, we'll learn about modeling and time series forecasting.

## 2. Modeling in data science

00:06 - 00:26

Data scientists and machine learning scientists spend a lot of time building models. Models attempt to represent a real-world process with statistics. At a high level, models define relationships between variables with equations. These definitions are based on statistical assumptions and historical data.

## 3. Predictive modeling

00:26 - 00:35

Predictive modeling is a sub-category of modeling used for prediction. By modeling a process, we can enter new inputs and see what outcome it outputs.

## 4. Predictive modeling

00:35 - 00:44

For instance, you can enter a future date in a model of unemployment rate to get a prediction of what the unemployment rate will be next month.

## 5. Predictive modeling

00:44 - 00:52

The output can be the probability of an outcome, for example, the probability that a tweet is fake.

## 6. Predictive modeling

00:52 - 01:05

Predictive models can be as simple as a linear equation with an x and y variable to a deep learning algorithm that is uninterpretable by humans. Let's look at using predictive modeling on time series data.

## 7. Time series data

01:05 - 01:29

Time series is a series of data points sequenced by time. Examples include daily stock and gas prices over the years. Often times, it's in the forms of rates, such monthly unemployment rates or a patient's heart rate during surgery. They can be measurements like CO2 levels or the height of tides recorded regularly over a time period.

## 8. Plotting time series data

01:29 - 01:45

Let's plot an example. We have time series data of Canadian unemployment rates measured monthly from 1976 to 2015. Time series data is usually plotted as a line graph like this, with time on the x-axis.

## 9. Seasonality in time series

01:45 - 02:00

Often times when plotting time series, you can find patterns. For example, this plot graphs the average temperature in Boston over three years. Can you figure out the pattern here?

## 10. Seasonality in time series

02:00 - 02:23

The line peaks during summer months and reaches its lowest during winter months. If we graphed ice cream sales, we'd see a similar pattern. This is called seasonality. Seasonality is when there are repeating patterns related to time such as months and weeks. Another example is spending spikes at the end of the month when people receive a paycheck.

## 11. Forecasting time series

02:23 - 02:55

Time series data is used in predictive modeling to predict metrics at future dates. We call this forecasting. For example, predicting rainfall next month or the state of traffic and the stock market in a couple of hours to what the population will be in 20 years. We can build predictive models using time series data from the past years or decades to generate predictions. This uses a combination of statistical and machine learning methods. Let's look at an example.

## 12. Pea prices in Rwanda

02:55 - 03:27

The United Nation provides open data on global food prices. Here we have the price of peas in Rwandan Francs from 2011 and 2016. There's some seasonality here, can you spot it? Prices are lowest around December and January, but peak around August. Some years show a second peak around April . There seems to be a general increase in pea prices annually. Can we forecast what will happen with consideration to this seasonality and price increase?

## 13. Forecasting pea prices in Rwanda

03:27 - 04:15

Here is the forecast of a predictive model. The blue line depicts the forecast. The seasonality remains and it anticipates a continued increase of pea prices, seen by the higher peaks and lows. There are also two blue areas shown along the forecast. These are confidence intervals, which are extremely useful for evaluating predictions. We see two confidence intervals: 80% and 95%. The model is 80% sure that the true value will be in the area labeled as 80. Same goes with the area labeled as 95. If we're using this forecast to make big decisions, confidence intervals can help us buffer for the unexpected.

## 14. Let's practice!

04:15 - 04:20

Ok, it's time for some exercises

![Pasted image 20240423225112.png](/img/user/Pasted%20image%2020240423225112.png)

Nice job! An easy way to distinguish non-time series data is the lack of time associated with every data entry.

![Pasted image 20240423225645.png](/img/user/Pasted%20image%2020240423225645.png)

Right on! That's about 0.50 USD, if you're wondering. Imagine you're trying to make a budget for food, confidence intervals would be useful for that!

# Lesson 3 - Supervised machine learning

## 1. Supervised machine learning

00:00 - 00:00

In this video, we'll dive into machine learning!

## 2. Data science workflow

00:00 - 00:00

As we learned previously, machine learning is a set of methods for making predictions based on existing data, hence it belongs in the last step of the workflow.

## 3. What is supervised machine learning?

00:00 - 00:00

Supervised machine learning is a subset of machine learning where the existing data has a specific structure: it has labels and features. More on that later. Examples of its abilities includes recommendation systems, diagnosing biomedical images, recognizing hand-written digits, and predicting customer churn. Let's define these new terms with a case study.

## 4. Case study: churn prediction

00:00 - 00:00

Suppose we have a subscription business and want to predict whether a given customer is likely to stay subscribed or cancel their subscription, also known as churn.

## 5. Case study: churn prediction

00:00 - 00:00

First, we need some training data to build our model off of. This would be historical customer data.

## 6. Case study: churn prediction

00:00 - 00:00

Some of those customers will have maintained their subscription, while others will have churned. We eventually want to be able to predict the label for each customer: churned or subscribed.

## 7. Case study: churn prediction

00:00 - 00:00

We'll need features to make this prediction. Features are different pieces of information about each customer that might affect our label. For example, perhaps age, gender, the date of last purchase, or household income will predict cancellations. The magic of machine learning is that we can analyze many features all at once. We use these labels and features to train a model to make predictions on new data.

## 8. Case study: churn prediction

00:00 - 00:00

Suppose we have a customer who may or may not churn soon. We can collect feature data on this customer, such as age, or date of last purchase.

## 9. Case study: churn prediction

00:00 - 00:00

We can feed this data into our trained model

## 10. Case study: churn prediction

00:00 - 00:00

and then, our trained model will give us a prediction. If the customer is not in danger of churning, we can count on their revenue for another month! If they are in danger of churning, we can reach out to them to try to keep them subscribed.

## 11. Supervised machine learning recap

00:00 - 00:00

Let's recap. Machine learning makes a prediction based on data. In supervised machine learning, that data has two characteristics: features and labels. Labels are what we want to predict, like the customer churning. Features are data that might help predict the label, such as profession or date of last purchase. Once we have the features and labels, we train a model and use it to make predictions on new data.

## 12. Model evaluation

00:00 - 00:00

After training a model, how do we know if it's any good? It's always good practice not to allocate all of your historical data for training. Withheld data is called a test set and can be used to evaluate the goodness of the model. In our example, we could ask the model to predict whether a set of customers would churn, and then measure the accuracy of our prediction.

## 13. Model Evaluation

00:00 - 00:00

For example, let's say we're testing our model on our test set made up of 1000 customers, where only 30 of the customers have actually churned.

## 14. Model Evaluation

00:00 - 00:00

We put that test data into our newly trained model and it predicts that all the customers remain.

## 15. Model Evaluation

00:00 - 00:00

If we calculate the overall accuracy of that model, it technically has a high accuracy of 97% because it was correct on 970 of the 1000 customers. This is despite never correctly labeling a customer churning. Checking both outcomes is important for rare events. Only by examining the accuracy of each label do we get 0% accuracy at predicting churn when churn was the actual outcome. This model is not useful to use in its current state, so we'll have to re-train it with different parameters or more data.

## 16. Let's practice!

00:00 - 00:00

You learned how supervised learning uses features and labels and how to be cautious with model accuracy. Time for practice!

![Pasted image 20240423225902.png](/img/user/Pasted%20image%2020240423225902.png)

Great job! A/B tests help us pick between two choices. Supervised machine learning helps us make predictions using features and labels. Dashboards help us display information.


![Pasted image 20240423230818.png](/img/user/Pasted%20image%2020240423230818.png)

Great job! Juan wants to predict the industry, hence it is our label. The other columns are features and will help us predict the value of the label “Industry”.

![Pasted image 20240423231300.png](/img/user/Pasted%20image%2020240423231300.png)

Correct! Overall, it is only accurate in 93% of cases, but it can always predict when a fraudulent transaction is fraudulent, which is important for our use case.


# Lesson 4 - Clustering

## 1. Clustering

00:00 - 00:10

Previously, we learned how to use Supervised Learning to make predictions based on labeled data. In this lesson, we’ll cover another subset of machine learning called clustering.

## 2. What is clustering?

00:10 - 00:31

Clustering is a set of machine learning algorithms that divide data into categories, called clusters. Clustering can help us see patterns in messy datasets. Machine Learning Scientists use clustering to divide customers into segments, images into categories, or behaviors into typical and anomalous.

## 3. Supervised vs. unsupervised machine learning

00:31 - 00:58

Clustering is part of a broader category within Machine Learning called "Unsupervised Learning". Unsupervised Learning differs from Supervised Learning in the structure of the training data. While Supervised Learning uses data with features and labels, Unsupervised Learning uses data with only features. This makes Unsupervised Learning, and clustering, particularly appealing: you can use it even when you don't know much about your dataset.

## 4. Case study: discovering new species

00:58 - 01:18

Let's say you are a botanist and you've been doing field work on a previously unexplored island. Notably, you have several observations on these flowers you've never seen before. You believe you might have discovered a couple new flower species, but you're not sure how many and how to classify each flower. Let's see if clustering can help.

## 5. Defining features

01:18 - 01:40

The first step is finding features. Luckily, you've been meticulous in your data gathering and measured over 100 flowers. We can use your measurements as features for our model. This is indeed an unsupervised learning problem because we have features but we're not sure what species each flower belongs to or even how many new species there are!

## 6. Defining number of clusters

01:40 - 02:01

Some clustering algorithms need us to define how many clusters we want to create. The number of clusters we ask for greatly affects how the algorithm will segment our data. Here's our flower data graphed over three features: petal width, sepal length, and number of petals on the x,y, and z axes, respectively.

## 7. Comparing number of clusters

02:01 - 02:17

Here is how the algorithm divides the data if we ask for two clusters. One color represents on cluster, in our case, one new flower species. And here is how it divides the same data if we ask for three clusters.

## 8. Comparing number of clusters

02:17 - 02:31

And these are the results when we ask for four and eight clusters. We can tell intuitively that eight is probably too many clusters, because there aren't as many clear cut areas in our graph.

## 9. Comparing number of clusters

02:31 - 03:02

Clustering won't tell us exactly how many clusters we have, but it can help us make an informed decision. In your case, it seems like you've found three or four new species. Having a strong hypothesis about our data helps us get better results from the clustering algorithm. For example, you may know from your experience as a botanist that petal width usually has wide variance within a species and shouldn't be given too much weight. You can use this information to design a better clustering algorithm.

## 10. Clustering review

03:02 - 03:34

Let's review. Clustering is an Unsupervised Machine Learning method that divides an unlabeled dataset into different categories. In order to perform clustering, we must first select relevant features of our dataset. Next, we select the number of clusters based on hypotheses about our data. Finally, we use the results of our clustering to solve our problems, whether it's defining new species, segmenting customers, or classifying movies into genres. There are a lot of diverse usages for clustering!

## 11. Let's practice!

03:34 - 03:39

Now that we understand clustering, let's practice!

![Pasted image 20240423231545.png](/img/user/Pasted%20image%2020240423231545.png)

Great job! Data that has labels, like whether or not a purchase was made, or whether or not a clothing item was profitable, can be used to train supervised learning models. Data with no labels can be clustered using unsupervised learning methods. Do you see how machine learning can be used at different types of organizations and companies?

![Pasted image 20240423231741.png](/img/user/Pasted%20image%2020240423231741.png)

Correct! The data is best described by four clusters. A new hub should be placed at the center of each cluster

# End

## 1. Congratulations!

00:00 - 00:10

Congratulations on reaching the end of this course, and thank you for taking it! Hopefully you have a much better understanding about what data science is.

## 2. Chap 1: Introduction to Data Science

00:10 - 00:21

In the first chapter, you learned about data science and the different roles within the data science field, got introduced to the data science workflow, and saw some real-world data science applications.

## 3. Chap 2: Data Collection and Storage

00:21 - 00:36

The second chapter focused on the first step in the data science workflow. First you learned about the different data sources you can draw from, what that data looks like, how to store the data once it's collected, and how a data pipeline can automate the process.

## 4. Chap 3: Preparation, Exploration & Visualization

00:36 - 00:48

In chapter 3, you learned what happens in steps two and three. You learned how to prepare and explore your data for analysis and ended by looking at some visualization best practices and dashboards.

## 5. Chap 4: Experimentation and Prediction

00:48 - 01:06

In this final chapter, the final step of the workflow was covered. Beginning with experiments, you learned about A/B testing, and then moved on to time series forecasting where you learned about predicting future events. Finally, you ended with machine learning, looking at supervised learning, and clustering.

## 6. What's next?

01:06 - 02:04

If, after taking this course, you're convinced of the power of data science and want to start coding, we recommend trying out our Introduction to Python course. Python is a programming language that is extremely popular in the fields of data science and machine learning. In our Introduction to Python course, you'll learn about powerful ways to store and manipulate data,and helpful tools to begin conducting your own data science analyses. Even if you've never written a line of code in your life, you'll be able to follow this course! If you want to learn more about some of the topics mentioned in the course, like machine learning, data engineering, or cloud computing, we've got the perfect track for you. The Data Literacy Fundamentals Skill track consists of other "For Everyone" courses on key data topics that assume no prior technical knowledge. This track is great if you want to build up your data literacy skills to unpack jargon and leverage data and technology at work.

## 7. Congratulations!

02:04 - 02:12

Once again, thank you for taking this course. We wish you the best of luck with your future data science endeavors!