# Activity: Creating a Topic-Specific Overview

## Objectives
- Use ChatGPT or OpenEvidence to create an overview of a topic
- Use the model to help verify its own outputs through iterative prompting and feedback
- Use context windows to create study tools based on your summary
- Recognize the importance of training data by comparing outputs between ChatGPT and OpenEvidence

## The Task
We already saw how effective GenAI can be at generating summaries for articles, but what if we want an overview of a particular topic?

For this activity, you will pick a topic that you are very familiar with and ask the model to create an overview for you.

As a starting point, a good generic type of prompt might be:

>I am a [TYPE OF LEARNER]. Please provide an overview of [TOPIC] in bullet-point format to be used for [PURPOSE]. Cite all sources in [FORMAT]. Do not use sources that do not exist.

## Let's Prompt
Getting an overview of a topic can be a great way to simplify broad concepts or create a starting point for making study materials.

Zero Shot Prompt:
> Give an overview of statin therapy.

This kind of prompt might work in more fine-tuned LLMs like OpenEvidence, but it may not be helpful with more general tools like ChatGPT. Did you notice any hallucinations in your answer? Were your sources accurate? Did you notice a difference in how useful your outputs were between the two tools? 

## Setting the Stage
By giving a little more context in our prompt, we can make sure our output gives us what we need. It's also a great way to really think about what you are trying to know.

A few shot prompt that you might start out with could be:
> I am a first-year internal medicine resident. Please give me a 5-minute summary of the current recommendations for starting statins in patients over 21. Use tables and bullet points whenever possible. Please cite all references with links.

Can we do a better job? Try coming up with a prompt that might be more useful for you. If you are verifying your outputs, you will probably need to do some back and forth. If you want to see an example of this prompt playing out, you can read a transcript [here](https://chatgpt.com/share/678ff45b-fe50-800f-8ddc-fee05b4e8355). 

## Examining Your Results

What kind of output did you get with the previous prompt? Were you surprised by anything? 

If you read the [transcript from my demo conversation in ChatGPT](https://chatgpt.com/share/678ff45b-fe50-800f-8ddc-fee05b4e8355), you'll see that I:
- Got a table from the 2018 ACC/AHA guidelines (but there are more current guidelines from other sources)
- Got a table of some useful information (not complete but a good reference)
- Received citation for CDC page that did not work
- Had to ask it to fix some broken links

It's easy to accept your output at face value, especially if you aren't as familiar with a topic. What could you do to better assess your result? 

In my case, I: 
- Asked ChatGPT why it gave me the resources it used
- Asked it to provide links to different society guidelines so I could reference them later

I independently looked up this information of course (always verify your output), but the gist of the overview was pretty useful!

## Discussion

- What are some follow-up prompts you could use to make your output more useful?
- How would you make teaching materials based on your output? What would you include in your prompt? (Spoiler alert: will cover this in the future!)
- What considerations should you have when doing a complex task like this?
- What sources would you use to verify the questions and answer choices?
- Did you notice if ChatGPT or OpenEvidence was better at this task? Why?
- What sources would you use to verify your output?

## Table of Contents
- [Getting started](getting_started.html)
- [Best Practices](best_practices.html)
- [Prompt Engineering](prompt_engineering.html)
- [Activities](activities.html)
	- [Summarizing an Article](article_summary.html)
	- **Creating a Topic-Specific Overview**
	- [Generating a Differential Diagnosis](differential_diagnosis.html)
