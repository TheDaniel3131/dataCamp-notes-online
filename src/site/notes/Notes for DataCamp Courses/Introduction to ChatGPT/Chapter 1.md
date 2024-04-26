---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/introduction-to-chat-gpt/chapter-1/","noteIcon":"","created":"2024-04-26T22:19:10.283+08:00","updated":"2024-04-26T23:01:21.265+08:00"}
---


# Lesson 1 - What is ChatGPT?

## 1. What is ChatGPT?

00:00 - 00:05

Hi! Welcome to this course on ChatGPT!

## 2. What is ChatGPT?

00:05 - 00:16

ChatGPT, by OpenAI, is a chatbot application, which means it can answer questions or perform tasks based on user-inputted text. This may not sound much different to a

## 3. What is ChatGPT?

00:16 - 00:45

traditional chatbot, but ChatGPT is much more than that. Traditional chatbots were usually designed to return a predetermined response to a limited number of questions. ChatGPT is far more generalizable, as it uses its understanding of language to interpret the question or task and determine the most appropriate response. This means that ChatGPT has a wide range of potential applications.

## 4. Generative AI

00:45 - 01:03

ChatGPT uses generative AI to respond to users. Generative AI is a subset of artificial intelligence, or AI, and machine learning, where a model creates new content based on patterns in information it has already seen.

## 5. From prompt to response

01:03 - 01:11

This is how ChatGPT works: the user writes a question or instruction, which is more generally called a prompt.

## 6. From prompt to response

01:11 - 01:23

This prompt is passed as an input to the application, which uses its understanding of language to interpret the prompt and generate new, relevant language in response to it.

## 7. From prompt to response

01:23 - 01:31

Finally, the response is returned to the user. Let's see ChatGPT in action with some examples!

## 8. Summarizing text

01:31 - 01:45

ChatGPT is great at summarizing text or explaining concepts for a particular audience, which is useful when summarizing reports for different stakeholders or interpreting complex information.

## 9. Summarizing text

01:45 - 01:51

Let's write a prompt to instruct ChatGPT to summarize generative AI in simple terms.

## 10. Summarizing text

01:51 - 02:09

ChatGPT responds with a summary that contains very few technical details or jargon while still capturing the key points. This is a good start; however, the summary is quite long. It would be better if we could boil it down to two key sentences.

## 11. Summarizing text

02:09 - 02:13

We can ask ChatGPT to do just that!

## 12. Summarizing text

02:13 - 02:35

Notice that we don't have to instruct it to summarize generative AI again; ChatGPT will actually remember the information and context from earlier in the conversation. The ability to remember the conversation history, and for the user to provide follow-up corrections to responses, are two of ChatGPT's most powerful capabilities.

## 13. Creating marketing content

02:35 - 02:52

Summarizing text or concepts is pretty cool, but ChatGPT can also perform more creative tasks, such as creating marketing content. Let's ask ChatGPT to write a tweet encouraging people to acquire data literacy skills.

## 14. Creating marketing content

02:52 - 03:22

This tweet is pretty good: ChatGPT came up with a catchy slogan (Unlock the power of data!), considered X's character limit, and utilized relevant hashtags and emojis to improve audience engagement. ChatGPT is already being applied to streamline many different marketing tasks, including creating email templates, writing blog post titles and descriptions, and copyediting large bodies of text.

## 15. Generating and debugging code

03:22 - 03:40

ChatGPT is also impacting how software engineers, data practitioners, and others write code. ChatGPT is able to generate template code, explain why code isn't working, and even make suggestions for improvements!

## 16. Why utilize ChatGPT?

03:40 - 04:30

So why should we begin implementing ChatGPT into our workflows and business processes? ChatGPT is able to perform many time-consuming tasks with greater efficiency. Using our own expertise, we can then verify and finalize the responses. This workflow of AI doing the legwork and a human providing the finishing touches saves a substantial amount of time and money. Take the example of using ChatGPT to generate marketing content: this will allow marketers to focus on more complex and nuanced tasks, such as deciding what to market and to whom. Implementing ChatGPT into products will also allow for greater personalization of content, delivering more value to customers.

