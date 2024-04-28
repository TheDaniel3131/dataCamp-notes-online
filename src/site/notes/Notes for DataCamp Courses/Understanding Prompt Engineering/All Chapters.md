---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/understanding-prompt-engineering/all-chapters/","noteIcon":"","created":"2024-04-26T23:02:55.279+08:00","updated":"2024-04-28T16:26:47.062+08:00"}
---

# Combine Chapter 1 + Chapter 2 + Chapter 3 
# Lesson 1 - A practical demonstration with ChatGPT

## 1. A practical demonstration with ChatGPT

00:00 - 00:00

Welcome to this course on Understanding Prompt Engineering. I'm Alex Banks, your guide through the dynamic world of ChatGPT. Think of this tool as the master key to unlocking your ideas. We're diving right into its practical use.

## 2. A practical demonstration with ChatGPT

00:00 - 00:00

I want to lose fat and gain muscle. But I don't know how. I can start by asking ChatGPT to give me a list of foods I should eat.

## 3. A practical demonstration with ChatGPT

00:00 - 00:00

We start by writing our text, hitting enter, and receiving the output from ChatGPT. But let’s take this one step further.

## 4. A practical demonstration with ChatGPT

00:00 - 00:00

I want to spice things up, quite literally, and combine cuisines to add some excitement to the foods I should be eating. We’ll ask ChatGPT to turn these combinations into a shopping list alongside the necessary cooking instructions.

## 5. A practical demonstration with ChatGPT

00:00 - 00:00

As you can see, we have a serious fusion menu. If we don’t like the suggestions, we can use the ‘regenerate response' button to get different variations.

## 6. A practical demonstration with ChatGPT

00:00 - 00:00

Let’s not just stop here. Let’s take this culinary journey and shift from the practical to the creative.

## 7. A practical demonstration with ChatGPT

00:00 - 00:00

This prompt is especially intriguing for several reasons. First, it demands a leap from the structured world of recipes to the emotive realm of poetry, especially that of Shakespearean caliber.

## 8. A practical demonstration with ChatGPT

00:00 - 00:00

It's a testament to ChatGPT's multifaceted capabilities – from providing structured, practical outputs to creating artistic content that resonates on a deeply human level.

## 9. A practical demonstration with ChatGPT

00:00 - 00:00

Additionally, the request doesn't end with the poem. It goes a step further, asking for a webpage design, a bridge from the world of words into the visual domain of web design.

## 10. A practical demonstration with ChatGPT

00:00 - 00:00

This multi-layered prompt illustrates how we can make connections across diverse and what were once seemingly unrelated tasks – creative writing and coding – into a single query, challenging ChatGPT to produce a holistic, interconnected solution.

## 11. A practical demonstration with ChatGPT

00:00 - 00:00

Such a layered prompt really showcases the spectrum of what ChatGPT can achieve. It's not just about answering questions; it's about embracing an idea, expanding upon it, and weaving it into a tapestry of interconnected outputs that serve a broader vision.

## 12. A practical demonstration with ChatGPT

00:00 - 00:00

I hope this example highlights the capabilities of what prompt engineering with ChatGPT can produce. As you saw in the example, ChatGPT is not just your run-of-the-mill chatbot.

## 13. A practical demonstration with ChatGPT

00:00 - 00:00

The outputs may not be perfect on the first try, it may have errors. Instead of criticizing it, think about the additional context you can provide to get an even better output on the next iteration.

## 14. A practical demonstration with ChatGPT

00:00 - 00:00

That’s what ChatGPT is all about. It’s not “write me an essay on cooking.” It’s about sparring back and forth with the language model, sharing ideas, and examples, and letting it learn your style and preferences until you get the desired response.

## 15. Welcome!

00:00 - 00:00

Now that you’ve seen ChatGPT’s capabilities, let me properly introduce myself. I’m Alex. I’ve been building and scaling AI products since 2021. I also write Sunday Signal, a newsletter covering AI highlights and broader insights that intrigue and inspire. I'm excited to guide you through the world of prompt engineering. You'll discover the tools and techniques to master your interactions with ChatGPT.

## 16. Getting the most out of ChatGPT

00:00 - 00:00

When taking this course, I want you to think of prompt engineering as getting the most out of ChatGPT. A basic prompt leads to a basic answer. But a well-thought-out prompt with rich context leads to capabilities that are powerful beyond measure. Whether you’re summarising text, creating content in your style or even writing code — after combining ChatGPT with effective prompting, your limitations are unbounded.

1. 1 Images: DALLE-3

## 17. Beyond traditional chatbots

00:00 - 00:00

Traditional chatbots work on predefined responses to specific inputs. But for ChatGPT, a chatbot that is tailored for human conversation, levering its understanding of language to discern the best response means you have access to a tool that has the potential to spark your imagination and allow your creativity to take flight.

1. 1 Images: DALLE-3

![Pasted image 20240428160231.png](/img/user/Pasted%20image%2020240428160231.png)

Fantastic job on crafting your prompt! Keep going in the course; there's so much more to discover about prompt engineering beyond just recipes.

# Lesson 2 - What is a prompt?

1. What is a prompt?
00:00 - 00:02
Welcome back!

2. The essence of a prompt
00:02 - 00:23
Every day, we use prompts without even realizing it. When you search on Google, question Siri, or ask a friend for advice, you're using prompts. These are more than just questions — they're gateways to information, insights, and solutions. “What’s the tallest mountain in the world?” “Set a timer for 10 minutes” “What’s the best pizza in London?”

1 Images: DALLE-3, Pixabay, Apple
3. The anatomy of a prompt
00:23 - 01:30
A prompt isn't just a question thrown into the void, expecting an answer. It's carefully crafted, with each word pivotal in guiding the response. Effective prompts typically exhibit three distinct traits: Clarity: A well-defined prompt includes the relevant context to reduce ambiguity. Specificity: The more specific you are, the closer you get to your desired answer. Make sure to avoid any unnecessary information. And finally, open-endedness: Sometimes, allowing the model to think outside the box can yield richer results that were non-obvious from the outset. Let's dissect the earlier example. A lack of clarity might lead to misconceptions about the tallest mountain. On Earth, it’s Mt. Everest, but in our solar system, it’s Olympus Mons, on the planet Mars. Without specificity, if we ask Siri to just “set a timer,” it would likely respond with “For how long?”. And the open-ended nature of asking a friend for their best pizza recommendations invites diverse answers. Leaving room for interpretation often brings newfound creativity.

