**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       | 34  |
|-----------------|---|
| Student Names:  |  Jonas Wong |
|                 |  Ryan Huynh |
|                 |   |
|                 |   |

# Introduction

# Assessment Using Reliability Growth Testing 
## Model Comparison Results
The top two models selected to fit the failure data the most was the Geomtric Model and the S Distribution Model. Visually, they fit closer to the shape of failure data in an MVF graph as well as in an intensity graph. They also seem to visually be equal, as the line graph of each model for this failure data cover the same points. However, by looking at the calculated AIC and BIC, the geometric model (GM) has a lower value then the S Distribution Model (S). This means that the geometric model is a better model than the S Distribution Model.

**MVF Graph**

![](./media/mod_comp_mvf.PNG) 

**Intensity Graph**

![](./media/mod_comp_intens.PNG)

**AIC and BIC**

![](./media/mod_comp_calc.PNG)

## Range Analysis
As for what range of data is good for analysis, in reliability growth testing, there are only two reasons to ignore failure data:
* The SUT has changed, and the failure data to be ignored is from a previous version
* The failure data is too old.

Given that the failure data provides no information on the version of the SUT these failures occured on, we can only presume they occured on the same version; So we cannot ignore data based on old changes. However, there are 92 failures total in the data; A general rule for ignoring old data is that recent failure data must contain at least 40-50 failures for proper analysis and is only applicable to systems that have had less than 20% of their program changed. Therefore, for this SUT, we can remove old data up until we have 50 failures left. In this case (referring to the MVF graph), **we can analyse the failure data from interval 13 and beyond.**

## How Decision Making is Affected Given a Target Failure Rate
A Failure Rate refers to the number of failures over time. A target failure rate affects decision making by affecting how much testing the developers (and subsequently, how many failures to fix) they would need to do. The lower the target failure rate, the more testing they would to do. Likewise, the higher the target failure rate, the less testing they would need to do.

As a consequence, a target failure can affect decision making by also affecting how resources are spent on other processes of the software development process, such as requirements elictation/analysis and implementation.

## Advantages and Disadvantages of Reliability Growth Analysis.
A major advantage of reliability growth analysis is that it gives the developers insight into how the reliability of their software is changing: Is the reliability growing or shrinking? When will the reliability reach the target reliabilty? When is testing of the SUT sufficient? With this insight, developers can make better decisions as they develop and maintain their software.

A disadvantage is that reliability growth analysis analysis is dependent on having a lot of failure data (typically at least 40-50 failures) in order for it to be accurate.  It is also dependent on the idea that the system in which the failures were found changes relatively little or not at all (except those changes resulting from failure correction). As such, it can be hard to have inaccurate failure data due to things like unreported failures or major changes to the program. When this inaccurate failure data is used in reliability growth analysis, the insight it provides may be meaningless, or worse, guide the decision making of the developers in the wrong direction.

# Assessment Using Reliability Demonstration Chart 

# 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed
We split up into two pairs where each pair would work primarily on either part one or part two. Though the teams were split, we also made sure to always check up with the other team to make sure that we understood all parts of the lab and that we could help out anytime any issues arise. We did this by making sure that we would meet up every few days to discuss what was done and if any additional help was needed and though both teams were working on different parts, we tried to collaborate whenever we could. 


# Difficulties encountered, challenges overcome, and lessons learned
For creating the RDC, figuring out what values to change to get the required results was confusing. We learned how to use excel better, especially with graphs and learned how MTTF would effect the whether the system would be within the reject, continue, or accept ranges.

# Comments/feedback on the lab itself
There weren't as many instructions and helpful tips for this lab so it was harder to understand how to use some of the tools given. As for the actual lab itself, because of the sparse amount of instructions, we had many difficulties figuring out what we were supposed to do and how to do it. For example, for the RDC portion of the lab, there was a lot of data all over the place and it was extrememly confusing finding out what values would need to be changed/what data to pay attention to in the first place. More details on what to focus on and how to proceed with the lab would have been extremely helpful.  