## 17. Let's practice!

04:30 - 04:35

Head on over to the exercises to test your understanding!

![Pasted image 20240426222024.png](/img/user/Pasted%20image%2020240426222024.png)

Great job! ChatGPT is definitely capable of performing some impressive feats. Head on over to the next exercise to test your understanding of how it works!

![Pasted image 20240426222115.png](/img/user/Pasted%20image%2020240426222115.png)

Awesome! ChatGPT's ability to answer questions or perform tasks using only a text input significantly lowers the entry barrier for users.

![Pasted image 20240426222636.png](/img/user/Pasted%20image%2020240426222636.png)

Excellent business acumen! ChatGPT has the potential to redefine how businesses operate, and the products and services they provide. In the next video, we'll discuss some of ChatGPT's limitations to inform how to use it safely and appropriately.

# Lesson 2 - Limitations of ChatGPT

## 1. Limitations of ChatGPT

00:00 - 00:00

Although ChatGPT is a valuable tool that can perform a huge variety of tasks, there are some limitations to be aware of to use it effectively.

## 2. ChatGPT under the hood

00:00 - 00:00

ChatGPT's text-generation capabilities come from a large language model, or LLM, which sits at the heart of the application. The LLM interprets the prompt and generates relevant text in response based on its understanding of language. To understand some of the limitations of ChatGPT, we'll first need to delve a little deeper into how the LLM works.

## 3. Demystifying the LLM

00:00 - 00:00

Imagine we've been shown a large and complex building block wall,

## 4. Demystifying the LLM

00:00 - 00:00

and then we've been given an incomplete wall to finish off in the same style as the large wall. This, in essence, is how ChatGPT works.

## 5. Demystifying the LLM

00:00 - 00:00

When developing ChatGPT, the LLM was shown a huge amount of text data, which is like the large building block wall. From this data, it develops its understanding of the structure of language by looking at the relation between characters, words, and sentences, which are like the differently-colored building blocks. The data that the model learns from is called

## 6. Demystifying the LLM

00:00 - 00:00

the training data, and the sheer amount and diversity of data used to train ChatGPT is a large part of its success. The model itself used complex

## 7. Demystifying the LLM

00:00 - 00:00

algorithms to detect these language patterns in the training data, and it was

## 8. Demystifying the LLM

00:00 - 00:00

fine-tuned through iterative processes that included rating the quality of the responses.

## 9. Demystifying the LLM

00:00 - 00:00

So when we provide a prompt to ChatGPT, it is essentially trying to complete a building block wall using its understanding of the training data to generate the words most likely to follow the prompt.

## 10. Limitation 1 - Knowledge cutoff

00:00 - 00:00

This leads us to our first limitation: ChatGPT was trained on data up to a certain date, which differs depending on the model used. Without being directly provided with additional context, these models will have no knowledge of events passed these dates. As OpenAI updates the LLMs used in ChatGPT, these dates will continue to shift forward.

## 11. Limitation 2 - Training data bias

00:00 - 00:00

Another limitation is potential bias in the training data. ChatGPT was trained on a massive text dataset from a variety of sources, including books, articles, and websites, but this data could contain biases. The model may learn these biases and produce biased responses.

## 12. Limitation 3 - Context tracking

00:00 - 00:00

ChatGPT has the ability to build on information and context from earlier in the conversation, so follow-up corrections can be made. However, if the topic of the conversation

## 13. Limitation 3 - Context tracking

00:00 - 00:00

shifts multiple times,

## 14. Limitation 3 - Context tracking

00:00 - 00:00

ChatGPT can struggle to keep track of the context and generate inaccurate or irrelevant responses. A good rule of thumb is to keep a conversation to one topic and create new conversations for different topics.