1 Images: Midjourney, Pixabay, DALLE-3
4. A simple example - clear
01:30 - 01:52
Let's illustrate the importance of clarity, specificity, and open-endedness using a practical example with ChatGPT. Imagine you’re a teacher and you want to design a lesson plan. Clarity: Start by providing ChatGPT with a clear context. Inform it, "I'm an 8th-grade math teacher preparing to teach trigonometry."

1 Image: DALLE-3
5. A simple example - specific
01:52 - 02:01
Specificity: Dive into specifics. Request, "Design a lesson plan tailored for a 60-minute session with 20 students."

1 Image: DALLE-3
6. A simple example - open-ended
02:01 - 02:11
Open-endedness: Encourage creative inputs. Pose a challenge like, "Can you also recommend some creative, real-world examples to make the lesson more engaging for the students?"

1 Image: DALLE-3
7. A simple example
02:11 - 02:20
With these guiding principles, what could have been a generic lesson plan is now transformed into a tailored and stimulating roadmap for your class.

8. The art and science of prompt engineering
02:20 - 02:47
Harnessing ChatGPT’s full potential requires a mix of art and science. This combination is what we call 'Prompt Engineering'. It’s all about writing inputs that maximize the quality of the output. The art lies in understanding the nuances of language, tone, and context. The science is about recognizing the model's capabilities and decoding strategies. Together, they help in sculpting the ideal prompt.

1 Image: Midjourney
9. Common pitfalls when crafting prompts
02:47 - 03:36
Mastering prompt engineering also involves understanding what not to do. While it may seem that any question or statement can serve as a prompt, not all prompts yield effective results. As we journey through this course, you'll learn the nuances that separate a good prompt from a great one, letting you achieve optimal responses from language models like ChatGPT. Just as there are best practices in prompt engineering, there are also pitfalls to avoid: Overloading: Bombarding the model with too much information can dilute the essence of your query. Ambiguity: Being vague can lead to generalized answers. Over-Complication: Using jargon, complex phrasing, or unnecessary technicalities can confuse the model, leading to misinterpretations or overly complex answers.

1 Image: Midjourney
10. Prompt evolution - refinement is key
03:36 - 03:53
Prompts aren’t static. The beauty lies in their iterative nature. Feedback-driven refinement enhances prompt quality, creating a continuous loop of improvement. Think of it as a dialogue, with both user and model striving for perfection.

1 Images: DALLE-3
11. Prompt evolution - refinement is key
03:53 - 04:09
Let’s take that simple example from earlier. We can ask for follow-up messages to ChatGPTs responses to dial in our preferences. In this case, we can ask for more real-world applications of trigonometry within navigation and astronomy.

1 Image: DALLE-3
12. Prompt evolution - refinement is key
04:09 - 04:32
Prompts are the bridge between curiosity and knowledge. With ChatGPT, they become powerful tools, unlocking vast reserves of information and insights. Nonetheless, it’s important to remember to use ChatGPT to augment, not replace, your creativity. Let it be a partnership where you break conventional thinking patterns, ushering in new ideas.

13. Let's practice!
04:32 - 04:44
Now, let's put theory into practice, it’s time for the exercises. Remember, a true prompt guides ChatGPT towards a specific output, steering the narrative.

![Pasted image 20240428160410.png](/img/user/Pasted%20image%2020240428160410.png)

Amazing work! Creating strong base prompts is crucial in prompt engineering, as it lays the foundation for clear and targeted AI responses, ensuring accuracy and relevance in the information you seek.

![Pasted image 20240428160539.png](/img/user/Pasted%20image%2020240428160539.png)

Fantastic! We explore the power of examples and context deeper throughout the course. Context turns ChatGPT and other LLMs into powerful targeted tools.

# Lesson 3 - The Next Level

## 1. The next level

00:00 - 00:00

Welcome to the edge of our conversational AI journey. We’re going to take a glimpse at the seamless integration of ChatGPT into our daily tasks. The upcoming chapters will unfold the capabilities of this tool, transforming the way we engage with information.

## 2. Infusing persona

00:00 - 00:00

When writing prompts, adopting a persona is sometimes helpful. Let’s ask ChatGPT to write a speech to give an address at my university.

1. 1 Image: DALLE_3

## 3. Infusing persona

00:00 - 00:00

As a result, the output is quite generic. It doesn’t know which writing style to follow.

## 4. Infusing persona

00:00 - 00:00

Instead of relying on a generic output, we can ask our trusty friend Ernest Hemingway to write a speech for us.

1. 1 Image: Pixabay

## 5. Infusing persona

00:00 - 00:00

This can help influence output style, audience, length and tone. Four variables we can control to help reach our desired response.

1. 1 Image: Pixabay

## 6. Making it personal

00:00 - 00:00

Soon, you'll see ChatGPT craft emails that echo your personal writing style. Providing examples to ChatGPT is a great way for the model to emulate your writing style. This makes every response resonate with your unique voice.

## 7. Useful ways to structure your prompt

00:00 - 00:00

Throughout this course we’ll learn how to use markdown, an elegant way of structuring text. In addition, the correct use of quotation marks and delimiters will lead to a more tailored input. These are two smart tools you can use that will help remove ambiguity from your prompt, turning a good question into a great one.

1. 1 Image: DALLE-3

## 8. Training techniques

00:00 - 00:00

We'll explore how to harness zero-shot, one-shot, and few-shot learning to guide ChatGPT towards crafting responses that feel personal and intuitive, whether it's recommending movies based on your preferences or mirroring output style.

1. 1 Image: DALLE-3

## 9. Training techniques

00:00 - 00:00

Example Teaser: "If my favorite films are 'Gladiator' and 'Sex and the City', what other movies should I watch?"

1. 1 Images: Wikipedia

## 10. Training techniques

00:00 - 00:00

