---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/explainable-artificial-intelligence-xai-concepts/chapter-2/","noteIcon":"","created":"2024-04-28T16:45:44.635+08:00","updated":"2024-04-28T16:47:39.121+08:00"}
---


# Lesson 1 - XAI Techniques

## 1. XAI techniques

00:00 - 00:10

Well done on the exercises so far! We will now explore ways in which XAI aims to explain an AI system in a transparent and understandable way.

## 2. XAI explanations

00:10 - 00:30

There are different ways in which XAI aims to explain the decision making of an AI system. We can categorize the approaches as follows. Model-specific explanations, model-agnostic explanations, local explanations, and global explanations. We will go over these throughout the course as well in more detail.

## 3. Model-specific explanations

00:30 - 00:49

An example of a model-specific explanation is a decision tree. We can use AI to automatically generate a decision tree from a dataset. This decision tree can be visualized to understand how the data is categorized. This is how a visualization of decision tree is a model-specific explanation.

## 4. Model-agnostic explanations

00:49 - 01:15

Model-agnostic explanations are like a swiss army knife. They're flexible and adaptable, capable of working with any AI model, whether it's a simple linear model or a complex neural network. These explanations don't need to know the inner workings of the model. They can provide insights just by looking at the input and output, much like how a swiss army knife can help you without needing to be custom-made for each task.

## 5. Local explanations

01:15 - 01:45

Imagine using a zoom lens on a camera to focus closely on a single detail in a vast landscape. Local explanations in XAI do something similar. They zoom in on a single decision made by an AI model, like why it recommended a particular movie or flagged a transaction as fraudulent. This close-up view helps us understand the reasoning behind specific, individual outcomes, providing clarity and transparency for those particular cases.

## 6. Global explanations

01:45 - 02:15

Contrast that zoom lens with a panoramic photo that captures the entire landscape in one wide shot. Global explanations offer a comprehensive overview of an AI model's overall behavior, similar to that panoramic view. They help us see the big picture, showing us how the model tends to make decisions across a wide range of scenarios. This broad perspective is crucial for understanding the general principles guiding the model's behavior, ensuring it aligns with our values and expectations.

## 7. Applying the right explanation

02:15 - 02:52

Choosing the right type of explanation depends on your specific needs and context. Use model-agnostic explanations when dealing with multiple models or when simplicity and flexibility are paramount. Opt for model-specific explanations when depth and detail are required to understand or refine a particular model. Apply local explanations when you need to dissect and justify individual decisions, especially in critical applications. Employ global explanations to gain and provide a comprehensive understanding of the model's behavior and to ensure alignment with broader goals and standards.

## 8. Let's practice!

02:52 - 03:07

As we move forward, we'll explore these concepts in more depth, applying them to real-world AI scenarios to see how they explain the inner workings of AI, making it more transparent, understandable, and trustworthy.

![Pasted image 20240428164714.png](/img/user/Pasted%20image%2020240428164714.png)

Exactly right! A local explanation is ideal for dissecting and understanding the specific reasoning behind this unusual movie recommendation.