## 15. Limitation 4 - Hallucination

00:00 - 00:00

Another common issue when interacting with ChatGPT is hallucination, which is when the model confidently tells us inaccurate information. This often occurs when attempting to go beyond ChatGPT's knowledge cutoff or abilities. Hallucinations can be difficult to identify without being able to validate the results, but fortunately, one of the most active areas of LLM development is the identification and reduction of hallucinations.

1. 1 https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)

## 16. Limitation 5 - Legal and ethical considerations

00:00 - 00:00

Let's discuss a limitation on what the user can do. Consider this situation: we ask ChatGPT to write a new song in the style of our favorite artist. ChatGPT generates a song that resembles the style of this artist based on the song lyrics that were present in the training data, but who owns this new song? Is it the user that wrote the prompt,

## 17. Limitation 5 - Legal and ethical considerations

00:00 - 00:00

the artist that wrote the original lyrics,

## 18. Limitation 5 - Legal and ethical considerations

00:00 - 00:00

or OpenAI, the creators of ChatGPT? It's easy to fall into one of these legal gray areas if the use cases for ChatGPT aren't properly scoped so that ownership and legal implications are well-understood and accepted. We'll discuss ownership and privacy in much more detail later in the course.

## 19. Let's practice!

00:00 - 00:00

Understanding these limitations will help inform how we can use ChatGPT effectively and responsibly. Time to practice!

![Pasted image 20240426222856.png](/img/user/Pasted%20image%2020240426222856.png)

Great job! From these observations, you're probably already beginning to see where some of the key limitations of ChatGPT might be. Head on over to the next exercise to begin identifying them!

![Pasted image 20240426223003.png](/img/user/Pasted%20image%2020240426223003.png)

Excellent work! Understanding the limitations of ChatGPT will allow you to identify appropriate use cases and avoid some of the common pitfalls.

![Pasted image 20240426223104.png](/img/user/Pasted%20image%2020240426223104.png)

Fantastic! The recency of this event means that ChatGPT won't have sufficient context to generate an accurate post. Later in the course, we'll use these limitations to create a framework that will help you make decisions on appropriate use cases.

# Lesson 3 - Writing effective prompts

## 1. Writing effective prompts

00:00 - 00:02

Welcome back!

## 2. Garbage in, garbage out

00:02 - 00:22

Have you heard the phrase garbage in, garbage out? This has never been more appropriate than with using ChatGPT - if the prompt we provide doesn't contain sufficient context or isn't written in an easily-interpretable way, chances are it will lower the quality of the response.

## 3. How does ChatGPT interpret a prompt?

00:22 - 00:38

To begin forming a set of guiding principles for writing effective prompts, let's discuss how ChatGPT interprets prompts using an example. Here, we're asking ChatGPT to write a job description for a data scientist based in New York.

## 4. How does ChatGPT interpret a prompt?

00:38 - 00:55

First, ChatGPT identifies the broad topic of the prompt. In this case, the phrases job description, data scientist, and New York help the model identify that the prompt is about a job description for a specific role and location.

## 5. How does ChatGPT interpret a prompt?

00:55 - 01:15

Next, ChatGPT attempts to understand what the prompt is requesting. In this case, the verb, write, and job description indicate the task being given to ChatGPT. Data scientist and New York provide additional context to help populate the response with relevant information.

## 6. How does ChatGPT interpret a prompt?

01:15 - 01:38

Finally, the response is generated. This isn't bad for a first draft with little specific context. More context could be added to the prompt for greater personalization, such as key role-specific skills and company culture information. Let's use this understanding to begin thinking about best practices for writing prompts.

## 7. Prompt engineering

01:38 - 01:55

Prompt engineering is the process of writing prompts to maximize the quality and relevance of the response. Prompt engineering is a whole topic in itself, so in this video, we'll present the foundational best practices to get the most out of our ChatGPT prompts.

