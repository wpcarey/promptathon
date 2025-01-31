# Activity: Summarizing an Article

## Objectives
- Use ChatGPT (or OpenEvidence) to create a summary and journal club outline for an article
- Learn how to refine a prompt to get more useful results
- Understand the importance of critiquing and verifying outputs

## The Task
ChatGPT and OpenEvidence can be very helpful in generating article summaries.

As  an  example, I’m using a [paper we’ve seen before](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/) as part of our Journal Clubs and will ask ChatGPT to generate an outline:

>Wong A, Otles E, Donnelly JP, et al. External Validation of a Widely Implemented Proprietary Sepsis Prediction Model in Hospitalized Patients [published correction appears in JAMA Intern Med. 2021 Aug 1;181(8):1144. doi: 10.1001/jamainternmed.2021.3907]. JAMA Intern Med. 2021;181(8):1065-1070. doi:10.1001/jamainternmed.2021.2626

Depending on the model you’re using, you may have to copy and paste the article directly into your prompt box or attach a file with the content you want summarized. A free text version of the article is available here: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/)

## Let's Prompt
Experimenting with these tools is where you'll learn the most, so open up your LLM of choice and try out some prompts!

Zero Shot Prompt:
> Summarize the following article: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/)

What did your output look like? Was it useful? How can we do this better? Try coming up with a prompt that might be more useful for you.

## Take Two
Using some of the [principles here](prompt_engineering.html), I tried to create a better prompt.

Few Shot Prompt:
> You are an internal medicine resident leading a journal club on this article: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/). Provide an outline of a 30 minute journal club presentation and make sure to address the following questions: 1. Why was the study done? 2. What was the study design? (Use the PICO format) 3. How was the study performed? 4. What are the key findings? 5. What are the strengths and imitations of this study? What kinds of bias might be present in this study? 6. What conclusions can be made?

How did your second attempt go?

Depending on your version model and how you accessed the article, you might have found that the LLM couldn’t access the link and created a generic outline. Because my prompt wasn’t so specific, even after copying in the article text, it only created a generic outline. So, I followed up with: “Please complete the outline using details from the paper.” This did give me something useful, but could I have done this more efficiently?


## Third Time's a Charm
For my third attempt, I made my prompt much more specific to my needs.

A Slightly More Shot Prompt:

> You are an internal medicine resident assigned to lead a journal club
> on this article: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/)
> 
> If you cannot access the full text of the article, stop and tell me.
> 
> Otherwise, provide an outline of a journal club discussion using this
> article in bullet point format as if you were making an outline for a
> presentation based on this article. Make sure to address the following
> questions and answer them using this article: 
> 1. Why was the study done? 
> 2. What was the study design? (Use the PICO format)
> 3. How was the study performed?
> 4. What are the key findings?
> 5. What are the strengths and imitations of this study? What kinds of bias might be present in this study?
> 6. What conclusions can be made? 
> 
> If there are key findings or significant parts of the paper that were
> not covered in these questions, list that information. As part of the
> limitations, include any funding disclosures from the authors if there
> are any. If there are no disclosures, mention that. Provide a list of
> 2 additional questions for discussion about this paper that are not
> addressed in the first 6 questions. Finally, provide a list of 3-4
> possible follow-up project ideas that could stem from this paper.

It's not uncommon for more engineered prompts to be multiple paragraphs, even multiple pages, to get the most efficient result. When developers *charge per token*, it's extremely important to be as specific as possible to get the best result!

## Discussion

Some thoughts to take away from this exercise:
- What did you find most helpful in refining your prompt?
- How accurate was your summary?
- Did you save time compared to reading the article and doing this yourself?
- Did you notice different answers depending on which model you used?

## Table of Contents
- [Getting started](https://wpcrp.github.io/promptathon/getting_started.html)
- [Best Practices](https://wpcrp.github.io/promptathon/best_practices.html)
- [Prompt Engineering](https://wpcrp.github.io/promptathon/prompt_engineering.html)
- Activities:
	- **Summarizing an Article**
	- [Creating a Topic-Specific Overview](https://wpcrp.github.io/promptathon/topic_overview.html)
	- [Generating a Differential Diagnosis](https://wpcrp.github.io/promptathon/differential_diagnosis.html)
