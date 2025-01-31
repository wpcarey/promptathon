# Activity: Generating a Differential Diagnosis

## Objectives
- Use ChatGPT or OpenEvidence to generate a differential diagnosis while maintaining patient privacy
- Recognize what constitutes PHI in this context
- Use the model to explain its reasoning

## Important Notes

Generating a differential diagnosis can be a powerful way to use GenAI

**IT IS VERY IMPORTANT TO BE AWARE OF POTENTIALLY VIOLATING HIPAA AND DISCLOSING PHI.**

You should be **EXTREMELY** cautious when using these tools for this purpose, as well as other use cases like drafting letters of medical necessity.

Using vague symptoms is ok, but be aware that the combination of symptoms and/or demographic information and/or date/time/location information can result in patient identification

If your patient could figure out that the prompt is about them, you are disclosing PHI

§Let’s try to generate a differential diagnosis for an imaginary patient with vague symptoms and refine our prompt to get more useful answers

–Patient is a 42yo female with type 2 diabetes and hypertension presenting to the emergency department with right lower quadrant abdominal pain x4 days, fatigue, and headaches.

## Let's Prompt

First round, zero shot:
> Summarize the following article: [https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8218233/)

Can we do a better job? Try coming up with a prompt that might be more useful for you.
