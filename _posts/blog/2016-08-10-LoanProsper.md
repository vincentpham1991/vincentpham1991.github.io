---
layout: post
title: "Prosper Exploratory Analysis"
modified:
categories: blog
excerpt:
tags: []
date: 2015-08-10T15:39:55-04:00
---

This is an exploratory analysis of Loan data from [Prosper][prosperweb].Check out the [R MarkDown][prospercode] for the codes.


## Questions of interests

* How does Prosper's borrowers base change over time? If Prosper is successful, we would expect an increase in borrowers base as well as an increase in Loan Amount borrowed. 

* How does the Borrower's APR change? Does APR increase/decrease affect the number of borrower's? 

* How does Prosper's lenders change over time? 

* Is there a correlation between Prosper's score and the Borrower's APR? Like any money lending, it is expected to have a gap between high risk lending versus low risk lending.

* How do the students' loan amount compare against each other? One would suspect that they would be almost similar since they would surely borrow to pay for tuition, which is a fixed rate accross grade level. But community college student should also borrow less since their tuition is less. 

* How does Prosper's score correspond to the Credit Score? Is one score a better predictor than the other?

* What is signal of delinquencies? Can you tell by looking at the scores? Or by the Occupation? Or by age?

* Why do Doctor's ask for loans? Is it for a new car? Or maybe it's for medical needs?

* Does Reccomendation effects the size of the loan received or the number of investors?

__The first five questions will be analyzed in this report.__

## Time-series: Average loan amount and number of borrowers

<figure>
	<img src="{{ site.url }}/images/timeseries1.png" alt="image">
	<figcaption></figcaption>
</figure>

Prosper started out with an average of $3700 across 13 borrowers. But it began to grow for 2 years, and the affect of the 2009 financial is noticable. In fact, there was 6 month of inactivity around the beginning of 2009. Loans were continued at a lower level then originally, but the average loan amount increased over time. The amount of loans given though though only remained below 2000 before 2013. 2013 saw a rapid increase in in loans given amounts topping 5000. You can not infer what caused this result, but a hypothesis is that a resurgence of investor's confidence and perhaps lower interests rates increased allowed more loans to be allotted. Regardless, these numbers are positive for Prosper since number of Borrowers and Loan Size have increased dramatically. 

## Time-series: Average Borrower's APR and number of borrowers

<figure>
	<img src="{{ site.url }}/images/timeseries2.png" alt="image">
	<figcaption></figcaption>
</figure>

The data above showed the the first average borrower's APR was a little below 10%. increased to around 20% shortly. This can be seen as Prosper trying to attract customers to its new business then adjusting to the market rate once it sets up a reputation. My best guess, although it can't be confirmed through this graph, is that the Borrower's APR is driven mainly by the market and by other competitors since the APR pretty much picked up where it left off when it stopped activities in 2009. Although it is likely that a lower interest rate attracted more borrowers, there could be other factors at play as well since the 2008 and 2014 period had about the same average APR but a lower borrower base.  

## Time-series: Average number of investor's lending and number of investors

<figure>
	<img src="{{ site.url }}/images/timeseries3.png" alt="image">
	<figcaption></figcaption>
</figure>

What is interesting about this graph is that it showing that it takes time to gain investor's confidence and have more loans invested. The data of the loan given is an aggregate of the investor data across all loans, so it is difficult to tell the amount of repeated investors. For example, alouth the amount of laon given migh be 5000, it might only be by a few people investing in several loans (diversfying their portfolia). Regardless, the average loans invested over the years have been consistent: a very small microloans of about $100 per investor per loan. There has been a huge surge in 2013 though in the amount of loans given and the amount of average amount invested. Lower Borrower's APR doesn't make sense since that would mean a smaller share for the lender, but the simple explanation of supply and demand is the best answers. A huge amount of people who needs to take out huge loan while the interest rate is low and a large pool of investors is a possible explanation for this huge increase. 

## Correlation between Prosper Scores and Borrower's APR

<figure>
	<img src="{{ site.url }}/images/correlation1.png" alt="image">
	<img src="{{ site.url }}/images/correlation2.png" alt="image">
	<figcaption></figcaption>
</figure>

The worst score that a Borrower can be assigned by Prosper is 1, and the best is 10. You can consequence of this fact by seeing the dispersion between the worst score and best score in the first graph. What is interesting is that not until 2013, does Prosper seem to give much incentive to the those who revieved an average score of 5 over those who recieved the worst scores in terms of APR. The only advantage of recieving a 5 over a 1 is that a borrower is more likely to get approved for the loan given by the fact that there are some missing APR for worst score. In 2013 (for the most part) those who recieved a score of 5 recieved an average APR equally between the worst scores and the best scores. This rebalance in APR can potentially attract more average Borrowers and can explain for the increase in number of borrowers in 2013 (as can be seen by the graph on page 3). The bottom graph shows the same idea for the different length of loan. In addition it shows an advantage of recieving the best score. Borrowers who are seeking a short term loan recieve a lower APR rate on average.  

## Student Data

<figure>
	<img src="{{ site.url }}/images/student_data1.png" alt="image">
	<figcaption></figcaption>
</figure>

From the box plot above, it can be seen that the median loan borrowed by students is about the same (around $2500). The variance is also almost similar with college seniors, graduate students, and technical students having more spread in the IQR. This can be explained by the fact that older students are more independent and recieve less fundings from their parents, so they need to seek another means of paying for their education. The higher spread in graduate students can be explained by the fact the master's program tend to have a wider variation in tuition cost than undergraduate programs. But is tuition truly the factor driving these range? If so, why are community college student receiving the same amount of loan as the others even though community college are known to be cheaper? To explore what students are using the funds for, examine the barplot on the next page. 

<figure>
	<img src="{{ site.url }}/images/student_data2.png" alt="image">
	<figcaption></figcaption>
</figure>

Mainly, students claims to borrow funds for non-student use. And only in 2007 - 2010 period do students take out loans for student use. This can be a result of family hardship during the financial crisis. Interestingly, community college students have never recieved loans for student use.  


[prospercode]: https://github.com/vincentpham1991/ProsperExploratoryAnalysis/blob/master/prosper_exploratory.RMD

[prosperweb]: https://www.prosper.com/tools/