## 8. Writing tips for prompt engineering

01:55 - 02:51

The first guideline is to be clear and specific. This sounds like common sense, but we need to ensure that the prompt contains all of the necessary context to create the desired response. One common ChatGPT use case is asking it to summarize a passage of text. In the prompt, we should specify roughly how long we want the resulting summary to be: one page, one paragraph, or even one sentence. Second, keep prompts concise. This means removing any unnecessary information or linguistic frills that don't provide extra context for the task at hand - these extras will only dilute the important information and keywords. Finally, use correct grammar and spelling in prompts. ChatGPT uses grammar to interpret the task, so make sure to include it in all the right places.

## 9. Provide examples if necessary...

02:51 - 03:33

Another way to superpower our prompts is to provide examples. In many cases, this is a much quicker way of providing extra context than writing a comprehensive explanation of the desired results. For example, let's use ChatGPT to create a list of example customer names, ages, and occupations that we can use to test our internal systems. We want the results in a very specific format: the full name and age separated by a comma, followed by the occupation in brackets. We should provide an example in the prompt so ChatGPT understands exactly what we're asking for.

## 10. Provide examples if necessary...

03:33 - 03:42

In our prompt, we specify the instruction and also provide the example, John Smith, 34, and Builder in brackets.

## 11. Provide examples if necessary...

03:42 - 03:51

Because of the example in the prompt, ChatGPT outputs exactly what we want and in the format that we wanted it.

## 12. Let's practice!

03:51 - 03:58

Now you have the tools to begin writing effective prompts. Time to practice!

![Pasted image 20240426223321.png](/img/user/Pasted%20image%2020240426223321.png)

Perfect! Now that you understand the best practices of writing prompts, head on over to the next exercise to begin applying them!

![Pasted image 20240426223510.png](/img/user/Pasted%20image%2020240426223510.png)
![Pasted image 20240426223614.png](/img/user/Pasted%20image%2020240426223614.png)

Excellent identification! This prompt is information-dense and provides an example to ensure the output is in the format you need for the posters and flyers.

# Lesson 4 - Enabling people to use ChatGPT

## 1. Enabling people to use ChatGPT

00:00 - 00:10

Great work so far! In this chapter, we'll focus on when to use ChatGPT and how to scale its adoption safely and responsibly.

## 2. Augmenting workflows

00:10 - 00:43

In any role, we develop workflows to achieve some end goal through a standardized series of tasks. These workflows are often molded through years of experience, experimentation, and innovation to achieve a high-quality end goal in a timely manner. These workflows inevitably contain some time-consuming and repetitive tasks, but many of these can now be performed by ChatGPT. These augmented workflows can ultimately improve the quality and timeliness of the end goal.

## 3. A standard workflow

00:43 - 01:15

Let's say that we've been scoping a complex project, and the resulting document is thirty pages long. We need to summarize the key findings for other stakeholders, so we decide whether the project gets the go-ahead. The standard workflow here would be for us to scan through the document, extract the key findings, and compile the summary by hand. Then, we might use a spelling and grammar checker to proofread. This process is extremely time-consuming, and minus the spellchecker, we had to do most of the legwork.

## 4. A ChatGPT-powered workflow

01:15 - 01:41

With ChatGPT, the roles of people and technology in this workflow can be reversed. We can ask ChatGPT to summarize the document for us with a well-engineered prompt; then, we proofread the final review for accuracy before sending. This relatively small change provides time savings and allows us to focus our time on more creative and higher-value tasks.

## 5. Who can use ChatGPT?

01:41 - 02:08

So who can benefit from ChatGPT-powered workflows, and which industries? A business is made up of many roles with vastly different workflows, considerations, and measurable outputs. Marketing often generates public-facing content, HR handles sensitive data on personnel, and technical roles in IT, data, or software engineering write complex code or design systems. Fortunately,