This will lead ChatGPT to offer you a curated watch list, as if from a trusted friend.

## 11. Training techniques

00:00 - 00:00

ChatGPT’s powers really come alive when we can blend individual interests of wildly different genres. ChatGPT help discern those preferences and offer advice accordingly.

## 12. A helping hand for problem-solving

00:00 - 00:00

Beginning to solve a problem alone can often seem like a monumental task. You’re often left scratching your head. Luckily, a technique called ‘chain-of-thought’ prompting can turn ChatGPT into your helpful assistant. Chain-of-thought works by getting ChatGPT to break down a task into its subsequent steps. This can be done via (i) Zero-shot. Not providing any examples and asking ChatGPT for the problem-solving guide, or (ii) One/few-shot. Providing one or more examples of a framework that ChatGPT can use to tackle the problem.

1. 1 Image: DALLE-3

## 13. Limitations

00:00 - 00:00

As with any tool, ChatGPT has its limitations. Understanding these conditions will help you recognise things like: Biases — The model presents stereotypes or misinformation Hallucinations — The model confidently states incorrect information Overfitting — The model is only as good as the data it's trained on Building a discerning eye for these shortcomings will help you get the most out of ChatGPT.

1. 1 Images: DALLE-3

## 14. Anticipating complex workflows

00:00 - 00:00

We'll learn to build complex workflows, chaining prompts that guide ChatGPT through multi-step tasks, from drafting business plans to developing content strategies, all tailored to our scenarios.

1. 1 Image: DALLE-3

## 15. Anticipating complex workflows

00:00 - 00:00

"Let's draft a startup plan focused on sustainable technology," will be our entry point into creating sophisticated, multi-part responses that mirror a strategic consultancy session. We can layer this with asks to ChatGPT for frameworks and resources that would’ve otherwise been overlooked.

1. 1 Image: DALLE-3
2. 
![Pasted image 20240428160820.png](/img/user/Pasted%20image%2020240428160820.png)

# Lesson 4 - Structuring a prompt

## 1. Structuring a prompt

00:00 - 00:00

Welcome back to our exploration of ChatGPT.

## 2. Introduction to prompt structure

00:00 - 00:00

Crafting a prompt is like laying the foundation for a building. It sets the stage for everything that follows. Just as a wise builder wouldn't construct their house upon the sand, we must master the art of prompt construction. We're diving deep into the architecture of prompts, understanding the intricacies of their structure, and setting the stage for meaningful interactions ahead.

1. 1 Images source: DALLE-3

## 3. Recap - prompt traits

00:00 - 00:00

A lot of people think a prompt is just a simple sentence like “make this better”, “summarise this text” or “correct my writing”.

1. 1 Images source: DALLE-3

## 4. Recap - prompt traits

00:00 - 00:00

However effective prompts typically exhibit three distinct traits: Clarity: A well-defined prompt includes the relevant context to reduce ambiguity. Specificity: The more specific you are, the closer you get to your desired answer. And finally, open-endedness: Sometimes, allowing the model to think outside the box can yield richer results that were non-obvious from the outset. In this lesson, we’re going one step deeper and define the five elements that can turn a good prompt into a great one. Let’s explore.

1. 1 Images source: DALLE-3

## 5. Elements of a prompt - instructions

00:00 - 00:00

In order to have a good prompt, at least one of the following elements should be present. Make your instructions clear to reduce ambiguity. Instead of “What is the name of the monarch?” which assumes the country, ask “What is the name of the current monarch in Denmark” This narrows down the response domain.

1. 1 Images source: DALLE-3

## 6. Elements of a prompt - persona

00:00 - 00:00

When writing prompts, adopting a persona is sometimes helpful. This can help ensure the model’s output is specific, relevant and useful to the target audience. Instead of “Write me a short story” which is a very broad statement, ask “You are J.K Rowling. Write me a short story about magic”. ChatGPT now adopts J.K Rowling’s writing style for your short story, leading to a much higher quality output.

1. 1 Images source: DALLE-3

## 7. Elements of a prompt - output format

00:00 - 00:00

We can ask for a summary, detailed explanations or even checklists. Let’s start with a simple prompt. “I’m applying for a job as a data scientist. Create a checklist for how I can best prepare.”

1. 1 Images source: DALLE-3

## 8. Elements of a prompt - output format

00:00 - 00:00

By specifying your desired format, ChatGPT understands the output style and tailors the result appropriately. Output controls are a critical element to help guide the model’s response through specifications. We’ll dive deeper into this later.

1. 1 Images source: DALLE-3

## 9. Elements of a prompt - context

00:00 - 00:00

We can give ChatGPT background information surrounding the topic at hand. “Here's the transcript from "How to Breathe Correctly for Optimal Health, Mood, Learning & Performance" by the Huberman Lab podcast. What does it say about physiological sighs?”

1. 1 Images source: DALLE-3

## 10. Elements of a prompt - context

00:00 - 00:00

ChatGPT is able to quickly locate relevant insights within large bodies of text that would typically take humans hours to do.

## 11. Elements of a prompt - examples

00:00 - 00:00

Proving examples to ChatGPT is a great way for the model to learn style and tone — especially if you want to emulate the writing style of your own or somebody else. "Here’s an example of a typical email response in my writing style: {insert example email}. Use my writing style demonstrated in the example email to reply to the following message: {insert email you want to respond to}.” This is perhaps one of my favourite prompting techniques. Getting ChatGPT to learn your writing style and persona - a powerful tool when used correctly.

1. 1 Images source: DALLE-3

## 12. Let's practice!

00:00 - 00:00

As you craft your prompts, clarity should be your compass. A well-defined, concise prompt often paves the way for a more insightful and relevant output. Engage with our exercises, where you'll experiment with different prompt structures. As you'll find out, a simple change in question or instruction can elicit entirely different responses from ChatGPT. It's all in the art of asking.

![Pasted image 20240428161118.png](/img/user/Pasted%20image%2020240428161118.png)

Correct! The approach to delivering the instructions as a third grade teacher is a persona element, which influences the style of the explanation.

![Pasted image 20240428161218.png](/img/user/Pasted%20image%2020240428161218.png)

