# Prompt Engineering: Building a Better Prompt
There is an entire field dedicated to creating better prompts, otherwise known as prompt engineering. LLMs (and other GenAIs) can't read your mind. Prompt engineering helps ensure the model provides you with useful ouputs. The more context you give to the GenAI when you provide a prompt, the better it will perform for you.

## Zero Shot Prompting
Zero shot prompting refers to giving prompts that are very general and don't provide additional context. It's impressive what tools like ChatGPT can do right out of the box, but you may not get great responses to your prompt.

Prompt: "What are the 5 best restaurants in Chinatown?"
- We ask a general question
- We’re not giving any context
- We’re not saying what it will be used for
- We’re not giving the audience

You *might* get some useful answers with restaurants in NYC, but ChatGPT doesn't know where you are, so it could give a list of places in San Francisco (or anywhere else with a Chinatown!). It could also completely make up restaurant names that sound plausible.

A better prompt: "You are a tourist visiting NYC looking to have a memorable meal and spend less than $100 per person. What are the 5 best reviewed restaurants in Chinatown in NYC? Create a list with the name of the restaurant, the average star review from Yelp, and the address with a link that opens up in Google Maps."
- We ask a more specific question
- We give some context about where we are and what we want
- We specify the format we're looking for

## Helpful Tips
1. **Be Specific:**  GenAI cannot read your mind. Being specific gives context to help you get useful answers. “What’s the best way to get to LaGuardia Airport?” isn’t going to give you as useful of a result as “What’s the fastest way to get to LaGuardia Airport from Washington Heights for a 7:30pm flight? What is the cheapest way?” Instead of “Write a summary of statin guidelines”, specify things you really want. What patient population are you interested in? What format do you want the information in? Who is using this information? How long do you want it to be?

2. **Use Open-ended Questions:**  Forcing the AI to provide “reasoning” allows you to more easily verify outputs. Consider asking ChatGPT to review a study question you've made. How useful would the output be if you asked it, "Is this true or false?" vs. "Review this question and verify if I gave the correct answer by checking with at least 2 sources. Can you explain why this answer is true or false?"

3. **Give Step-by-Step Instructions:** For complex tasks, break down your task into step-by-step instructions to get the best answers. Giving clear, concrete commands helps ensure your outputs are what you want. "First, I will give you some text in square brackets. Summarize the text in one paragraph. Second, create a bullet-point list of key takeaways from the summary you generated."

4. **Give Examples If Possible:** Giving an example of what output you’re looking for is a great way to fine-tune the AI. **However**, if you’re putting proprietary info into the chat, it could be used later for training—make sure you are aware of the risks/implications of this. Be aware of copyrights.

5. **Ask the Model to Adopt a Persona:**:  GenAI can play other roles if you ask it to so you can get better responses. “Create five internal medicine board study questions about infectious diseases using this content outline,” followed by a content outline. But if you added “You are a professor at a prestigious medical school teaching a class to first year residents.” first, the AI will consider this context in its response, adjusting the difficulty of the questions

6. **Define What You Want Your Output to Be:**  You can specify the length and the format you'd like your output to be in, for example, a 10-minute presentation on a topic as a PowerPoint file, a 250-word abstract as a text document, or a table of names and addresses as a CSV file.

7. **Define Your Audience and Platform:**  Specify who this content is for and how it will be consumed (Is this part of a presentation? A handout?). You can also specify the kind of tone you’d want to use (casual, sarcastic, formal, etc).

8. **Ask Follow-up Questions to Refine Your Prompt:** Also known as “prompt chaining”, you can leverage ChatGPT’s “memory” of your current conversation to refine your original prompt and get better outputs. Be aware of the size of context windows-- longer conversations will be "forgotten" if you reach a model's context window limit.

9. **Give Feedback to the AI:** There are built in ways to give feedback to the AI (usually a thumbs up/down), but you can also write in if you want something to be changed. “This presentation is too wordy. Can you make it shorter and tailor it for an audience of 8th graders?” Keep in mind that these instructions won’t persist across multiple chats unless you adjust your settings within your ChatGPT or OpenEvidence accounts.

10. **Ask the AI for Help:**  It feels a bit meta, but you can get some great suggestions this way. Adding questions to the end of your prompt like “What should I ask you to help me do [X]?”, “What other information do you need to do [X]?”, or “What would you suggest I ask you to get a more specific answer?” will give you more info to refine your prompt further.

11.  **Ask the AI to Check for Errors**: Give instructions for the model to check for errors or confirm accuracy. Depending on the task, this could be as simple as saying, "Before displaying your response, check in the source material to make sure you have the correct information."

## Notes
For many models, the free versions will have a limit on the number of tokens you can use in a certain time or the types of analyses you can perform. Each tool will have its own constraints. Try to find out what limits you have so you know what you can expect from your interaction with the GenAI. In ChatGPT for example, when you hit your free limit, the model will switch from the most updated version (GPT 4o or 4o-mini) to an older model (ChatGPT 3.5).

## Table of Contents
- [Getting started](getting_started.html)
- [Best Practices](best_practices.html)
- **Prompt Engineering**
- [Activities](activities.html)
	- [Summarizing an Article](article_summary.html)
	- [Creating a Topic-Specific Overview](topic_overview.html)
	- [Generating a Differential Diagnosis](differential_diagnosis.html)