## 6. ChatGPT can deliver value to everyone!

02:08 - 02:29

all industries and roles can benefit from integrating ChatGPT into their workflows! ChatGPT's contribution will differ significantly from role to role, and there are some ownership and privacy considerations that we'll discuss later in the course, but let's take a look at some common use cases for these roles.

## 7. Leaders

02:29 - 02:56

Business leaders not only make key decisions to steer the direction of the company but need to communicate the vision and direction to the wider business. Leaders can use ChatGPT to help compose emails, draft presentations, brainstorm strategic ideas, and summarize meeting notes. In these cases, it's still advisable to verify the generated content depending on the complexity and stakes involved.

## 8. Technical roles

02:56 - 03:22

Software engineers, data practitioners, and other technical roles spend a lot of their time writing code, and the typical workflow often includes repetitive tasks like looking up code syntax and writing documentation. These roles can use ChatGPT to recall code syntax and generate examples, explain code, troubleshoot errors, and even write documentation to accompany the code.

## 9. HR and people teams

03:22 - 03:34

HR and people teams can use ChatGPT to brainstorm initiatives for improving employee engagement and well-being and allow them to communicate more effectively and efficiently with other employees.

## 10. Marketing

03:34 - 03:56

Marketing teams are responsible for increasing brand and product awareness. Marketing teams can use ChatGPT to write social media posts, help with copyediting human-written content, and create all types of marketing copy. ChatGPT can even help with optimizing content for search engines if the target keywords are provided.

## 11. Sales

03:56 - 04:24

The goal of sales teams is to acquire new customers, so their workflow often involves communicating with internal stakeholders for product information and also outreach to generate leads and opportunities. Sales teams can harness ChatGPT to generate outreach templates, personalize outreach content for greater effectiveness, brainstorm approaches and strategy, and summarize information from internal stakeholders.

## 12. Let's practice!

04:24 - 04:31

Phew! That was a lot of use cases, and there's even more where that came from!

![Pasted image 20240426224037.png](/img/user/Pasted%20image%2020240426224037.png)

Great spot! The desired workflow is one that has ChatGPT doing much of the legwork, so a person only has to finalize tasks before completion.

![Pasted image 20240426224145.png](/img/user/Pasted%20image%2020240426224145.png)

Great work! This toolbox of use cases can already help you augment your own workflows and save lots of time! In the next video, you'll learn how to identify other use cases for ChatGPT.

![Pasted image 20240426224242.png](/img/user/Pasted%20image%2020240426224242.png)

You've got it! ChatGPT could quite easily misinterpret the prompt, use an undesirable writing style, or even worse, hallucinate information. Ensuring that there's always a human to verify the generated content is a crucial step in the workflow.

# Lesson 5 - Identifying use cases for ChatGPT

## 1. Identifying use cases for ChatGPT

00:00 - 00:02

Welcome back!

## 2. Coming up...

00:02 - 00:23

Deciding when it's appropriate to use ChatGPT isn't easy and requires considering ChatGPT's capabilities and limitations and the requirements of the use case. In this video, we'll provide a framework in the form of key questions to validate the suitability of ChatGPT for a particular use case.

## 3. Validating a use case

00:23 - 00:47

The first question to ask ourselves is if we require a high degree of accuracy in the response? ChatGPT can be inaccurate, and there's no predictability in its response, so two people providing the same prompt often get different responses. If the use case requires certainty in the quality of the response, such as government policy advisory,

## 4. Validating a use case

00:47 - 00:50

ChatGPT would be an unsafe option.

## 5. Validating a use case

00:50 - 01:09

Next, we should evaluate whether someone is able to verify the quality of the response. This is where subject matter expertise still plays a huge part in the workflow. A good rule of thumb is to not ask ChatGPT to do something that we couldn't do ourselves given enough time.

## 6. Validating a use case

01:09 - 01:18

