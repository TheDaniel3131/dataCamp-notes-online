---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/explainable-artificial-intelligence-xai-concepts/chapter-3/","noteIcon":"","created":"2024-04-28T17:09:05.457+08:00","updated":"2024-04-28T17:39:31.279+08:00"}
---


# Lesson 1 - Tailoring AI to the user

## 1. Tailoring AI to the user

00:00 - 00:00

Excellent work so far! We will now dive into how we can design more effective AI systems with XAI in mind.

## 2. AI systems need to align with the end-user

00:00 - 00:00

Often, AI systems are used to optimize current processes. To effectively integrate AI within these processes, its important to tailor the AI system we are developing to the main stakeholder in this process. Imagine receiving a high-tech coffee machine equipped with the latest AI to brew coffee exactly to our taste. However, it comes with a complex interface filled with confusing buttons and menus. This scenario mirrors integrating an AI system into a process without tailoring it to its users. Just as we struggle to make a simple cup of coffee due to the machine's complexity, stakeholders can be overwhelmed by an AI system that doesn't consider their needs and expertise. It's like a skilled barista designed the system from their expertise, without tailoring it to us. For effective integration, just like the coffee machine needing a user-friendly interface to truly benefit us, an AI system must be designed with intuitive and accessible features that align with the stakeholders' requirements, making the technology a helpful tool rather than a hurdle.

## 3. Scenario: the Smell Nice Shop

00:00 - 00:00

Take the scenario of a fictional company called the 'Smell Nice Shop'. At the shop, they want to make sure they have enough stock in their shop. Traditionally, they rely on simple past sales data to decide on stock quantities. Based on the sales of the last few weeks, the shop could decide to buy 160 bottles of shampoo. For the shop, the historical sales are an easy to understand, tangible factor, on which they base their expected required stock.

## 4. Scenario: the Smell Nice Shop

00:00 - 00:00

By leveraging an AI system capable of analyzing intricate data, including sales trends and product performances, we can achieve more accurate forecasting. However, the complexity of this AI system might pose challenges. For instance, at the Smell Nice Shop, if the staff responsible for stock inventory lacks a technical background, they might find it difficult to grasp the AI's forecasting logic. This could potentially erode their confidence in and willingness to rely on the system.

## 5. Scenario: the Smell Nice Shop

00:00 - 00:00

At the Smell Nice Shop, an XAI-enhanced system could demystify the AI's stock level predictions by clarifying how different factors impact sales, effectively turning AI from an enigmatic 'black box' into a clear, interactive aid. Imagine an AI system at the shop that not only forecasts shampoo sales but also illustrates the factors influencing these sales. This kind of transparency in AI's reasoning is a prime example of how XAI can enhance AI utility. By comprehending the AI's logic, the shop owner can quickly identify inaccuracies in the AI's predictions, simplifying the process of refining the system. The ability to provide targeted feedback on the AI's decisions streamlines its improvement. Furthermore, XAI opens up the world of AI to non-technical shop staff by unveiling the extensive data and considerations behind AI's conclusions. This insight helps them recognize overlooked variables, improving decision-making and fostering a view of AI as a valuable collaborator that enhances their own skills.

## 6. Let's practice!

00:00 - 00:00

Now that we've seen an example of how important it is to make the AI system understandable to the end-user, let's go into some exercises'

![Pasted image 20240428172004.png](/img/user/Pasted%20image%2020240428172004.png)

Excellent choice! This option perfectly illustrates the application of XAI by making the AI's decision-making process transparent and understandable through interactive visuals. This approach not only builds trust but also enhances the collaborative relationship between the user and the AI system, embodying the user-centric nature of XAI.

![Pasted image 20240428172048.png](/img/user/Pasted%20image%2020240428172048.png)

Well done! You've correctly identified the potential risks of not incorporating the end-user perspective from the very beginning of AI system development for retail inventory management. Understanding these risks highlights the importance of involving end-users in the design process to ensure the AI system is not only technically sound but also user-centric, transparent, and aligned with the actual needs of those it's intended to serve.

# Lesson 2 - XAI by design

## 1. XAI by design

00:00 - 00:12

Excellent work on the course thus far. Now that we've seen how XAI allows AI systems to be more tailored to the end-user, we will look into how we can further incorporate XAI by design.

