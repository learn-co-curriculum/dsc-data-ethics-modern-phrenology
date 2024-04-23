# AI Phrenology and How to Avoid It

## Introduction
In this course, you will be introduced to a number of data science topics from coding with Python, statistics, databases, natural language processing, and more. Data science is a relatively new field and every day data scientists are challenged with ethical questions for which there are little regulations and precedent to dictate their course of action. 

When you are choosing a topic for a machine learning project, you have a lot of options, particularly when you are a student. As information technology professionals, it is crucial that you use good science to ensure that the insights you report to your stakeholders are based on sound evidence and not __pseudo-science__.

This lesson details some kinds of targets you should _not_ try to build a project around predicting, in order to avoid performing "AI phrenology".

## Objectives
* Define phrenology
* Describe examples of AI projects that resemble phrenology
* List the types of machine learning targets to avoid

## Phrenology

> <table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3_ethics/Phase-0/images/dsc-ethics-p1-rep1-1.jpg" alt="Cover of Phrenology Journal from 1848 that contains an illustration of a human skull divided into subsections that contains the illustrators depiction of different human thoughts represented as humans engaged in various activities, like dancing and studying. The words 'agreeableness' and 'memory' also appear." width=250/>
</td></tr></table>


[Phrenology](https://en.wikipedia.org/wiki/Phrenology) is a type of pseudoscience first introduced in the the late 1700s. Practitioners of phrenology believed that the shapes of bumps on the human skull could tell you information about the person's personality, character, and psychology. Phrenology was used to uphold racist and sexist beliefs that were common at the time, and also to determine what sort of punishment or rehabilitation a person accused of a crime might receive.

Phrenology was already discredited by the end of the late 1800s and is no longer widely in use. However it continues to be a useful point of comparison for modern-day pseudoscience. In particular, [people tend to make comparisons to phrenology](https://www.inputmag.com/culture/lemonade-swears-it-totally-isnt-using-ai-for-phrenology) any time someone tries to predict or analyze some attribute using data that is unrelated to that attribute, the way that bumps on a skull are unrelated to the attributes that phrenologists claimed to be measuring.

## What Not to Predict
Image data (e.g. photos of faces) and text data (e.g. names) tend to be the most susceptible to modern phrenology attempts. This kind of data tends to be widely available, and both businesses and governments might be interested in inferring information about people based on these pieces of data.

### Personality Traits
Trying to predict personality traits based on a face or a name is the AI phrenology that most closely resembles historical phrenology. There is no evidence whatsoever that appearance can predict these things, but that has not stopped some people from trying to predict [trustworthiness](https://www.vice.com/en/article/g5pawq/an-ai-paper-published-in-a-major-journal-dabbles-in-phrenology), [criminality](https://www.americanscientist.org/article/the-dark-past-of-algorithms-that-associate-appearance-and-criminality), and [jobworthiness](https://www.washingtonpost.com/technology/2019/10/22/ai-hiring-face-scanning-algorithm-increasingly-decides-whether-you-deserve-job/).

If you're interested in reading more about the issues with predicting these attributes, check out the links above. The main problem here is not that personality traits are impossible to predict, but that the data being used here is inappropriate for the intended target.

### Sensitive Features

Regardless of the type of input data being used, predicting sensitive features can be an ethical minefield and should only be done in very rare circumstances, if at all. Attempting to predict things like sexual orientation, [ethnicity](https://www.vanityfair.com/news/2019/04/china-created-a-racist-artificial-intelligence-to-track-muslims), and [disability status](https://www.brookings.edu/blog/techtank/2019/10/31/for-some-employment-algorithms-disability-discrimination-by-default/) can bring real-world harm to people regardless of the accuracy of the models being used.

One example of when it might be _appropriate_ to try to predict a sensitive feature is if you are specifically trying to measure disparities or discrimination. For example, researchers studying [disparities in citation counts based on race and gender](https://www.socialsciencespace.com/2021/11/keeping-an-eye-on-who-we-cite-and-who-we-dont/) needed to predict the race and gender of most authors in their database in order to determine if they were being discriminated against.

If you decide to build a model that predicts a sensitive feature because you believe that you have a strong enough reason, try to make sure you consult with the people who might be marginalized on the basis of that feature in order to avoid any unintended harms.

### (Nearly) Impossible to Measure Features
The one other type of feature to watch out for is a feature where the "ground truth" is (nearly) impossible to determine. A classic example of this is ___emotion detection___.

> <table><tr><td>
<img src="https://curriculum-content.s3.amazonaws.com/data-science/images/v3_ethics/Phase-0/images/dsc-ethics-p1-rep1-2.jpg" alt="A grid containing images of a woman. Each square on the grid depicts the woman making a different facial expression. " height=250/>
</td></tr></table>

There are two main ways that a set of photographs can be turned into an emotion detection database:

1. The people being photographed are asked to make a facial expression that represents a particular emotion
2. Data labelers are asked to look at photos and infer emotions from facial expressions

In both cases, what is being measured is a ___proxy___ for the person's emotion, not their actual emotion. You can read more about the ethical challenges of different proxies for emotion [here](https://osf.io/9ad4u/).

## Additional Resources
* [Phrenology's History and Influence](https://www.verywellmind.com/what-is-phrenology-2795251) (web article)
* [Citation inequities in the social sciences: The case of Communication studies - Dr Deen Freelon](https://youtu.be/F3N65rFcawA) (YouTube video)
* [Physiognomic Artificial Intelligence](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3927300) (research paper calling for legislative action)

## Summary

Out of all the options for building a machine learning model, make sure you avoid dabbling in AI phrenology. This means not predicting personality traits based on images or names, not predicting sensitive features unless there is a very good reason, and not claiming you can predict an attribute while actually predicting a proxy for it.