If we can't verify the correctness or quality of the result, it would be irresponsible to begin using it to drive decisions or surfacing it to customers.

## 7. Validating a use case

01:18 - 01:26

The use case may require inputting sensitive data, such as customer's personal information or company source code.

1. 1 https://openai.com/policies/terms-of-use

## 8. Validating a use case

01:26 - 01:48

Enabling a use case involving sensitive data is difficult. We need to acquire the necessary consent to process the data, as well as ensuring that the applicable data governance laws, such as GDPR or CCPA, are being adhered to. For these use cases, it's best to seek legal counsel that specializes in data governance.

## 9. Validating a use case

01:48 - 01:58

Finally, ask whether ownership over the response is required. Ownership will likely be required if we intend to generate revenue from the response.

## 10. Validating a use case

01:58 - 02:18

Providing that users comply with OpenAI's terms of use, they can claim ownership over the output in many cases, but other considerations, such as copyright infringement, may prevent ownership. We'll dive deeper into the legalities and ethics of using ChatGPT a little later in the course.

1. 1 https://openai.com/policies/terms-of-use

![Pasted image 20240426224409.png](/img/user/Pasted%20image%2020240426224409.png)

Excellent! So you now know the key factors to determine the suitability of a use case for ChatGPT; head on over to the next exercise to apply this knowledge and understanding!

![Pasted image 20240426225006.png](/img/user/Pasted%20image%2020240426225006.png)

Great work! Due to the severe implications of breaching data and privacy agreements, this use case requires certainty in the correctness of the output, which ChatGPT can't provide. Head on over to the next video to learn about the ownership and privacy considerations at play when using ChatGPT.

# Lesson 6 - Ownership and Privacy

## 1. Ownership and privacy

00:00 - 00:04

Let's now discuss ownership and privacy in more detail!

## 2. Ownership and privacy

00:04 - 00:22

Ownership and privacy are two key considerations when scoping ChatGPT's suitability for a particular use case. Neglecting to consider these factors, especially for companies, can bring with it financial penalties, lawsuits, and damage to customer trust and brand image.

## 3. Who owns the response?

00:22 - 00:38

We'll first discuss the response, as this is ultimately how value will be delivered to users. Establishing ownership over the response is crucial, especially if we intend on integrating ChatGPT into revenue-generating products.

## 4. Who owns the response?

00:38 - 00:54

As stated in OpenAI's terms of use, providing that users comply with the terms or use and any applicable laws, they can claim ownership to the output. This is great, but before we begin celebrating, let's dig a little deeper into these terms.

1. 1 https://openai.com/policies/terms-of-use

## 5. Who owns the response?

00:54 - 01:46

First, we cannot claim ownership over responses that are considered non-unique, as they can also be generated for other users. If we use a prompt with a small number of likely responses, such as asking factual questions or requesting very short pieces of text, we cannot claim ownership over the response. Second, we can't claim that responses from ChatGPT were human-generated. For products or tools built on top of ChatGPT, we'll need to ensure that customers aren't under the misapprehension that the generated content is human-generated. Finally, ChatGPT can't be used to infringe on a person's rights, which includes copyright infringement. OpenAI update their terms of use fairly regularly, so be sure to double-check them before giving the green light.

1. 1 https://openai.com/policies/terms-of-use

## 6. Ownership and copyright

01:46 - 02:02

Copyright prevents people from using intellectual property without prior consent from the owner. If AI-generated content bears similarity to content protected by copyright, we're at risk of receiving an infringement claim from the owner of the IP.

## 7. Who owns the prompt?

02:02 - 02:06

Now let's discuss ownership over the prompt!

## 8. Who owns the prompt?

02:06 - 02:19

As we might expect, OpenAI's terms state that the user owns the input as far as permitted by the law. Although this addresses ownership over the prompt, there are other considerations to be aware of.

1. 1 https://openai.com/policies/terms-of-use

