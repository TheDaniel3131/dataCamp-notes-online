---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/explainable-artificial-intelligence-xai-concepts/chapter-2/","noteIcon":"","created":"2024-04-28T16:45:44.635+08:00","updated":"2024-04-28T17:08:45.212+08:00"}
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

![Pasted image 20240428165154.png](/img/user/Pasted%20image%2020240428165154.png)

Well done on finishing the exercise! Your understanding of model-specific and model-agnostic XAI techniques is essential for navigating the complexities of AI explanations. This knowledge is valuable for applying XAI effectively. Keep building on this foundation as you progress in the field.

# Lesson 2 - Model-specific Explanations

## 1. Model-specific explanations

00:00 - 00:00

Congratulations on the great progress thus far! In this video, we're going to dive deeper into what makes certain AI models inherently explainable through model-specific explanations.

## 2. Model-specific explanations

00:00 - 00:00

We'll be exploring two fundamental AI systems, regression and classification. Both methods have roots that predate AI, yet they remain central in the data science landscape. They help us make sense of the vast data in today's digital world by providing clear, interpretable outcomes. Regression is about determining the relationship between two variables, for instance the relationship between the outside temperature and ice cream sales. Classification is about predicting the label of a certain input, for instance if the fruit is red it is probably a strawberry.

## 3. Regression: understanding linear relationships

00:00 - 00:00

Let's look in more depth into regression. At its core, regression is about understanding the relationship between variables. For instance, we might look at how outside temperature affects ice cream sales. This might seem straightforward, but here's where its explainability shines. Through regression, we can visualize this relationship. Imagine plotting temperature against ice cream sales on a graph and drawing a line that best fits the data points. This line isn't just a mathematical abstraction, it's a tangible representation of the relationship between these variables. It allows us to predict, say, ice cream sales based on temperature in an intuitive, visually interpretable way. This visual aspect, where results can be graphed and relationships literally seen, is what makes regression inherently explainable.

## 4. Classification: sorting data into categories

00:00 - 00:00

Moving on to classification, this method is about sorting data into categories based on certain features. Think of it as sorting a basket of fruit into oranges, apples, and cucumbers based on characteristics like color and shape. The explainability of classification models often comes from their decision-making process, which, in simpler models, can be as clear as following a flowchart. For example, a decision tree, a type of classification model, lets us trace exactly how decisions are made. First we check if the fruit is red. Next we'll check if it's round. If yes, it's probably an apple. This step-by-step process, where we can follow the logic from input to category, showcases the inherent explainability of classification models.

## 5. Black box models: multitude of intricate patterns

00:00 - 00:00

However, as we introduce more complex models that analyze a multitude of factors—like texture, genetic variety, and growth conditions—the decision-making process can become less transparent, turning these models into what we call black boxes. Despite their ability to handle vast datasets and uncover intricate patterns, the 'how' of their predictions becomes obscured. This transition from clear, interpretable models to more opaque ones highlights the importance of XAI. As we delve further into this course, we'll explore strategies within XAI aimed at demystifying these complex models, making AI's intricate decisions more transparent and understandable.

## 6. Let's practice!

00:00 - 00:00

Now that we've clarified why regression and classification can be inherently explainable through their visual and logical clarity, let's put this understanding into practice with some exercises.

![Pasted image 20240428165307.png](/img/user/Pasted%20image%2020240428165307.png)

Correct! This analogy beautifully captures the essence of classification's explainability. It's important because it helps demystify AI decisions, making the technology more transparent and trustworthy.

![Pasted image 20240428165513.png](/img/user/Pasted%20image%2020240428165513.png)

Excellent! Black box models are ideal for dissecting complex relationships within large datasets, offering insights that simpler models might miss. Black box models, due to their inherent complexity, can challenge transparency, making them less suited for projects where explainability is key.

# Lesson 3 - Model-agnostic Explanations

## 1. Model-agnostic explanations

00:00 - 00:06

Excellent work on the exercises so far! We will now dive into the explainability of black box models.

## 2. Black box models

00:06 - 00:30

Imagine a black box model as a magical device that can predict things like whether a photo contains a cat or a dog, but we have no idea how it makes those predictions. It’s like a magician’s hat. We know what goes in, and we see what comes out, but the trick happening inside is a mystery. This is caused by the amount of internal parameters, which can become huge in complex models.

## 3. Global and local explanations

00:30 - 00:53

To mitigate this lack of transparency in black box models, we can apply two techniques to estimate what happened in the magician's hat. This will give us an insight into how the model came to its decision. We will look into SHAP, short for SHapley Additive exPlanations, and LIME, which is short for Local Interpretable Model-agnostic Explanations.

## 4. SHAP (SHapley Additive exPlanations)

00:53 - 01:27

Now, let’s talk about SHAP. SHAP is like a detective, it helps us uncover the secrets hidden within the black box. It does this by looking at each piece of evidence, in this case features, and figuring out how much each one contributes to the final decision. Imagine you’re baking a cake. SHAP utilizes cooperative principles from game theory to determine the impact of each ingredient in the cake. It ensures that each ingredient gets its fair share of credit in determining the taste of the cake.

## 5. Shapley values

01:27 - 02:05

