---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/travel-demand-and-behavioural-modeling/notes/02-data-and-space-tdbm/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Notes/02 - Data and Space - TDBM\|02 - Data and Space - TDBM]]

```table-of-contents
```

When trying to model transportation patterns, one of the biggest challenges is the data collection. There are several ways of collecting data:
- **Traffic detection stations**: inductive loop detectors, radars, magnetometers...
- Antennas to capture Bluetooth or Wi-Fi equipped devices
- CCTV image processing (Licence plate recognition, emulation of Traffic Detection Stations)
- Capture of digital footprints (ex: TAGs)
- GPS tracking of fleets
- Telephone [[#Surveys]]

- [?] What is the difference between "inductive loops" and "magnetometers"?
	- [ ] She does not know.

# Surveys

Surveys are an **active data collection process**. Data is collected based on pre-defined questions. When carrying out surveys, only a portion of the population of interest is interviewed. This portion is referred to as the **sample**.

They can be carried out in several ways:
- Calling on the phone
- By mail
- In person

A survey is different from a census because, in a census, the whole population is interviewed. In a survey, the information gathered from the sample is then expanded and associated to the rest of the population. There are several ways of selecting a sample. More information can be obtained in [[#Sample Theory]].

It is higly recommended the use of questionnaire, allowing for standardised, pre-defined questions that should be asked to everyone in the same way.

Some surveys focus on opinions and attitudes, such as election polls. Others are concerned with factual characteristics or behaviours, such as transportation habits, housing or consumer spending.

Questions can be asked in an open or closed format. Closed questions are much easer to interpret than open ended questions. Preferably, for ease of analysis, all questions should have a binary response.

Usually, surveys combine questions of different types.

There are many stages in a survey process:
- Goal setting
- Survey design
- Sampling
- Data collection
- Capture
- Cleaning
- Analysis
- Reporting results
- Decision-making based on the results


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/question-you-should-ask-when-doing-a-survey/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Question you should ask when doing a survey]]

1. Who did the poll?
2. Who paid for the poll and why was it done?
3. How many people were interviewed for the survey?
4. How were those people chosen?
5. What area (nation, state, or region) or what group (teachers, lawyers, Democratic voters, etc.) were these people chosen from?
6. Are the results based on the answers of all the people interviewed?
7. Who should have been interviewed and was not?
8. When was the poll done?
9. How were the interviews conducted?
10. What about phone-in polls or polls on the Internet?
11. What is the sampling error for the poll results?
12. Who’s on first?
13. What other kinds of factors can skew poll results?
14. What questions were asked?
15. In what order were the questions asked?
16. What about "push polls"?
17. What other polls have been done on this topic? Do they say the same thing? If they are different, why are they different?
18. So I've asked all the questions. The answers sound good. The poll is correct, right?
19. With all these potential problems, should we ever report poll results?
20. Is this poll worth reporting?


</div></div>



# Survey types in transportation systems

- [[#Household travel/activity surveys]]
	- These are used to collect data about households or individuals.
	- Nowadays, they are not used anymore to generate Origin/Destination matrixes since they are expensive and we have cheaper alternatives available
	- They only interview a subset of all residents (a sample)
- Vehicle intercept and external station surveys
- [[#Transit on-board surveys]]
- [[#Transit operator - satisfaction surveys]]
- [[#Commercial vehicle surveys]]
- Workplace and establishment surveys
- [[#New sources of mobility data]] (phone data)
- [[#Special generator, visitor surveys]]
- [[#Parking surveys]]
- [[#Revealed versus stated preference]]

```ad-example
title: Example: EMEF survey

[[EMEF\|EMEF]] surveys are done every year in Barcelona. About 10'000 people are interviewed by phone. The survey is about the last working day trip the responder took (it's about the whole day trip)

```

### Household travel/activity surveys

In the 1950/60s, surveys were conducted on a large sample, about 3 to 5% of all households. The goal was to estimate O/D matrixes for region. At the time, TAZs were much larger because computer capacity was limited.

Today, we only interview 2000 to 15000 households (corresponding to about 0.3%). The goal is no longer to obtain O/D matrixes, but to to get dailiy activity pattern sequences

![Schermata 2025-03-05 alle 18.25.30.png](/img/user/allegati/Schermata%202025-03-05%20alle%2018.25.30.png)

### Transit on-board surveys

These are surveys usually conducted by travelling agencies. Some data may already be known beforehand, like count of bourdings, but lack information about customer characteristics, like **frequency of transit trip-making**, vehicle avaialbility, origin-destination...

### Transit operator - satisfaction surveys

These are to quantify the importance of items related to day to day conditions of transit network. For each item, the responders selects a score (from 1 to 10, or on the [[Likert Scale]]).



### Commercial vehicle surveys


![Schermata 2025-03-05 alle 18.30.50.png](/img/user/allegati/Schermata%202025-03-05%20alle%2018.30.50.png)

![Schermata 2025-03-05 alle 18.30.59.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Travel%20Demand%20&%20Behavioural%20Modeling/Notes/Allegati/Allegati/Schermata%202025-03-05%20alle%2018.30.59.png)


### New sources of mobility data

New sources of data collection include:
- Data from social networks
- Data from call detail records (CDR): mobile phone data

This sources are now used to extract OD matrices but do not provide modal data for urban trips, since they are too short.

![Schermata 2025-03-05 alle 18.34.10.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Travel%20Demand%20&%20Behavioural%20Modeling/Notes/Allegati/Allegati/Schermata%202025-03-05%20alle%2018.34.10.png)

```ad-example
title: Example - Nommon

Nommon is an IT company in Barcelona that produces mobility data from Call Detail Records (CDR) and network probe of the Orange telephone operator to generate OD matrices.

It does not include modal split. It does provide trip length estimation and precise timestamps.

```

- [x] Does the CDR relies on phone calls being made, or is the phone connection sufficient? ✅ 2025-03-11
	- [ ] Connection is sufficient. Call is not necessary

### Special generator, visitor surveys

Special generator, visitor surveys are intended for specific demand attraction points like *tourists hotspots*, *big shopping malls*, *airports*.

### Parking surveys

Parking surveys ask about distance to final destination, duration of stay, posted prices vs cost for the individual...

### Revealed versus stated preference

Sometimes we are interested in knowing the factual state of the art. In other occasions, we want to investigate what people think of a new scenario that does not exists yet.

#### Revealed preference

```ad-Definizione
title: Revealed preference

A **revealed preference** is the actual behaviour of the individuals.

```

When we collect data from surveys on actual travel, then we are collecting infromation on revealed preference.

#### Stated preference

```ad-Definizione
title: Stated preference

A **stated preference** is obtained by asking the responders about scenarios that do not yet exist.

```

Responders are asked about hypothetical fictitious conditions, with typical variables strategically defined by means of experiment design and measurign the selected choice by the individuals in different conditions.

Conditions for valid results are:
- Design should be undertaken by expert personnel
- Alternatives should be described realistically and accurately
- The presentation of hypothetical alternatives must be intelligible and concise
- The responses may be choosing an alternative, or establishing a ranking or preference among alternatives
- The order, presentation and number of alternatives/factors is important
- A pilot test is necessary to detect problems in the design

Louviere, J.J., Hensher D.A. and Swait J (2000) [[Stated Choice Methods: Analysis and Application]]. Cambridge Univ. Press, Cambridge

##### Errors in stated preference data

###### Bias statement

The respondent answers, onsciously or unconsciously, what they think the interviewer wants

###### Rationalisation Bias

The respondent tries to be rational in their responses in order to justify their behaviour at the time of the interview.

###### Political Bias

The respondent answers in order to influence policy decisions based on their beliefs about how they can affect the results of the survey.

###### No restriction Bias

When responding does not take into account any restrictions on their behaviour, so that the answers are not real.


# Questionnaire design

Questionnaire design is the process of writing the questions and possible answers.

Questionnaire usually contain:
- **Socioeconomic descriptors of individuals** (gender, age, education, social status, employment status, occupation, residence, family structure, income, wealth, etc.)
- **Contextual descriptors:** highly dependent on the object of study (contextual knowledge, behaviours, etc.)
- **Practices descriptors and opinions**: attitudes, habits, collective membership, etc.

The general organisation, especially the order of questions, is important.

```ad-tip

- go from general to particular
- go from less committed to most committed
- delicate questions must never go at the beginning or at the end
- socio-economic questins go to the end
- use transitional phrases to break the monotony and thematic changes
- first questions are usually strategic and set the tone and predispose the respondent: they must be neutral, pleasant and easy
- Avoid questions conditioning the response to the following questions
- When designing filter questions, try not to frustrate people that do not meet certain requirements

```

The **order** of the questions can influence non-response.

- Employ a simple and suited vocabulary to the type of population studied. Pay attention to the opening words of issues and questions.
- Avoid asking a question so that response involves meeting certain requirements.
- Check the logical structure of the questions: interrogative sentences with negations, double negatives that can lead to ambiguity, misunderstanding and finally observation errors.
- Avoid introduction of two concepts in the same question and double question.
- Avoid loaded terms of affection, value judgments or sentences of different connotations depending on the context because the meaning of the question depending on the context of the individual changes.
- Avoid situations where ambiguities and to the same question can give you the same answer, but for different reasons.
- Authorize **double responses** in closed questions, but at least minimise them since the subsequent statistical analysis is greatly complicated.
- Closed questions (where individuals choose the answer from a list of possibilities) must **cover all possible situations**. Establish, where appropriate, a balance between positive and negative forms, checking the list of good possibilities offered.

# Survey design

Survey design involves:
- Choice of data collection methodology (face-to-face in home or central location, telephone, e-mail)
- [[#Questionnaire design]]
- [[#Sample design]] and analysis planning
- Estimating survey costs


# Statistical issues

There are some possible errors that may occur when analysing data.

First, let's focus on the difference between [[Accuracy]] and [[Precision]]:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/accuracy-vs-precision/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# [[Accuracy vs Precision]]

It is very intersting to look at the difference between [[Accuracy]] and [[Precision]]. This difference is well explained by the following diagram:

![Accuracy vs Precision 2025-03-05 19.34.35.excalidraw.png](/img/user/allegati/Accuracy%20vs%20Precision%202025-03-05%2019.34.35.excalidraw.png)
%%[[Accuracy vs Precision 2025-03-05 19.34.35.excalidraw.md|🖋 Edit in Excalidraw]]%%


</div></div>


Lack of [[Accuracy]] corresponds to a [[#Systematic error]] (or bias) in sampling
Lack of [[Precision]] corresponds to a [[#Sampling error]].

## Sampling errors

There are 2 types of sampling errors that may occur, summarised in the table below:

| Decision\Truth   |    $H_0$ true     |    $H_0$ false     |
| ---------------- | :---------------: | :----------------: |
| **Accept $H_0$** |         ✅         | [[#Type II error]] |
| **Reject $H_0$** | [[#Type I error]] |         ✅          |

These errors occur when we test an hypothesis and, the decision we take based on the p-value ends up being inccorect.

### Type I error

Type I error occurs when the null hypothesis is true, but the sample leads us to reject it.

### Type II error

Type II error occurs when the null hypothesis is false, but the sample leads us to accept it.



# Sample theory

## Sample size

It's important before any investigation to determine the sample size in respect to the population. Keep in mind that there is always a trade-off between the sample size and the resources available.

Sample size depends on various factors:
- Significance level
- Power
- Expected prevalence of factor of interest

### Steps in determining the sample size

- Identify major target study variable
- Determine type of estimate (%, mean, ratio)
- Indicate expected frequency of the target variable
- Decide on desired precision of the estimate (absolute or relative error)
- Decide on acceptable risk that estimate will fall outside its real population value
- Adjust for expected response rate
- Adjust for estimated design effect



## Statistical terminology

### Unit

```ad-Definizione
title: Unit

A **unit** is a single person, household, business that is intended to answer the survey.

```

### Population

```ad-Definizione
title: Survey population

The **population** is the collection of [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Notes/02 - Data and Space - TDBM#Unit\|units]] that the survey result should describe or explain. It's the set that includes all measurements of interest to the researcher.

```

#### Target population

```ad-Definizione
title: Target population

Target population is the [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Notes/02 - Data and Space - TDBM#Population\|#Population]] we are interested in studying.

```


### Sample

```ad-Definizione
title: Sample

A **sample** is a subset of the population for which the survey data is collected

```


### Sampling frame

```ad-Definizione
title: Sampling frame

**Sampling frame** is the list of all sampling [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Notes/02 - Data and Space - TDBM#Unit\|units]] from which the sample is drawn.

```

### Sampling scheme

```ad-Definizione
title: Sampling scheme

The **sampling scheme** is the method of selecting sample units from the [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Notes/02 - Data and Space - TDBM#Sampling frame\|#Sampling frame]].

```


## Why sampling

Sampling is necessary to get information about large popoulations.
- Less costs
- Less field time
- More accuracy - we can do a better job in the data collection
- When it's impossibile to study the whole population

## Sampling schemes

- [[#Probability sampling]]
- [[#Judgment sampling]]
- [[#Quota sampling]]
- [[#Convenience samples]]


### Probability sampling

```ad-Definizione
title: Probability (or random) sampling

**Probability (or random) sampling** is where each object has a known, non-zero probability of being selected.
```

It can produce unbiased results (if no non-response) and it allows for calculation of sampling error (if pairwise selection probabilities known). Most widely accepted sampling method.

It allows application of statistical sampling theory in order to:
- Generalise
- Test hypothesis

And it ensures:
- Representativeness
- Precision

There are several methods in probability sampling:

#### Simple random sampling

In simple random sampling we simply select responders at random from a given list.

#### Systematic sampling

In systematic sampling, we select at random one responder from a given list, then, based on how many responses we need, we select every nth possibility from the list.

#### Stratified sampling

In **stratified sampling** we divide the population in strata (same age-group, same occupation...), then we draw a random sample from *every* stratus.

![Schermata 2025-03-06 alle 12.18.17.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Travel%20Demand%20&%20Behavioural%20Modeling/Notes/Allegati/Schermata%202025-03-06%20alle%2012.18.17.png)

- [p] Can acquire information about the whole population **and** of the individual strata
- [p] Precision is increased if variability within strata is less than between strata
- [c] It can be difficult to identify strata
- [c] Loss of [[Precision]] if there is only a small numbers of individual in a stratus


#### Cluster sampling

In cluster sampling, we dived the population in clusters, select some clusters at random, then survey every unit in each cluster.

![Schermata 2025-03-06 alle 12.04.30.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Travel%20Demand%20&%20Behavioural%20Modeling/Notes/Allegati/Allegati/Schermata%202025-03-06%20alle%2012.04.30.png)


#### Multi-stage sampling

In **multi-stage sampling** we apply a combination of [[#Stratified sampling]] and [[#Cluster sampling]].

First, we select some strata at random, then, from the selected strata, we select [[#Unit|units]] at random.

![Schermata 2025-03-06 alle 12.21.50.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/2%C2%B0%20Semestre/Travel%20Demand%20&%20Behavioural%20Modeling/Notes/Allegati/Allegati/Schermata%202025-03-06%20alle%2012.21.50.png)


### Judgment sampling

```ad-Definizione
title: Judgment sampling

**Judgment sampling** involves choosing objects that it is believed will give accurate results.

```


### Quota sampling

```ad-Definizione
title: Quota samples

**Quota samples** are based on selecting objects until you have a certain number (the quota) of each type – Appeals to idea of a “representative” sample, but usually biased – Still widely used (especially for telephone surveys with high non- response levels)

```


- [?] Can you apply quota sampling a posteriori? For example, I end up with 60% of female responders so I exclude, at random, some female responders in order to have balance?

### Convenience samples

**Convenience samples** are obtained by choosing the easiest objects available


## Sampling from a finite population

A [[#Simple random sampling|simple random sample]] from a finite population of size $N$ is a sample selected such that each possible sample of size $n$ has the same probability of being selected.

## Point estimation

In point estimation we use data from a [[#Sample]] to compute a value of a sample statistic that we then use as an estimate of the population statistic.

```ad-Definizione
title: Point estimate

A **point estimate** is as statistic computed from a sample that gives a single value for the population parameter.


```

We have a population of size $N$, from which we select a sample of size $n$.

Let $Y$ be the target variable (numeric) and we are interested maybe in the population mean ($\mu$) or the population variance ($\sigma^{2}$).

Let the sample be the set of obseravtions:
$$
\{ Y_{1}, ..., Y_{n} \}
$$
Then, the sample mean is:
$$
\overline{Y} = \frac{\sum\limits_{i=1}^{n}Y_{i}}{n}
$$
I want, starting from $\overline{Y}$, the **point estimate** for the population mean.

Statistics can prove that the [[Estimator]] ($E[...]$) for the population mean, is the sample mean itself:
$$
E[\overline{Y}] = \mu 
$$
```ad-attention

This is not true for every statistic. If for example I define a statistic like:
$
\theta = \frac{\min{(Y_{1},..., Y_{n})}+ \max{(Y_{1},..., Y_{n})}}{2}
$
Then I don't know what its estimator is:
$
E[\theta ] = ???
$
```






- [?] What is a sample distribution?