## 9. Prompt privacy

02:19 - 02:51

OpenAI are continuously developing ChatGPT to improve its performance, and one way this is being achieved is by analyzing user's prompts and responses. If we're interacting with ChatGPT via the browser, and don't want this data being used for performance improvements, we'll need to opt-out in the privacy settings. Inputting sensitive data without the proper consent could risk breaching data governance laws, so it's always important to check the specific terms and applicable laws.

1. 1 https://openai.com/policies/terms-of-use

## 10. Data governance

02:51 - 03:25

Data governance laws govern how data and information can be collected, stored, and used to protect people's personal data. One of the biggest and most established data governance laws is GDPR, which governs data usage impacting EU citizens and residents. Data governance laws already place restrictions on how sensitive data can be used, so any use case for ChatGPT must not only satisfy OpenAI's terms of use but must also adhere to the applicable data governance laws.

## 11. AI ethics

03:25 - 03:53

Aside from the legalities of enabling a use case, we should also stop to consider the ethics. AI ethics is a field dedicated to ensuring that AI is used with people and society's best interests in mind. Although this is a fairly loose definition and not legally binding, we should still ensure that enabling our use case won't adversely impact society and, desirably, bring an overall positive impact.

## 12. Let's practice!

03:53 - 04:00

Grab your gavel; it's time to put your new-found legal and ethical understanding into practice!

![Pasted image 20240426225335.png](/img/user/Pasted%20image%2020240426225335.png)

Fantastic job—you really know your stuff! Understanding ChatGPT's terms of use will allow you to identify concerns about enabling a use case while in the scoping stage, where the investment and associated risk is small.

![Pasted image 20240426225429.png](/img/user/Pasted%20image%2020240426225429.png)

Great work! Recognizing legal and ethical concerns is a key step while scoping ChatGPT's suitability for a use case. Head on over to the next exercise to judge whether a use case can be enabled after considering the legal and ethical impact.

![Pasted image 20240426225518.png](/img/user/Pasted%20image%2020240426225518.png)

Incredible work! That definitely wasn't easy and showed how nuanced enabling ChatGPT can be. By spreading misinformation, this use case doesn't have people's or society's best interest at-heart.

# Lesson 7 - Advancements in generative AI

## 1. Advancements in generative AI

00:00 - 00:03

Awesome work getting this far!

## 2. Coming up...

00:03 - 00:12

In this video, we'll discuss the exciting future of generative AI models, like ChatGPT, as well as some of the key hurdles to overcome.

## 3. Performance improvements

00:12 - 00:43

As with all technological advancements, we expect better performance with time, but let's define what we mean by better performance. Generative AI models produce content, so it's natural to compare what they can produce with what people can. We expect that generative AI models will produce content that much more closely resembles human-generated content. We also expect generative AI models to tackle more complex instructions and questions with greater reliability.

## 4. What's driving the improvements?

00:43 - 01:12

So what will drive these improvements? Recall that ChatGPT, and other text-generating AI models, have a large language model at their heart. The LLM learns patterns and structure in language from being given a huge amount of text data to learn from, which we call training data. Algorithms then detect language patterns by looking at the frequency and order of words in the training data, and finally, the model is fine-tuned through iterative processes that involves rating the quality of responses.

## 5. What's driving the improvements?

01:12 - 01:24

The amount of available training data will continue to increase, so models should develop a deeper understanding of language, including complex language expressions, such as sarcasm and idioms.

## 6. What's driving the improvements?

01:24 - 01:41

Additionally, many generative AI models collect usage data, including user ratings of the generated content. This data allows developers to continue to fine-tune the model while it is live. Let's discuss a few hurdles related to these improvements.

## 7. Building balanced datasets

01:41 - 02:07

Although there will be more training data that models can learn from, a big challenge will be ensuring that the data is balanced and high quality. Due to the sheer quantity and unstructured nature of the training data, reducing bias before training the model is difficult. As generative AI begins to become an integral part of day-to-day life, more robust procedures to mitigate bias will need to be developed.