Correct! The prompts lack additional background information about the task.

# Lesson 5 - Output control techniques

## 1. Output control techniques

00:00 - 00:02

Welcome back!

## 2. Output control techniques

00:02 - 00:23

Harnessing the true potential of Language Models like ChatGPT isn't just about asking the right questions but also about steering the response in a desired direction. We'll dive deep into techniques that grant you control over the model's outputs. Think of yourself as the conductor of a vast informational orchestra, guiding it to play the exact tune you want to hear.

1. 1 Images source: DALLE-3

## 3. Your guiding acronym

00:23 - 00:59

While ChatGPT's knowledge base is impressive, to truly make the most of it, we need to understand how to guide its outputs. To simplify output control, remember our acronym: SALT. Each letter stands for a different control variable: Style — define the framework; Audience — tailoring the content; Length — brevity or depth, and Tone — covering the mood and feel. Like a chef seasoning a dish, SALT will help you flavor your interactions with ChatGPT, ensuring that the results are always to your taste.

1. 1 Images source: DALLE-3

## 4. Style

00:59 - 01:23

Style isn't just about the format; it's about the framework of your desired response. Asking for a structured output, like a list or a step-by-step guide, can drastically change the information you receive. “Describe the solar system” might give you a paragraph, but “List the planets in the solar system” provides a clear, organised response. By shaping the style, you shape the narrative.

1. 1 Images source: DALLE-3

## 5. Style

01:23 - 01:30

My personal favourite is “Provide a list of steps I need to make the perfect blueberry pancake.”

1. 1 Images source: DALLE-3

## 6. Style

01:30 - 01:34

As we can see, we receive a clear, step-by-step set of instructions.

## 7. Style

01:34 - 01:41

This highlights the importance of specifying your desired output style. I’m saving this recipe for later!

## 8. Audience

01:41 - 02:14

Every audience is unique, with its own set of requirements. A child might need a simple, engaging explanation, while a professional might seek technical details. When we tailor our prompts to our intended audience, we ensure that the content we receive is both relevant and understandable. It's like dressing for the occasion; the content must fit the audience just right. I like to use audience controls if I’m learning a new concept and need a simple explanation. “Explain the concept of machine learning to me like I’m a 5-year-old.”

1. 1 Images source: DALLE-3

## 9. Length

02:14 - 02:33

Whether you want a concise summary or an in-depth analysis, controlling the length of your response is vital. This ensures that the information you receive is as detailed or as brief as you require. An example you could use for this course: “Write me traditional Japanese haiku about the importance of prompt engineering with ChatGPT."

1. 1 Images source: DALLE-3

## 10. Length

02:33 - 02:41

It's the difference between a snapshot and a full-length portrait; both have their uses and with ChatGPT, you get to choose.

1. 1 Images source: DALLE-3

## 11. Tone

02:41 - 02:50

Tone adds color to content. It defines the mood and feel of the response. Whether you're seeking a formal explanation,

1. 1 Images source: DALLE-3

## 12. Tone

02:50 - 02:51

a casual chat,

1. 1 Images source: DALLE-3

## 13. Tone

02:51 - 03:04

or a playful anecdote, setting the tone ensures your output resonates with its intended purpose. It's like choosing the music for a scene in a movie; the right tone can elevate the content and make it truly memorable.

1. 1 Images source: DALLE-3

## 14. Tone

03:04 - 03:32

Here’s a favourite of mine. We’ll ask ChatGPT to “Write a formal letter of recommendation for my friend Lauren applying for a senior data science position. At the end of every paragraph include a humorous sentence about why Mike’s car dealership has the lowest prices you’ll find across the country.” ChatGPT does an excellent job of infusing humor into what is typically a formal piece of writing. Have fun experimenting with this one.

## 15. Let's practice!

03:32 - 03:56

By understanding and applying output control techniques, you're not merely interacting with a model; you're directing a flow of information, ensuring that every response is fine-tuned to your needs. With these techniques in your arsenal, it's time to dive into the exercises. Craft prompts using the SALT framework, observe the results, and refine your approach.

![Pasted image 20240428161353.png](/img/user/Pasted%20image%2020240428161353.png)

Great Job, the response is much longer than 100 words! ChatGPT and other large language models have a difficult time producing responses that fall within extremely tight constraints like specific word counts. Use tight constraints with caution.

![Pasted image 20240428161530.png](/img/user/Pasted%20image%2020240428161530.png)

Correct! Since SALT is focused on influencing the output, we don't introduce specific examples into our prompts. We can rely on other engineering frameworks to utilize examples and craft effective prompts.


# Lesson 6 - Evaluating responses

## 1. Evaluating responses

00:00 - 00:02

Hello again!

## 2. Introduction to evaluating responses

00:02 - 01:06

Every tool has its limitations, and ChatGPT is no exception. ChatGPT has a knowledge cutoff date. This refers to the point in time up to which it has been trained with information. This means the AI model is aware of events, developments, and general knowledge that has occurred up until that specific date. Any new information that emerged after this cutoff date is not included in its training data, and therefore, ChatGPT would not be aware of or be able to provide information on these topics. This limitation can sometimes influence the accuracy of responses. However, through smart prompting, we can navigate this. For instance, if you’re asking questions or retrieving data in your prompt, you can specify: "If you don't know the answer and believe this information is after your cutoff date, specify that you don't know". Whilst this method isn’t perfect, highlighting the importance of cross-referencing data points, it can be a helpful tool to identify where ChatGPT’s limitations lie.

1. 1 Images source: DALLE-3

## 3. The four cornerstones of evaluation

01:06 - 01:36

Engaging with ChatGPT yields a myriad of responses, but it's vital to judge the quality of these outputs. Before delving deep, let's set the stage by understanding the four cornerstones of evaluating responses. Yep, you guessed it, another acronym: LARF. But there’s no joke about its importance; it stands for Logical consistency, Accuracy, Relevance and Factual correctness. This will give you the skills to critically assess the outputs you receive from ChatGPT.

1. 1 Images source: DALLE-3

## 4. Logical consistency - the coherence check

01:36 - 01:50

