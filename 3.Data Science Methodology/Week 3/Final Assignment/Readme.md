# Data Science Methodology. Final Assignment. Chosen topic: Emails

In this Assignment, you will demonstrate your understanding of the data science methodology by applying it to a given problem. Pick one of the following topics to apply the data science methodology to:

- **Emails**
- Hospitals
- Credit Cards

You will have to play the role of the client as well as the data scientist to come up with a problem that is more specific but related to these topics.

### Question 1. Which topic did you choose to apply the data science methodology to?

**Answer:**
The chosen topic was Emails.

### Question 2. Next, you will play the role of the client and the data scientist. Using the topic that you selected, complete the Business Understanding stage by coming up with a problem that you would like to solve and phrasing it in the form of a question that you will use data to answer.

*You are required to:*

*Describe the problem, related to the topic you selected.
Phrase the problem as a question to be answered using data.
For example, using the food recipes use case discussed in the labs, the question that we defined was, "Can we automatically determine the cuisine of a given dish based on its ingredients?".*

**Answer:**
Let's say the client is a corporate entity and they have big problems with email spam. Apparently, the standard filters are not sufficient, and the email buffer overflows quickly, preventing the real important emails from being received. The client then asks a data scientist to collaborate with an IT department to solve this problem.

And here we are! Now the first step is to understand the problem - Business Understanding. After performing this step, we realise that the company gets a lot of promotional spam and fishing emails that are aimed to gain remote access to company servers or steal corporate data. The standard filters are not sufficient and, therefore, we need to train a new smart spam-filter which would be able to sort this whole mess.

As a result, we get a problem: a lot of spam.

And we can derive a question to work on: how to detect whether an email is a spam or not automatically?

### Question 3. Briefly explain how you would complete each of the following stages for the problem that you described in the Business Understanding stage, so that you are ultimately able to answer the question that you came up with.

1. Analytic Approach
2. Data Requirements
3. Data Collection
4. Data Understanding and Preparation
5. Modeling and Evaluation

*You can always refer to the labs as a reference with describing how you would complete each stage for your problem.*

**Answer:**

1. **Analytic Approach:**

Basically, we know that for us emails can be in either of two conditions: spam or non-spam — a simple binary situation. From what we have learned during this course, such problems are handled with the classification models. Such a model will then decide if the emails are spam. So at this stage, we determine that we need to classify each incoming email. 

2. **Data Requirements:**

There no other factors crucial to our approach that could be found outside of emails. Therefore, for this stage, we need all the email the company received during some time, both spam and non-spam ones. Emails on their own will give us the necessary information.

3. **Data Collection:**

Luckily, the company's IT team is helping us in this, and we have signed a lot of papers on non-disclosure of corporate info. So, this way, we get access to all the emails within the company. However, as we do not know the relationship between spam and non-spam emails, we also need to collect some emails that belong to both categories from other sources: internet, friends, other companies. This step has to be taken with care if the company work in a niche industry and, as a result, the emails would be particular and introduce bias to our data. Naturally, the data we get might vary in structure.

4. **Data Understanding and Preparation:**

**Data Understanding.**
Well, at this stage, we do our best to understand the content of our data, assess its quality. We can also make a few plots and/or graphs to get a better understanding of how the values are distributed and some first take-aways. Also, we would see if additional data is needed for a better sample or to fill the gaps. Regarding emails, we could see some basic patterns and words which characterize them as spam.

**Data Preparation.**
We need to prepare and clean our data from duplicates, missing values, similar parameters/patterns. We also see which email tags/words/parameters are important to us, and we try to merge the data in a single data frame which have all the crucial and clean parameters. Eventually, this data frame will provide us with the model. 

5. **Modeling and Evaluation:**

**Modeling.**
This stage is performed via various modelling tools and programming libraries. IBM Watson Modeller can also be used. With these tools, we try a variety of algorithms and pick the most accurate and suitable one.

**Evaluation.**
Then we need to see if our model works and sorts the emails into spam and non-spam correctly. We split the data into two sets: training and test. Then we use a training set to build the model, and after that, we test it on our training set of emails to see if it works fine and predicts correctly. We would do a lot of visualisation at this stage to get readable outputs.

The modelling and evaluation steps are very iterative and can be repeated multiple times until the desired outcome is reached. 

Finally, hopefully, in the end, we can provide the company with our model for a spam-filter, and they would be able to solve most of their problems.