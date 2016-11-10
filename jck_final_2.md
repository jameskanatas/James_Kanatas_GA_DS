# Project Design Writeup and Approval Template

Follow this as a guide to completing the project design writeup. The questions for each section are merely there to suggest what the baseline should cover; be sure to use detail as it will make the project much easier to approach as the class moves on.

### Project Problem and Hypothesis
* What's the project about? What problem are you solving?

#### James answer: The objective of this project is predicting the likelihood of customer churn based on available data.


* Where does this seem to reside as a machine learning problem? Are you predicting some continuous number, or predicting a binary value?

#### James answer: Predicting a continuous variable -- customer tenure (i.e. days as a customer before churning)


* What kind of impact do you think it could have?

#### James answer: Predicting customer churn will help our business understand user behavior so we can make adjustments to keep customers longer and therefore make more money.


* What do you think will have the most impact in predicting the value you are interested in solving for?

#### James answer: I think the proximity of "order date" to "soccer event" will have the most predictive value (i.e. people who sign up for the product immediately around a soccer game are more likely to churn).


### Datasets
* Description of data set available, at the field level (see table)

#### James answer: CSV file of historical customer orders.  It includes a variety of fields including customer ID, signup date, order date, order platform (e.g. iOS, Android), and more.


* If from an API, include a sample return (this is usually included in API documentation!) (if doing this in markdown, use the javacription code tag)



### Domain knowledge
* What experience do you already have around this area?

#### James answer: I have deep experience with this dataset -- I use it at work at least once a week.

* Does it relate or help inform the project in any way?

#### James answer: Yes, I have an understanding of which data fields are correct and incorrect -- i have spoken with the data provider at length.

* What other research efforts exist?
    * Use a quick Google search to see what approaches others have made, or talk with your colleagues if it is work related about previous attempts at similar problems.
    
#### James answer: We did a very rough "eyeballing" of this problem 6 months ago.  But there was no legitimate statistical methodology around it.
    
    * This could even just be something like "the marketing team put together a forecast in excel that doesn't do well."
    * Include a benchmark, how other models have performed, even if you are unsure what the metric means.

### Project Concerns
* What questions do you have about your project? What are you not sure you quite yet understand? (The more honest you are about this, the easier your instructors can help).

#### James answer: which approach to use -- linear regression, or random forest, etc


* What are the assumptions and caveats to the problem?

#### James answer: I can't think of any implicit assumptions or caveats at this time

* What data do you not have access to but wish you had?

#### James answer: I wish i had access to user usage data (and i may still get access to it!) but it's a Big Data thing, sitting in a redshift database, and I'm not quite skilled enough to run queries on it


* What is already implied about the observations in your data set? For example, if your primary data set is twitter data, it may not be representative of the whole sample (say, predicting who would win an election)

#### James answer: it is implied that the future will look a lot like the past -- practically speaking, it assumes that customers in the future are similiar to customers who joined in the past, which may not be the case (e.g. the die-hard fans already subscribe)

* What are the risks to the project?

#### James answer: the risk is that the business makes an incorrect decision based on this analysis


* What's the cost of your model being wrong? (What's the benefit of your model being right?)

#### James answer: cost of the model being wrong is that we make an incorrect decision regarding the product or the content offering, which could cost out of pocket development costs or content costs, AND we could in fact INCREASE customer churn.  The benefit of the model being correct is the opposite; we make a good decision and make more money.

* Is any of the data incorrect? Could it be incorrect?

#### James answer: Yes some of the data fields are incorrect (e.g. the payment fields).


### Outcomes
* What do you expect the output to look like?

#### James answer: I expect the outcome to generate a prediction, in days, for how long it will take for a given customer to churn, based on how closely to a soccer game, as well as day of week and several other fields, that customer signed up.

* What does your target audience expect the output to look like?

#### James answer: Target audience expects the output to be a churn prediction (in days) for all new customers.

* What gain do you expect from your most important feature on its own?

#### James answer: I don't know!

* How complicated does your model have to be?

#### James answer: Hopefully not very complicated.  Ideally i'll have no more than 4-5 variables.

* How successful does your project have to be in order to be considered a "success"?

#### James answer: Probably pretty successful.  If it tells us something we already felt we knew, then the model needs to show a pretty strong link between inputs and outputs.  However if it contradicts what we feel in our guts, then all the more reason the model needs to show a very strong link!

* What will you do if the project is a bust (this happens! but it shouldn't here)?

#### James answer: I'll go back and try to obtain the customer usage data (which would tell me WHAT PROGRAMS the customer actually watched, instead of just when they signed up)