In cooperative game theory, there’s a concept called Shapley values. These values help distribute the contribution of each feature fairly. SHAP applies this concept to machine learning models, ensuring that each feature’s impact is accurately assessed. For example, when trying to predict customer churn, SHAP helps us understand which features matter the most for the model to say, “This customer will churn”. We can see the average positive and negative impact of each feature on the model's output. It’s like ensuring that each ingredient in your cake gets the right credit for its role in the cake’s deliciousness.

## 6. SHAP image recognition

02:05 - 02:24

Showing how SHAP works in an image recognition example, we can see where the model bases its classification on. It shows that for the Dowitcher, the beak is a feature of the bird to classify it as such. Similarly, we can see for the Meerkat that the head played an important role.

## 7. LIME (Local Interpretable Model-agnostic Explanations)

02:24 - 02:55

Now, let’s meet LIME. LIME is like a curious scientist who wants to understand the magician’s trick by changing things slightly and observing the outcome. It tweaks the input data to see how the model reacts. Think of it as having a scientist in a laboratory setting. LIME helps us create a simpler, understandable recipe for individual predictions. In image recognition, LIME would ask, "What if we change some pixels in this image? Would it still be classified as a cat?"

## 8. Building a self-driving car

02:55 - 03:31

To compare SHAP and LIME, let’s imagine we’re building a self-driving car. We would use SHAP to global understanding, finding out which car features (like steering, brakes, and gas pedal) are most important for the car’s overall safety and performance across your entire dataset. It’s like deciding which car parts to focus on for an entire fleet of cars. On the other hand, LIME helps us explain specific moments when the car made decisions, like turning left at an intersection. It’s like conducting experiments in a lab to understand why our car made a specific turn in a particular situation.

## 9. Let's practice!

03:31 - 03:40

Let's dive into some exercises to get a deeper understanding of how to apply explainable techniques to black box models.

![Pasted image 20240428170216.png](/img/user/Pasted%20image%2020240428170216.png)

Excellent job! You've successfully completed the exercise, demonstrating your understanding of different techniques in XAI. Understanding these methods is crucial in the field of machine learning and AI, as it empowers us to make complex models more transparent and interpretable.

![Pasted image 20240428170526.png](/img/user/Pasted%20image%2020240428170526.png)

Fantastic choice! This approach closely mirrors the LIME methodology, focusing on understanding the impact of individual changes, just as you'd tweak a single ingredient to see its effect on the dish.

# Lesson 4 - Explainability of LLMMs

## 1. Explainability of LLMs

00:00 - 00:00

Excellent job on understanding the concepts in XAI so far. We will now explore the world of Large Language Models. In particular the explainability of LLMs.

## 2. Large Language Models (LLMs)

00:00 - 00:00

Language Models, particularly Large Language Models, are the brains behind the AI systems that understand, generate, and interpret human language. Examples of LLMs are ChatGPT or Bard. These models are trained on vast amounts of text data, learning the intricacies of language patterns, grammar, and semantics. They can write articles, compose poetry, or even code, mimicking human-like language understanding. But with this complexity comes a challenge: how do we understand the decisions and predictions made by these models?

## 3. LLMs and explainability

00:00 - 00:00

The primary challenge with LLMs is their black box nature. LLMs are huge neural networks with a vast amount of layers that contribute to their complexity. Given their complexity and the sheer scale of data they're trained on, it's often not clear why a model generates a specific piece of text. For instance, why does a chatbot respond in a particular way to a user's question? The complexities of these models, combined with their ability to learn and replicate biases present in their training data, make it imperative to develop methods to peer into these black boxes, ensuring they operate fairly, ethically, and transparently. There are methods creators of an LLM tool can implement, but also methods end users can utilize to make the decision-making of LLMs more transparent.

## 4. Methods for LLM explainability

00:00 - 00:00

Creators can provide clear documentation and understanding of the data used to train LLMs, through which we can gain insights into the potential biases and limitations of these models. Creating a simpler, more interpretable proxy models can help approximate the behavior of more complex LLMs, offering a window into their decision-making process. Creators can also incorporate human feedback and oversight into the model's training and deployment processes to ensure that LLMs remain aligned with ethical standards and societal values. End users could prompt the LLM to generate and provide evidence to substantiate the statements it produces. End users could also generate examples of how slight changes in the input could lead to different outputs to help understand the model's reasoning process.

## 5. Future use of LLMs

00:00 - 00:00

As we continue to integrate LLMs into various aspects of our lives, enhancing their explainability is not just a technical challenge but also a requirement. Ensuring that these models are understandable and accountable helps build trust and confidence in AI systems, which results in ethical AI solutions.

## 6. Let's practice!

00:00 - 00:00

Now that we've learned all about the explainability of large language models, let's go into some exercises to test our knowledge.

![Pasted image 20240428170723.png](/img/user/Pasted%20image%2020240428170723.png)

Congratulations! You've nailed it! Just like a librarian in a vast library, an LLM draws upon a wide expanse of information (akin to books) to craft responses, showcasing its ability to synthesize and interpret vast amounts of data.

![Pasted image 20240428170843.png](/img/user/Pasted%20image%2020240428170843.png)

Great choice! By generating multiple responses to slightly varied prompts, your friend can observe how small changes influence the LLM's output, offering indirect insight into its reasoning process.

