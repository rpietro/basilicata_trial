# A parallel randomized controlled trial comparing a Situated Cognition online learning program vs. control and its effect on decision making: A reproducible research protocol

Mauro Maldonato  
Silvia Dell'Orco  
Rossella Gagliardi  
Bruno Melo  
Joao Ricardo Vissoci  
Ricardo Pietrobon


## Abstract
<!-- write at the end -->

## Introduction

The concept of situated cognition implies that our thinking is not restricted to our brains. A typical example is that when a person is asked about the total population of Timbuktu in Mali, the answer would be nearly impossible to most of us, unless our memory is assisted by a technology such as [Google searching](https://www.google.com/). Of importance, cognitive enhancement through technologies is but one of many ways in which cognition can be enhanced, with potentially beneficial gains from a learning perspective. Despite a substantial body of literature in the Humanities about the concept of situated cognition(@prinz2009consciousness, @clark2008supersizing), to our knowledge its potential effect on online learning has not been previously tested in randomized trials.

Situated cognition essentially argues that traditional cognitive theories are missing essential components when it affirms that brain processes can be separated from technological and social contexts (Extended cognition), bodily experiences (Embodied cognition), actions (Enacted cognition) and the environment (Embedded cognition). These essentially constitute what has been labeled the four Es constituting situated cognition (@aydede2009cambridge). Although the term situated learning has been previously used, it is usually restricted to learning happening within communities of practice (@lave1991situated), therefore been overly restrictive in comparison with the more contemporary definition of situated cognition.

The objective of this parallel randomized trial is therefore to compare standard training vs. an intervention involving {behavior} in educating college students regarding {course}, the study design, conductance and reporting following a reproducible research approach. We hypothesize that the intervention would result in decision making that is more fully supported by information gathered in a more comprehensive manner through technological and socially means, actions that are more effective and adaptive and also more empathetic and connected to the needs of others. 


## Methods

This trial was designed and reported in accordance with the recommendations provided by the [CONSORT statement](http://www.consort-statement.org/)

### Ethics
This study was approved by the Ethics Committe at the University of Basilicata ([Università degli Studi della Basilicata](http://portale.unibas.it)), informed consent having been waived since this was considered a research with minimal risk within an educational context. All participants were ensured that their participation was absolutely unrelated to their performance in their current disciplines and that they could drop out at any point if they so wanted.

### Trial Design
This is a parallel controlled randomized trial comparing (1) the introduction of a situated cognition approach to learning in the context of professional activities, delivered through an online platform versus (2) a control without any intervention. The trial involved 106 participants <!-- replace by the actual number and describe dropout rate -->, randomized on a 1:1 ratio to the intervention and control arms, with the intervention and respective follow-up lasting a total of four weeks. No changes to the initially methods design were implemented while the trial was in course. <!-- need to check at the end whether this is true -->

### Participants
Our study involved 106 participants. Participants were undergraduate and graduate students at the University of Basilicata, located in the Basilicata region of Southern Italy. Demographic information is provided as a separate dataset in our reproducible research protocol to preserve participant confidentiality and prevent loss of confidentiality. For exach participant we have collected information on gender, age, course, and course year.

### Interventions

The main intervention was constituted by a short course with weekly video lectures and exercises focused on three aspects of situated cognition as applied to their daily personal, academic or professional lives. Specifically, these three aspects constituted Extended Cognition (social and technological components), Embodied Cognition and Enacted Cognition. All educational material is made available within our Reproducible Research repositories, but in short they were constituted by the topics described under Table 1. 

Table 1

| Component | Content |
| --- | --- |
|Extended social cognition| How to appropriately post on popular Web-based discussion groups, using not only Italian but also basic English  |
|Extended technological cognition|How to perform advanced searches on the Web using both general search engines as well as specialized database repositories|
| Embodied cognition|How to use basic principles of emotional influence (@cialdini1993influence) regarding reciprocation, consistency, social proof, liking, authority and scarcity|
| Enacted cognition|How to use Lean processes (@ries2011lean) of short cycles and experiments to put information in practice|

All instructional material was delivered through the original [Open edX platform](http://code.edx.org/). Videos were provided in English with subtitles in Italian. All remaining material was made available in Italian, although both Italian and English versions are provided within our Reproducible Research repositories (see subsequent section on Reproducible Research).

The control group was constituted by the lack of intervention, participants simply logging in at least twice/week to fill out the Situated Cognition Learning Index as further described in the Outcomes section.


<!-- add CONSORT for Non-Pharmacological Treatment Interventions -->

<!-- soft skills, tacit knowledge, rationality, competition, empathy, choice, aesthetics, memory, emotion, happiness - ask mauro for opinion on what could work -->


### Outcomes

Given the absence of standardized scales to measure learning outcomes related to situated cognition, we have devised and concomitantly validated a Situated Cognition Learning Index within our trial. The main outcome measure for our study is a mixed weekly log containing multiple alternative and open questions regarding the three situated cognition components to be evaluated in our study. These components and their respective items are described under Table 2. Participants were asked to fill this log out at least twice/week regarding their daily daily activities. For each item participants were asked to indicate how many times they had performed that activity in that day.

Table 2. Items within the weekly log for the Situated Cognition Learning Index

| Construct | Item |
| --- | ---- |
| Extended social cognition | Today I have posted a question to an online forum |
| Extended social cognition | Today I have asked somebody who is an expert on a topic I needed |
| Extended technological cognition | Today I have searched the Web to answer a question I had |
| Extended technological cognition | Today I have searched Google or some other general engine to answer a question |
| Extended technological cognition | Today I have consulted a specialized database or information repository to answer a question |
| Embodied cognition | Today I have attempted to use some form of reciprocation, social proof or liking strategies in a way that would emotionally persuade my colleagues |
| Embodied cognition | Today I have attempted to use some form of authority, consistency or scarcity strategies that would emotionally persuade my colleagues |
| Enacted cognition | Today I have used a short experiment to put information I gathered in practice in one of my personal, academic or professional projects |
| Enacted cognition | Today I have used what I learned in a short experiment to pursue a second cycle of experiments for one of my personal, academic or professional projects |
| Other strategies | Please write down any comments you might have regarding the activities above |

<!-- add any changes to outcomes happening during the trial  -->

### Sample size

<!-- 
install.packages('pwr')
library(pwr)
pwr.t.test( d = 0.55 , sig.level = 0.05, power = 0.8 , type = c("two.sample")) 
-->

Given the absence of preliminary data, we calculated our sample size based on an assumption of a two-sample t-test for an index representing the combined outcomes, with an effect size of 55%, a significance level and statistical power set at the traditional levels of 0.05 and 80%, respectively. Under these assumptions the estimated required sample size is of 52.9 per group, which we have rounded to 53, ultimately leading to a total sample size of 106 participants in total.


### Randomization

We used a randomization scheduled generated through the R computer language (@rcitation2014), with a blocking strategy of 8 participants to ensure a reasonable distribution between the two arms. Allocation was defined by pairing the random list with a list of participants in alphabetical order by last name. Given the explicit nature of the educational intervention, blinding was only possible at the analysis level, where the analyst (RP) received the dataset with a code that did not explicitly indicate which interventions were allocated to each participant. 


### Statistical methods

All analysis were conducted using the R language (@rcitation2014). Given the small amount of missing values across variables, no imputation was applied to our dataset. Descriptive analysis was conducted using means and standard deviation for continuous variables, with frequencies and percentages being applied to categorical variables. 

We have partially validated the Situated Cognition Learning Index by calculating its Cronbach's alpha reliability coefficient usign the [psych package](http://cran.r-project.org/web/packages/psych/index.html) within the R language.

Inferential tests were used to both verify the efficacy of the randomization in balancing both arms in terms of potential confounders at baseline. Briefly, we used two sample unpaired t-tests calculated with 95% confidence intervals for all continuous variables with a normal distribution, and Chi square tests for categorical variables, also calculated with 95% confidence intervals. Given the longitudinal nature of our outcome measures, we used mixed models to compare individual outcomes between the two arms.


### Reproducible research
In order to follow a reproducible research protocol, we have written our final manuscript using an Rmarkdown, which combines the R language with the [Markdown markup](http://daringfireball.net/projects/markdown/), ultimately allowing us to leave all calculations and data manipulation within the article text. All data sets and respective analytical scripts were provided in CSV (comma separated value) formats in open public repositories including [Figshare](http://figshare.com/) and [Github](https://github.com/). In addition, we have also stored the version of the software used in this analysis and deposited it within our Github and Figshare repositories, ultimately decreasing the probability of reproducibility issues during subsequent attempts to reproduce our analyses. <!-- add paper that recommends this procedure -->

## Results

<!-- add this section in alignment with CENT -->

## Discussion