A response can be accurate, relevant, and factually correct but still lack logical consistency. Imagine you prompt ChatGPT with the question, "What are the benefits and drawbacks of solar energy?" If the model responds by stating:

1. 1 Images source: DALLE-3

## 5. Logical consistency - the coherence check

01:50 - 01:59

Benefits: Solar energy is renewable and sustainable. It can reduce electricity bills. Solar panels require minimal maintenance.

1. 1 Images source: DALLE-3

## 6. Logical consistency - the coherence check

01:59 - 02:28

Drawbacks: The initial investment can be high. Solar energy is weather-dependent. Solar panels require minimal maintenance. Notice the inconsistency? Point 3 appears in both benefits and drawbacks. While it's true solar panels require minimal maintenance (a benefit), it shouldn't also be listed as a drawback. This lack of logical consistency shows the importance of critically evaluating responses to ensure they make logical sense.

1. 1 Images source: DALLE-3

## 7. Accuracy and the hallucination tendency

02:28 - 03:17

While striving for accuracy, it's crucial to be aware of ChatGPT's tendency to "hallucinate" at times. This means the model can confidently state an incorrect answer. Suppose you prompt ChatGPT with, "Who was the first person to walk on the moon?" If ChatGPT replies with, "It was Buzz Aldrin," this would be inaccurate. The correct answer is Neil Armstrong, with Buzz Aldrin being the second person. Even though Aldrin did walk on the moon, the response is not factually accurate concerning the specific question. This illustrates why it's crucial to verify the factual accuracy of responses, especially when they're being used as a source of information. Always cross-reference answers with alternate resources to ensure accuracy.

1. 1 Images source: DALLE-3

## 8. Relevance - meeting the context

03:17 - 03:36

Relevance ensures the response aligns with the context and intent of the prompt. Imagine you ask ChatGPT, "What are the top tourist attractions in Paris?" If the model responds with: The Eiffel Tower Disneyland The Great Wall of China The Louvre Museum Notre Dame Cathedral

1. 1 Images source: DALLE-3

## 9. Relevance - meeting the context

03:36 - 03:52

Notice the odd one out? The Great Wall of China is not in Paris, nor is it a tourist attraction relevant to the question. Whilst this is an extreme example, it highlights the importance of ensuring the response is relevant to the prompt.

1. 1 Images source: DALLE-3

## 10. Factual correctness beyond the cutoff date

03:52 - 04:05

We can encourage the model to be factually correct. Here’s an example: “Are universal basic income trials successful in reducing poverty? Provide your answer by only referencing and citing reliable sources.”

## 11. Factual correctness beyond the cutoff date

04:05 - 04:38

For events or developments after ChatGPT’s cutoff, ChatGPT Plus's browser capability can be a game-changer. It allows the model to pull in relevant and up-to-date information, circumventing the cutoff limitation. This feature can be valuable when you need the latest data or insights. Whilst these examples may change over time, it’s important to avoid blindly trusting answers generated by the model. Developing a critical eye is paramount to effectively evaluate ChatGPT’s responses.

1. 1 Images source: ChatGPT

## 12. Let's practice!

04:38 - 04:58

Equipped with the tools and understanding of ChatGPT's strengths and limitations, it's time to put them to the test. Dive into the exercises, challenge yourself, and critically assess the responses. Remember, every interaction is an opportunity to learn and refine your prompting skills.

![Pasted image 20240428161656.png](/img/user/Pasted%20image%2020240428161656.png)

Amazing! The only way we can know the responses provided are accurate is if we verify important facts and information to make informed decisions.

![Pasted image 20240428161739.png](/img/user/Pasted%20image%2020240428161739.png)

Exactly! Working with large language models often requires that you verify and adjust how your prompt is being interpretted.

# Lesson 7 - Prompt Formatting

## 1. Prompt formatting

00:00 - 00:02

Welcome back!

## 2. Introduction to prompt formatting

00:02 - 00:12

In the realm of interacting with ChatGPT, the way you present your prompt is just as important as the content within it. Think of it as the difference between reading a well-formatted book

1. 1 Images source: DALLE-3

## 3. Introduction to prompt formatting

00:12 - 00:21

and a jumbled manuscript. We'll focus on how to effectively format prompts to ensure clarity, precision, and optimal responses from ChatGPT.

1. 1 Images source: DALLE-3

## 4. The power of markdown

00:21 - 00:38

Markdown offers an elegant and straightforward way to structure text. To create headers in markdown, you can use the hash symbol. The number of hashes indicates the level of the header. This enhances the clarity of your prompts, potentially leading to better responses.

## 5. The power of markdown

00:38 - 01:01

We can also use bold for highlighting. This is done by using double asterisks or double underscores before and after the text you want to bold. This signals ChatGPT to focus on that specific aspect of the prompt. With these simple Markdown tricks, you can make the key points more noticeable and easier to follow, driving ChatGPT towards a more targeted response.

## 6. Quotation marks and their magic

01:01 - 01:32

Quotation marks are another powerful instrument in our prompting toolkit. They serve to highlight specific phrases or content. This allows ChatGPT to distinguish between general and specific references. Let’s look at an example. Tell me about the Great Expectations for this course. The prompt is ambiguous. Is the user asking about the expectations for the course, or are they referencing Charles Dickens' novel "Great Expectations"?

## 7. Quotation marks and their magic

01:32 - 02:02

What about when using quotation marks? Tell me about the "Great Expectations" for this course. By placing "Great Expectations" within quotation marks, it becomes clear to ChatGPT that the user is referring to the novel by Charles Dickens and is curious about its relevance to the course. Quotation marks act as clarifiers. They eliminate confusion and direct focus to where it's intended. This clarity can lead to a more contextually appropriate response.

## 8. Delimiting for distinct input

02:02 - 02:37

Delimiters act as a clear separator within your prompt. An example of this is using triple dashes (---) to indicate distinct parts of the input. By separating your instructions, context, or examples, you guide ChatGPT to process each section independently, leading to a more tailored output. Let's see how this works in practice: You're preparing for a debate on the impact of social media on society. You want both pros and cons, followed by a brief conclusion. Let’s use delimiters in our prompt.

## 9. Delimiting for distinct input

02:37 - 02:46

