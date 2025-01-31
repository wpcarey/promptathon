
# Activity: Generating a Differential Diagnosis

## Objectives
- Use ChatGPT or OpenEvidence to generate a differential diagnosis while maintaining patient privacy
- Recognize what constitutes PHI in this context
- Use the model to explain its reasoning

## Important Notes

Generating a differential diagnosis can be a powerful way to use GenAI

**IT IS VERY IMPORTANT TO BE AWARE OF POTENTIALLY VIOLATING HIPAA AND DISCLOSING PHI.**

You should be **EXTREMELY** cautious when using these tools for this purpose, as well as other use cases like drafting letters of medical necessity.

Using vague symptoms is ok, but be aware that the combination of symptoms and/or demographic information and/or date/time/location information can result in patient identification.

**If your patient could figure out that the prompt is about them, you are disclosing PHI!**

## The Task

Let’s try to generate a differential diagnosis for an imaginary patient with vague symptoms and refine our prompt to get more useful answers.

> Patient is a 42yo female with type 2 diabetes and hypertension presenting to the emergency department with right lower quadrant abdominal pain x4 days, fatigue, and headaches.

## Let's Prompt
When it comes to coming up with a differential diagnosis list, context means a lot.

Zero Shot Prompt:
> What is a differential diagnosis for abdominal pain?

As you can imagine, this general prompt will not yield the most helpful results. If a colleague called you without any context and asked you this question, you would probably not know how to begin to give a useful answer. How would you create a more helpful prompt? What information would you include?

## Getting More Specific
It is imperative to be very cautious when creating few shot prompts related to patient care. It's quite easy to move from a de-identified vignette to something that could potentially disclose PHI.

Here are some examples of few shot prompts and whether they are ok with respect to privacy:

✅ OK: There is not enough identifiable information in the prompt
>What is a differential diagnosis for a middle-aged female presenting to the emergency room with fatigue, headaches, and right lower quadrant abdominal pain lasting for more than 3 days. What questions would you ask the patient to narrow the differential diagnosis?

⚠️ BORDERLINE: With some sleuthing, a person might be able to re-identify this patient because you gave information about co-morbid conditions, when and where you saw them, and more specifics about their duration of symptoms. One could argue this isn't ok at all, depending on how busy the emergency department is and where you are located.
> Give me a differential diagnosis for a middle-aged female with diabetes and high blood pressure that I saw in the emergency room today with fatigue, headaches, and abdominal pain for the last 4 days. What questions would you ask the patient to narrow the differential diagnosis?

🛑 NOT OK: You are giving specifics and a person could re-idenitfy this patient with limited information
> What is the differential diagnosis for a 42yo F with T2DM and HTN presenting to the ED with fatigue, headaches, and RLQ abdominal pain x 4 days? Pt is s/p cholecystectomy in 2019 done at [HOSPITAL NAME].

How do we make this better while still making sure we protect patient privacy?

## A Balancing Act
Hopefully by this point, it's clear that there is a delicate balance between providing context and protecting patient privacy.

A common way to avoid disclosing PHI is by asking questions that will change your differential rather than providing answers to symptoms. For example, instead of saying "the patient is 42 yo", consider what you're trying to assess by providing this information. Do you want to know if they could be pregnant? Instead of saying the patient's age, you could ask, "How would the differential change if the patient was of reproductive age?" 

You can ask broader questions to try and figure out what information you might need to create your differential. You can imagine you and a colleague are having a conversation to try and narrow things down.

Using an extremely broad example, we can get things started:
> You are an emergency medicine resident. You are triaging a patient who has the chief complaint of abdominal pain. What are 5 differential diagnoses for abdominal pain? Which diagnoses would be fatal if they were not identified during this encounter? What questions would you ask the patient to help narrow the differential diagnosis? What other information do you need?”

What would you add to this prompt to get more useful results? I tried out the following:
> You are an emergency medicine resident. You are triaging a patient who has the chief complaint of abdominal pain. The patient is of reproductive age. What are 5 differential diagnoses for abdominal pain? Which diagnoses would be fatal if they were not identified during this encounter? What questions would you ask the patient to help narrow the differential diagnosis? What other information do you need to diagnose this patient? If you would order tests, which tests would you order and how would the results change your assessment?

You might be pleasantly surprised to see the answers that an LLM can generate given this information, but remember that **you must verify the output**. The LLM cannot reason or think, so while it may come up with something that seems plausible, it could be completely false. For example, it might say:
> If the patient could be pregnant, you should ask them if they are pregnant. If they say they are not, a urine pregnancy test is not likely to give additional information and you can rule out ectopic pregnancy as a diagnosis to avoid unnecessary testing.

Obviously this is faulty logic, but it certainly sounds reasonable to the uninformed user!

## The Model Matters
If you've been comparing outputs from ChatGPT and OpenEvidence, you may have noticed certain tasks are easier to do in one vs. the other. 

OpenEvidence is primarily trained on Elsevier's peer-reviewed publications, including journal articles and textbooks. There are pros and cons to using it (some of which you may have discovered in other activities), but a large benefit is it will have more baseline context focusing on accurate medical information compared to something more general like ChatGPT. One nice feature is that below the search bar, you will provide find generic prompts for you depending on what you're trying to learn, which can be extremely helpful in this context.

## Discussion
- How does adding more information to the prompt change your results?
- Are you surprised by how easy it can be to disclose PHI unintentionally?
- What are some other strategies you can come up with to balance specificity with privacy?

## Table of Contents
- [Getting started](getting_started.html)
- [Best Practices](best_practices.html)
- [Prompt Engineering](prompt_engineering.html)
- [Activities](activities.html)
	- [Summarizing an Article](article_summary.html)
	- [Creating a Topic-Specific Overview](topic_overview.html)
	- **Generating a Differential Diagnosis**