## 2. Scenario: the Smell Nice Shop

00:12 - 00:36

In the context of the Smell Nice Shop, where they are tasked with determining the necessary shampoo stock, we can explore the application of explainability by design. Initially, we outline the existing workflow. Weekly, the staff estimates the needed stock based on past sales and intuition. Despite these efforts, there are occasions when their predictions miss the mark.

## 3. Scenario: the Smell Nice Shop

00:36 - 01:07

During our pilot at the Smell Nice Shop, we deployed an AI system that markedly enhanced the accuracy of stock level predictions. Together with the shop, we decided to implement this AI tool to forecast the necessary inventory. Although the AI system frequently delivers accurate predictions, there are moments when its estimates are significantly off. In these instances, it's vital for the staff to analyze and understand why such discrepancies occurred in the AI's forecasts.

## 4. Scenario: the Smell Nice Shop

01:07 - 01:22

If we use a very complex model, such as a deep learning model, it can detect intricate patterns between all the different variables. This might make the model more precise, but it's hard to pinpoint for the staff working at the shop why the AI system has come to its decision.

## 5. Scenario: the Smell Nice Shop

01:22 - 01:47

If we use a simpler model, for instance a decision tree model, the explanation will be more tangible, even though it might be less precise. This is why, during the development of the AI system, we have to take into account how we can interpret the model. Often, the accuracy is less important for the end user. It can be way more valuable if the staff of the shop understand the AI model's decision making.

## 6. Integrating explainability by design

01:47 - 02:21

From the very beginning of designing the AI system, we have to look at how the shop staff will interact with the system. That's what we call explainability by design. The staff of the Smell Nice Shop will be way more likely to interact with the first system on the left, where we used a simple AI model in combination with XAI techniques. The system on the right could be perfect in predicting the amount of stock required, but it might be too complex for the staff to use. Once we have defined the end user's goals and requirements, we can start selecting the right model for the task at hand.

## 7. Documentation during development

02:21 - 02:47

During the development of AI systems, there should be clear documentation of the data sources, model choices, and the rationale behind these choices. This should make sure that we include all relevant data that could influence the required stock for the shop. This includes looking into the required explainability techniques, such as SHAP. Through using SHAP, we can include feature contributions, as in the shown example.

## 8. Continuous monitoring and improvement

02:47 - 03:12

Because we have implemented the right explainability tools, and the staff at the shop understand the AI decision-making, we can gather feedback on the initial prototype. It could be that the staff sees why the prediction is wrong, for instance because we miss the campaigns of shampoo of the last weeks. This continuous feedback loop helps in continuously monitoring and improving the AI model.

## 9. Determine risks before deployment

03:12 - 03:32

As you deploy the first version of the AI system, we want to make sure to look at ethical considerations. What could be potential risks if the AI system is wrong? What if it predicts a very high number of required shampoo bottles and the staff at the shop do not notice? We want to make sure that we mitigate these potential risks.

## 10. Let's practice!

03:32 - 03:39

Let's look at how to apply XAI by design with some exercises!

![Pasted image 20240428173153.png](/img/user/Pasted%20image%2020240428173153.png)

Great work! This approach is wise because it combines transparency with the ability to explain decisions made by the AI system. It's crucial in hiring processes, where understanding the basis for a decision can help applicants improve or contest decisions if needed

![Pasted image 20240428173315.png](/img/user/Pasted%20image%2020240428173315.png)

![Pasted image 20240428173346.png](/img/user/Pasted%20image%2020240428173346.png)

Superb job! You've successfully sequenced the tasks in designing an AI system while incorporating XAI. By starting with a deep understanding of user needs and systematically building upon that foundation, you've laid the groundwork for an AI system that is not only effective and transparent but also ethically responsible and aligned with XAI principles. This thoughtful approach is key to developing AI solutions that truly serve and empower users.

![Pasted image 20240428173421.png](/img/user/Pasted%20image%2020240428173421.png)

Well done! Providing clear explanations for content recommendations aligns with XAI principles, making the AI's decisions transparent and enhancing user trust.

# Lesson 3 - XAI in action

## 1. XAI in action

00:00 - 00:22

Now we'll delve into how XAI is revolutionizing various sectors, showcasing real-world instances where transparency and interpretability enhance decision-making. We'll examine the dynamic application of XAI, shedding light on the tangible benefits and innovative solutions it brings to diverse industry challenges.