ChatGPT understands the use of delimiters to separate the output into distinct sections that we can define in the prompt.

## 10. Delimiting for distinct input

02:46 - 02:54

As we can see, the use of delimiters helps in guiding the response structure, making both the prompt and output clearer to view and understand.

## 11. Let's practice!

02:54 - 03:20

In our journey with ChatGPT, we've learned that how we present our prompts is just as crucial as what we ask. By mastering prompt formatting, we not only ensure clearer communication with the model but also enhance the quality of our interactions. Now it’s time for some exercises to test the difference a well-structured prompt makes to help inform ChatGPT’s response.

![Pasted image 20240428161848.png](/img/user/Pasted%20image%2020240428161848.png)

Great! Delimiters in prompts, such as quotation marks or parentheses, do not actually speed up the response time of the model.

![Pasted image 20240428161920.png](/img/user/Pasted%20image%2020240428161920.png)

Great! The differences are very subtle but utilizing quotes can be an important tool when trying to put the final touches on a well crafted prompt.

# Lesson 8 - Training techniques

## 1. Training techniques

00:00 - 00:00

Welcome back to our journey with ChatGPT!

## 2. Introduction to training techniques

00:00 - 00:00

At the core of your interactions lie training techniques. These determine the way the model generates answers. It's crucial to understand the spectrum of zero-shot, one-shot, and few-shot learning. These aren't just cool names. They represent the degree of examples or context we provide ChatGPT before asking our main question. Let's explore these methods.

## 3. Zero-shot learning

00:00 - 00:00

Zero-shot learning is when we throw a question or task at ChatGPT without providing any prior examples. It's like asking someone to dive into the deep end without any practice. But sometimes, diving right in works! For example, let’s ask ChatGPT to write a poem about the tranquility of mountains.

## 4. Zero-shot learning

00:00 - 00:00

In this scenario, the model relies on its extensive pre-training, leveraging the multitude of patterns it has learned to generate a response that fits the prompt. Zero-shot learning showcases the power of language models to respond in novel situations without the need for prior examples.

## 5. One-shot learning

00:00 - 00:00

One-shot is the middle ground. Think of it as showing someone how to do a task once and then expecting them to replicate it. We give ChatGPT one example to guide its response, showing that London is the capital of the UK. Then we ask what is the capital of Japan.

## 6. One-shot learning

00:00 - 00:00

One-shot learning is an echo of human learning, where one example can serve as a powerful template for understanding and action.

## 7. Few-shot learning

00:00 - 00:00

Few-shot learning is where we arm ChatGPT with multiple examples before posing our main query. Here, we ask for the capital of Australia, whilst learning the formatting of placing the country’s flag after the capital city.

## 8. Few-shot learning

00:00 - 00:00

Each example serves as a building block, creating a more nuanced understanding within ChatGPT. We're essentially training the model on the fly, giving it a richer context to grasp the essence of our queries.

## 9. Pattern matching and recognition

00:00 - 00:00

One fascinating aspect of few-shot learning is that ChatGPT becomes more than just an autocomplete tool. It turns into a pattern-matching and pattern-generation engine. ChatGPT understands the structure of the information and generates new content based on recognized patterns you provide. Number one, it starts by analyzing the examples. It then mirrors the underlying patterns. Then finally it creates new ideas.

## 10. Pattern matching and recognition

00:00 - 00:00

The possibilities for few-shot learning are endless. You can feed ChatGPT examples of: your writing style to help construct email replies; also, formatting preferences for reports to ensure consistency across documents; and finally, decision-making frameworks to generate new approaches to problems. Few-shot learning provides the opportunity for ChatGPT to extend beyond a mere respondent and become an extension of our mind.

## 11. Chain of thought (COT) prompting

00:00 - 00:00

Chain of Thought Prompting (COT) is an advanced technique that takes training a step further. Here, we're not just giving examples but a roadmap of how to arrive at the answer. It mirrors the way we are, as humans, approach problem-solving: by breaking down complex tasks into manageable steps.

## 12. Zero-shot COT

00:00 - 00:00

With zero-shot COT, we provide a situation: travelling to space and encountering aliens. We ask ChatGPT to "think step by step."

## 13. Zero-shot COT

00:00 - 00:00

We get a thoughtful breakdown where ChatGPT reasons through the encounters. By prompting ChatGPT to reveal its reasoning, we gain insights into the model's thought process, allowing us to better understand, verify and trust its conclusions.

## 14. One-shot COT

00:00 - 00:00

But when we provide an example using one-shot training, we can teach the model how to approach a particular type of problem. It learns the steps and considerations necessary to reach a conclusion.

## 15. One-shot COT

00:00 - 00:00

In this case, ChatGPT only acknowledges the number of astronauts you had a direct interaction with. This can help prevent errors that might occur if it were to jump directly to the end.

## 16. Let's practice!

00:00 - 00:00

Training techniques aren't just about getting an answer; they're about shaping that answer. Whether you're using Zero-shot for a quick reply, One-shot for guided responses, Few-shot for pattern-driven answers, or COT for methodical solutions, you're in the director's chair, shaping the narrative of ChatGPT's responses. Dive into the exercises and see how different training techniques can dramatically alter the output

![Pasted image 20240428162045.png](/img/user/Pasted%20image%2020240428162045.png)
Exactly! One-shot prompting generally is easier and quicker since it doesn't require as many examples as few-shot, but it may be less precise and adaptable in understanding complex or nuanced tasks.

![Pasted image 20240428162116.png](/img/user/Pasted%20image%2020240428162116.png)

Exactly! Chain of Thought prompts help in breaking down complex problems into simpler steps, making it easier for the AI to generate accurate and detailed responses.

# Lesson 9 - Mitigating model limitations

## 1. Mitigating model limitations

00:00 - 00:00

Hello again!

## 2. Introduction to model limitations

00:00 - 00:00

Every model, regardless of its sophistication, has its set of limitations. These limitations stem from the data it's trained on. By recognizing these, we can craft prompts that navigate around these pitfalls and evaluate outputs with a critical eye.

## 3. The reversal curse

00:00 - 00:00