## 8. Opportunities for misuse

02:07 - 02:35

As AI-generated content becomes more human-like, there will be more opportunities for misuse, such as representing AI-generated content as human-generated or using AI to create malicious content, such as spam emails. Because of the potential for misuse, we can expect governments and lawmakers to take a more active role in AI usage through regulatory measures, which could help or hinder advancements.

## 9. From generalized to specialized

02:35 - 03:11

As we've seen, ChatGPT is able to perform a very broad range of tasks, from generating marketing materials to writing and explaining code. In the future, we'll likely see more specialized models developed to generate content within a narrower scope. An example of this would be a model specifically designed to generate code for specific purposes, like software application development or database querying. More specialized models generally perform better than generalized models, as they're trained on the data most relevant to their application.

## 10. Other types of generative AI

03:11 - 03:32

As well as text generation, generative AI models already exist to generate images, audio, and even video! These models operate under the same principles as ChatGPT, where training data is gathered, and a set of algorithms detects the patterns to develop its understanding, which it uses to generate new content.

1. 1 DALL-E 3

## 11. AI for everyone!

03:32 - 03:53

ChatGPT has opened the door to the wide-scale adoption of generative AI, and a key factor in its success is accessibility. One crucial requirement to continue the adoption of generative AI is ensuring the democratization of AI tools so everyone has access to the benefits of this amazing technology.

## 12. Let's practice!

03:53 - 03:57

Now for the final exercises!

![Pasted image 20240426225715.png](/img/user/Pasted%20image%2020240426225715.png)

Fantastic work! There's definitely a lot to look forward to with advancements in generative AI, all of which will be beneficial to augmenting your workflows. With that, there are some interesting challenges to overcome, so don't expect AI to disappear from the headlines any time soon!

![Pasted image 20240426225824.png](/img/user/Pasted%20image%2020240426225824.png)

Spectacular! Although having more specialized models in the market will be less convenient for the end user, the added performance and capabilities will almost certainly make up for it!

![Pasted image 20240426225902.png](/img/user/Pasted%20image%2020240426225902.png)

Well done! Here's an AI-generated company logo created by OpenAI's image generation model, DALL-E 2. Not bad at all!  
  
![A logo for a tech company generated by DALL-E 2.](https://assets.datacamp.com/production/repositories/6244/datasets/b6265c1f07740e20f9d9bbb3e3c5d1decefc38fa/logo-min.png)  
  
Audio generation is being used heavily for text-to-speech tasks, such as generating narration from a script. Video generation is still in its infancy but could eventually be used for compiling movie trailers or even generating entire scenes from a screenplay.

# Congratulations

## 1. Congratulations!

00:00 - 00:05

Congratulations! You've made it to the end of the course!

## 2. Chapter 1 - Interacting with ChatGPT

00:05 - 00:21

In Chapter 1, you learned the fundamentals of interacting with ChatGPT effectively. You learned about what ChatGPT can do, what some of its limitations are, and how to write prompts to maximize the quality of the response, so-called prompt engineering.

## 3. Chapter 2 - Adopting ChatGPT

00:21 - 00:52

In Chapter 2, you learned how businesses are using ChatGPT to augment their workflows to improve efficiency and value. You understand how to identify new, appropriate use cases for ChatGPT using a framework of four key questions. You've investigated the legal and ethical considerations to regard prior to enabling a use case. Finally, you learned about the key factors that will determine the future success and widespread adoption of generative AI.

## 4. Where next?

00:52 - 01:01

This course is only the start of your AI journey. At DataCamp, we've created courses and learning paths to help you achieve your AI goals.

## 5. Congratulations!

01:01 - 01:09

I hope you enjoyed the course and now feel confident and prepared to begin superpowering yourself with ChatGPT!