## 2. Computer vision: detecting skin cancer lesions

00:22 - 00:54

A compelling case study is the application of computer vision in diagnosing skin cancer. Traditionally, dermatologists visually examine skin lesions and may perform biopsies to confirm cancer. Now, AI models, trained on thousands of images of skin conditions, assist in identifying malignant lesions with high accuracy. However, the complexity of these models often made their decisions seem like a "black box," raising concerns about reliability and trust.

1. 1 Mahmud, F., Mahfiz, M. M., Kabir, M. Z. I., & Abdullah, Y. (2023). An Interpretable Deep Learning Approach for Skin Cancer Categorization. arXiv preprint arXiv:2312.10696.

## 3. Computer vision: detecting skin cancer lesions

00:54 - 01:42

XAI comes into play by providing insights into how these models arrive at their conclusions. For example, an AI system might highlight areas of a lesion image that were most indicative of malignancy, offering dermatologists a comprehensible rationale behind the AI's diagnosis. This transparency not only builds trust among healthcare providers but also enriches their understanding, enabling more informed decision-making. Additionally, the AI system can provide a confidence score, which is an indicator of how confident the AI system is in detecting the malignancy. In this way, the dermatologist understands the decision-making, and can decide whether or not to intervene with the classification.

## 4. Natural language processing: sentiment analysis

01:42 - 02:18

Natural Language Processing, also called NLP, is a known component of Artificial Intelligence. Instead of analyzing images like we saw in the example of computer vision, we are know focusing in on the analysis of words. We can use sentiment analysis to analyze the sentiment of customer reviews for a shop. If the shop has a large amount of reviews, automatically analyzing the amount of positive and negative reviews can give great insights. The shop could combine this data with the shop assistant schedule to see how each assistant performs.

## 5. Natural language processing: sentiment analysis

02:18 - 03:08

An explanation that could be provided to test and evaluate the model is by addressing what and how much certain words contributed to the classification. In these examples, the amount of transparency highlights how important a certain word was for the classification of the review. Behind the scenes, the AI system provides a probability score to each word and how it contributes to the prediction. So we can see that in a positive review, the words 'passionate', 'knowledgeable', and 'appreciate' were important. Similarly, we can find the words 'expectations', 'didn't', and 'not' contributed to the review being classified as negative. In this way, we can understand the AI's decision-making, and clarify why the model works as it does.

## 6. Let's practice!

03:08 - 03:19

Now that we've seen case studies of how XAI aids in making AI systems understandable, we will apply our knowledge to some exercises.

![Pasted image 20240428173637.png](/img/user/Pasted%20image%2020240428173637.png)

Excellent work! You've successfully categorized the importance and target audience of XAI across healthcare, finance, and retail sectors. Your understanding of how the necessity of XAI varies—from critical life-and-death decisions in healthcare, to balancing business and customer needs in finance, to enhancing user experience in retail—shows a deep comprehension of the subject.

![Pasted image 20240428173723.png](/img/user/Pasted%20image%2020240428173723.png)

Excellent choice! Combining confidence scores with visual explanations offers a clear insight into the model's decisions, enhancing trust and transparency.

# Lesson 4 - Future of XAI

## 1. Future of XAI

00:00 - 00:08

In this final video, we explore the emerging trends, potential challenges, and future directions in the field of XAI.

## 2. Advances in interpretability techniques

00:08 - 00:50

As AI models become more complex, developing innovative interpretability techniques is essential. Future advancements may include more sophisticated model-agnostic methods, enhanced visualization tools, and interactive interfaces that allow users to explore and understand AI decision-making processes in real-time. These innovations aim to bridge the gap between complex AI systems and human interpretability, making XAI more accessible and effective. An example of this is the usage of Large Language Models to simplify Explainable AI. The use of LLMs such as Chat-GPT, could be used to explain an AI's decision making to a larger audience.

1. 1 Mavrepis, P., Makridis, G., Fatouros, G., Koukos, V., Separdani, M. M., & Kyriazis, D. (2024). XAI for All: Can Large Language Models Simplify Explainable AI?. arXiv preprint arXiv:2401.13110.

## 3. Addressing the scalability challenge

00:50 - 01:53