ChatGPT’s knowledge base is imperfect and often quite strange. This is perfectly demonstrated with a recent viral example, highlighting the reversal curse. Let’s ask GPT-4, the best language model currently available, “Who is Tom Cruise’s mother?” It will respond with “Mary Lee Pfeiffer”, which is correct.

## 4. The reversal curse

00:00 - 00:00

But if you ask “Who is Mary Lee Pfeiffer’s son?”, ChatGPT doesn’t know. As Andrej Karpathy recently highlighted, it shows that ChatGPT’s knowledge is almost one-dimensional. You have to ask questions from a certain direction to get the answer. Unlike understanding a car and its respective components, we still don’t know exactly how language models work.

## 5. Biases - a mirror of Society

00:00 - 00:00

What we do know is that language models learn from vast amounts of data sourced from the internet. Consequently, they can inherit and sometimes amplify biases present in the data. Recognizing biases in outputs is crucial to avoid perpetuating stereotypes or misinformation. If you ask ChatGPT, "Who typically cooks in a household?" and it responds with a gendered answer, it showcases the bias it might have absorbed from historical or cultural data. A more neutral answer would acknowledge that anyone, regardless of gender, can cook in a household.

## 6. Hallucinations - when the model imagines

00:00 - 00:00

Hallucinations in the context of LLMs refer to instances when the model confidently provides information that isn't accurate. It might "imagine" details or facts, leading to incorrect outputs. As models like ChatGPT are improving over time, it can be challenging to show concrete examples. Nonetheless, let’s take a closer look at what a hallucination could look like.

## 7. Hallucinations - when the model imagines

00:00 - 00:00

If you ask: “Who was the only survivor of the sinking of the Titanic?” ChatGPT responds: “The only survivor of the sinking of the Titanic who is widely recognized as such was Violet Jessop.” This is a hallucination. Asking ChatGPT to provide sources of information often leads to correcting itself.

## 8. Hallucinations - when the model imagines

00:00 - 00:00

We can ask the follow-up question: “Can you provide sources? Really think about it.” ChatGPT apologizes for the confusion and highlights the misconception. Recognizing and cross-referencing ChatGPT’s answers is crucial to ensure factual correctness.

## 9. Overfitting - echoing the data

00:00 - 00:00

Overfitting occurs when a model is too closely tailored to its training data, making it less effective at generalizing to new, unseen data. In essence, the model might echo what it has seen in the past, rather than providing a balanced response.

## 10. Overfitting - echoing the data

00:00 - 00:00

An example of overfitting is humor. Comedy challenges large language models like ChatGPT. In June 2023, researchers found that if you ask ChatGPT to tell you a joke, 90% of 1,008 generations were the same 25 jokes. These responses were likely learned during ChatGPT’s training.

## 11. Overfitting - echoing the data

00:00 - 00:00

The model currently sucks at discontinuous tasks that require a creative leap in progress. Examples include writing jokes, developing scientific hypotheses or creating new writing styles. My advice is to stick to incremental tasks. These are solved sequentially, adding more information in a gradual setting. Examples include writing summaries, answering questions or imitating your writing style through techniques such as one-shot or few-shot learning.

## 12. Let's practice!

00:00 - 00:00

Dive into the exercises designed to challenge your understanding of biases, hallucinations, and overfitting. By understanding its limitations, we become better users, ensuring that our interactions with ChatGPT are informed, critical, and productive.

![Pasted image 20240428162236.png](/img/user/Pasted%20image%2020240428162236.png)

Exactly right! In this scenario, the repetition of jokes is a symptom of overfitting, where ChatGPT is echoing familiar patterns from its training data. To encourage more original and creative outputs, you should engage ChatGPT in tasks that require innovative and unconventional thinking.

![Pasted image 20240428162408.png](/img/user/Pasted%20image%2020240428162408.png)

Correct! Actively avoiding stereotypes and promoting a diversity of perspectives in your prompts can help mitigate the biases inherent in the model’s training data, leading to more inclusive and unbiased humor.

# Lesson 10 - Building advanced applications

## 1. Building advanced applications

00:00 - 00:02

Welcome back!

## 2. Introduction to building advanced applications

00:02 - 00:24

As we look into the realm of advanced applications, we'll venture beyond routine Q&A. This lesson will introduce you to chaining prompts, maintaining context over multiple interactions, and constructing complex workflows. By tailoring prompts to fit real-world scenarios, we unlock the huge potential prompt engineering has to offer.

## 3. Chaining prompts for depth and continuity

00:24 - 01:09

One brilliant feature of ChatGPT is that within an individual conversation, each prompt builds upon the previous response. This creates a rich dialogue that uncovers deeper insights and fosters a comprehensive understanding of the topic. For example, our first prompt could be: "What are the latest trends in renewable energy?" We can then ask a follow-up prompt: "How could these trends impact global energy policies?" ChatGPT understands that "these trends" refer to the latest trends in renewable energy. Chaining prompts means building a narrative, where each question or task is a link in a chain that extends the context and depth of the conversation.

## 4. Sustaining context over sessions

01:09 - 01:51

If we’re chaining multiple prompts over time, we want to maintain context. This is like developing a storyline that continues seamlessly across sessions, preserving the flow and nuances of the dialog. For example, in our initial session, we might "Outline the steps to start a small business." In our next session, we can ask: "Considering our previous outline, what legal considerations should we focus on next?" By referencing past interactions within a chat window, we can maintain a thread that enhances the model's ability to provide continuity. What we get is more coherent and contextually relevant advice.

## 5. Advanced workflows for complex scenarios

01:51 - 02:07

Designing workflows with ChatGPT allows us to manage and execute multi-step processes. Let’s use a workflow prompt: "Create a step-by-step guide for conducting market research, then draft a survey based on the guide."

## 6. Advanced workflows for complex scenarios

02:07 - 02:20

This approach leverages ChatGPT's ability to handle layered tasks. What’s more, if we combine this using examples through one-shot or few-shot learning, we can access much richer results.

## 7. Persona-problem-solution framework

02:20 - 03:00

We’ve now explored the essential elements of a prompt, highlighting that a great prompt should use at least one of the following: instructions, persona, output format, context, and examples. One framework I’ve come to love, which runs smoothly like a well-oiled train on tracks, encompassing all of the essential elements of a prompt, is the persona-problem-solution framework. Put yourself in the shoes of a business operator. You have clients who want solutions to some tough leadership questions. How do you go about answering them fast and deliver quality in return? Let’s ask ChatGPT.

## 8. Persona-problem-solution framework

03:00 - 03:49

We start by defining the persona of the language model. In this case, we choose relevant criteria for the problem we are solving: Firstly, an advisor to Ray Dalio, a prominent American billionaire investor and hedge fund manager. Secondly, an expert problem solver for leadership tasks. Thirdly, a detailed prompt writer for large language models. Now ChatGPT has all the relevant context for the nature of the problem it will solve. We then list the problem. This can be a single piece of information or a longer paragraph of text. Here, we provide ChatGPT with a list of struggles our clients face. It’s important we include these in quotations to help convey the exact words or phrases that we want ChatGPT to consider.

## 9. Persona-problem-solution framework

03:49 - 04:27

Now it’s time to highlight a suggested solution structure. This is absolutely critical to get the most out of the language model. If we instead wrote “give me solutions to the problems” the AI has a tendency to go off on a tangent.?Notice how we are hyper-specific and define: Relevant online resources to consider Mental models and frameworks for the problem at hand A reference to Ray Dalio’s book “Principles” to draw additional insights What’s more, we even get the language model to provide a prompt for itself to help solve the problem, reducing the cognitive load we place on ourselves.

## 10. Let's practice!

04:27 - 04:52

Through the exercises, you'll see how chaining prompts, sustaining context, and structuring complex queries can transform ChatGPT from a conversational partner to an invaluable asset in your professional toolkit. If you use these techniques correctly, you’ll be able to see the transformation in the quality and applicability of the responses you receive.

![Pasted image 20240428162510.png](/img/user/Pasted%20image%2020240428162510.png)

Exactly! This approach creates a rich, interconnected dialogue, where each prompt adds depth and continuity, leading to a more comprehensive and nuanced conversation.

# Lesson 10 - Prompt Iteration Tips

## 1. Prompt iteration tips

00:00 - 00:07

Hello again. Welcome to the final lesson of our series, where we refine the art of communication with ChatGPT.

## 2. Introduction to prompt iteration

00:07 - 00:22

Like sculpting clay, the first shape is rarely a masterpiece. Iteration is key. With each adjustment to a prompt, the responses become more precise and useful. Let’s explore how to iterate prompts effectively.

## 3. Principle: encourage deliberate thinking

00:22 - 01:13

ChatGPT benefits from a thoughtful approach to problem-solving. Encouraging the model to engage in deliberate thinking helps not only prevent premature conclusions but also ensures the model fully comprehends the task at hand. Consider a general prompt: "Describe the impact of climate change on polar bear populations.” Now consider a deliberate thinking prompt: "First, consider how climate change affects Arctic sea ice levels. Then, analyze how these changes in sea ice impact polar bear hunting patterns, habitat, and overall population." This example illustrates the importance of prompting ChatGPT to think through each step of a problem, thereby leading to more insightful and accurate responses.

## 4. Tactic: step-by-step instructions

01:13 - 01:51

When approaching complex tasks or seeking detailed outputs, breaking down the prompt into step-by-step instructions can dramatically enhance the depth of ChatGPT's response. By doing so, we're guiding the model through a structured thought process, much like walking someone through a recipe. Instead of the general prompt: “Tell me how to start a garden.” We use the following step-by-step prompt to outline our preferences and areas we want to focus on when starting and cultivating our garden. The step-by-step approach not only structures the response but enriches it with details often overlooked in a more general prompt.

## 5. Tactic: deliberate before deciding

01:51 - 02:33

Push ChatGPT to think before presenting an answer. By instructing the model to deliberate or reason through a problem, you're essentially giving it "thinking time." This often results in a more accurate output, as the model takes a moment to sift through its vast knowledge base. A prompt without deliberation could be: "Is Pluto a planet in our solar system?" But when we include deliberation: "Before answering, think carefully and reason through the history of planetary classifications. Is Pluto a planet in our solar system?" By pushing ChatGPT to deliberate and reason through the information, we’ll often receive a more context-rich response.

## 6. Refining prompts based on model feedback

02:33 - 03:49

Each response from ChatGPT is a feedback loop. This is a chance to refine our prompts for greater relevance. We can sharpen our prompts by paying close attention to the model's response. For example, if we start with the initial prompt: "How can I improve team productivity?" We can leverage ChatGPT’s suggestions to spark new ideas and considerations that were non-obvious to us when we first started. This leads us to our refined prompt based on feedback: "The initial suggestions are valuable, but I'm looking for methods specifically tailored for remote teams that face frequent interruptions and varying time zones. Could you provide strategies under these conditions?" The initial prompt was too broad, leading to general advice. By incorporating specifics from the model's response and adding unique challenges faced by the team, the refined prompt directed ChatGPT to offer tailored strategies that address the complexities of remote work. This method really highlights the iterative nature of communication with AI. The back-and-forth is what our experience leveraging ChatGPT is all about. Engaging with intelligent interfaces to strive for the solution in a step-by-step fashion.

## 7. Refining prompts based on model feedback

03:49 - 04:15

Feedback from the model can guide us to ask better questions. By infusing our prompts with the core elements: instructions; persona; output format, context, and examples. Alongside output control techniques with our famous SALT acronym: style; audience; length; and tone. Iteration allows us to move closer to extracting the answers we seek.

## 8. Path to mastery

04:15 - 04:53

The more you practice, the more intuitive these techniques will become. Remember, harnessing ChatGPT’s full potential requires a mix of art and science. And that’s exactly what understanding prompt engineering is all about. We’re writing inputs that maximize the quality of the output. Sparking creativity, saving you time, and opening the door of opportunity to your next brilliant idea. Thank you for joining me on Understanding Prompt Engineering, I’ll see you very soon.

![Pasted image 20240428162645.png](/img/user/Pasted%20image%2020240428162645.png)

Fantastic job on engineering your prompt! You are ready to wield chatGPT effectively and continue your journey with prompt engineering!