To run XAI techniques such as SHAP requires lots of computations. So the more complex models we run, the more computing power we need to provide explanations. As AI systems are deployed at scale across various sectors, ensuring the scalability of XAI methods becomes imperative. This involves developing efficient algorithms that can provide explanations in real-time for large-scale systems without compromising performance. Future research may focus on optimizing existing XAI techniques for scalability and exploring new paradigms that inherently support large-scale interpretability. The integration of XAI with cloud technologies offers a pathway to scalability and efficiency. By leveraging cloud resources, XAI systems can process vast amounts of data more effectively, while edge computing allows for decentralized, real-time explanations closer to the data source, enhancing responsiveness and reducing latency.

## 4. Cross-disciplinary approaches to XAI

01:53 - 02:57

The future of XAI lies in cross-disciplinary collaboration, bridging the gap between AI technology and insights from social sciences and humanities. Understanding human cognition, ethics, and social dynamics can inform the design of XAI systems that are more aligned with human values, ethics, and societal norms. Collaborations between AI researchers, ethicists, psychologists, and social scientists can lead to more holistic and human-centered XAI solutions. Integrating user experience design principles into XAI systems can enhance their usability and effectiveness. Future XAI systems might employ user experience (UX) design to tailor explanations to different user groups, ensuring that information is presented in an accessible, intuitive, and actionable manner. As we've seen earlier, the user-centric approach in the design of AI systems can improve the adoption and impact of XAI in various applications.

## 5. Future challenges

02:57 - 03:30

As AI and XAI evolve, and the usage of LLMs will increase, so too will the ethical and regulatory challenges. Anticipating and addressing these challenges proactively is crucial. This includes staying ahead of potential privacy concerns, biases in AI systems, and the ethical implications of autonomous decision-making. Ongoing dialogue between AI practitioners, ethicists, policymakers, and the public will be essential to navigate these complex issues.

1. 1 https://artificialintelligenceact.eu/

## 6. Let's practice!

03:30 - 03:37

Let's conclude with some final exercises about the future of XAI

![Pasted image 20240428173817.png](/img/user/Pasted%20image%2020240428173817.png)

Excellent choice! This approach acknowledges the diverse needs of users by personalizing explanations according to their understanding levels. Leveraging psychological insights to design user interfaces can make explanations more accessible, engaging, and reassuring, which aligns with ethical standards of care and transparency.

![Pasted image 20240428173914.png](/img/user/Pasted%20image%2020240428173914.png)

Well done! You've recognized the multifaceted approach needed to address the ethical and regulatory challenges in AI and XAI technologies. Incorporating a robust feedback loop ensures the system remains adaptable and responsive to user concerns and biases, while integrating human oversight for critical decisions respects the complex nature of ethical responsibility. Your choices reflect a deep understanding of the importance of balancing technological advancements with ethical considerations and human values, essential for developing trustworthy and effective AI systems.

# Lesson 5 - Recap

## 1. Recap

00:00 - 00:03

Well done on completing the course!

## 2. Core concepts

00:03 - 00:17

Throughout this course, we've covered a lot of ground. From the basics of why XAI is crucial for transparency, interpretability, and trust in AI systems, to the deep dive into the technicalities that make AI decisions understandable.

## 3. XAI enhances clarity and reliability of AI systems

00:17 - 00:39

Throughout the course, we dove straight into practical applications, illustrating how XAI enhances the clarity and reliability of AI. You've gained insight into crafting AI solutions that not only perform well but also uphold transparency and responsibility, crucial for aligning with real-world ethical guidelines and societal values.

## 4. Unravel AI's black box nature

00:39 - 00:59

Moving through the course, we explored various techniques to unravel the "black box" nature of AI, making its decision-making processes clear. Through exercises and examples, you've seen how these concepts apply to real-world scenarios, enhancing both your understanding and ability to communicate these ideas effectively.

## 5. Key takeaways

00:59 - 01:16

As you move forward, remember the key takeaways: the balance between an AI model's complexity and its explainability, the importance of tailoring AI to its users, and the ongoing need for XAI in making AI more accessible and trustworthy.

## 6. Congratulations!

01:16 - 01:29

Let's take these insights forward and work together to ensure our AI systems are transparent and comprehensible, making technology more accountable and accessible to everyone.
