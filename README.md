# Analysis of Hospital Presence and Education in Connection Covid Deaths (In PA and OH Counties) 
Project 1 for ChE 2410

Obtaining knowledge of disease and illness spread is an important concern of modern science. We often seek to identify the potential factors that promote or inhibit the spread of illness amongst populations. Moreover, we often attempt to identify characteristics amongst the population itself that affect the spread of illness. In wake of the Covid-19 pandemic significant research has been devoted to understanding the contributing factors to its spread in the context of population influences. Futhermore, current research seeks to rationalize any differences in Covid-19 fatalities amongst various counties. 

The purpose of this research was to analyze if education or hospital presence contributed to differences in Covid outcomes between  Pennsylvania (PA) and Ohio (OH) counties.The motivation behind this research is not revolutionary but rather seeks to understand if any fundamental characteristics of a population contribute to differences in Covid outcomes. One would likely assume that counties with a higher population of college educated individuals would possess a greater level of basic knowledge of disease spread mitigation practices and health practices in general or be capable of informing themselves through scientific literature. Such knowledge would lead one to suspect their outcomes following Covid-19 infection would be better than those who are less educated. Similarly, one would also likely assume that counties with a greater hospital presence would enable more patients to recieve medical care following Covid-19 infection and subsequently contribute to a better outcome than counties with less or no hospital presence. These assumptions therefore need to be evaluated on scientifically rigours standard to test their validity. 

To evaluate the validity of such assumptions college education data and hospital data were collected for all counties in PA and OH. Categorization of the data was then necessary prior to analysis. In the case of education, we sought to categorize counties as "Higher Education Population" and "Lower Education Population" based on the percent of college educated individuals in that county. The criteria of the education grouping was whether or not 25% or greater of the population had a college education. Thus, counties with a population in which 25% or greater of the population is college educated was assigned to the "Higher Education Population" while those with less than a 25% college educated population were assigned to the "Lower Education Population". 

The hospital data was similarly categorized in two groups for the purpose of analysis. In the case of hospital data categorization, identifying the appropiate data to represent "Hospital Presence" is non-trivial. With the county data at hand, the number of hospital beds in total per county was chosen to represent the "Hospital Presence" in a county. "High Hospital Presence" counties were those in which the total number of hospital beds in that county was greater than or equal 500 beds while those attributed the title "Low Hospital Presence" counties had less than 500 hospital beds. This chosen statistic may be questioned by external reviewers because counties with a greater number of hospital beds are very likely to be counties with a greater population size. Such an arguement is valid, however, the analysis below attempts to correct for this discrepancy by using Covid deaths in proportion to population size. Despite this correction it is fair to claim that analysis of different parameters that reflect "Hospital Presence" is needed to truly understand if any connection between Covid-19 outcomes and "Hospital Presence" exist. 
#### Hypothesis: That counties of the "Higher Education" classification as well as counties with a "High Hospital Presence" will have better outcomes follwoing Covid-19 infection (i.e., less death) than counties of the "Lower Education" classification and/or "Low Hospital Presence". Additionally, we suspect there to exist a strong interaction between the education classification and hospital presence being that almost all medical professions require a college education.  

# Results Summary 
Beginning with the analysis of the efffects of education on Covid-19 deaths, counties were categorized based on the percent of the population with a college education. "Higher Education" counties were those with a population makeup of 25% or greater with a college education while those that did not satisfy the criteria were termed "Lower Education" counties. A scatter plot of the data with a fit generated using linear regression is seen below.

![image](https://github.com/cag325/Project1/assets/144633699/6297e015-8b7a-483a-a41f-c8c1ae10ad36)

We observe a slightly positive slope in our linear fit potentially suggesting that "Higher Education" counties have worse outcomes following Covid-19 infection than "Lower Education" counties. However, further investigation into the statistical significance of this relationships demonstrates that this difference is really non-existant (calculated p-value of 0.477).

![image](https://github.com/cag325/Project1/assets/144633699/8b16c5f1-43eb-4e26-ba8e-b71677c7f94b)

#### Conclusion 1: The education classification of a county does not affect the proportion of Covid-19 fatalities in that county.

The analysis of the effects of hospital presence per county on Covid-19 fatalities. As previously stated "High Hospital Presence" counties were those in which at least 500 general hospital beds in total were present in the collection of hospitals in the county. Therefor, "Low Hospital Presence" counties were those in which less than 500 general hospital beds existed in the county. A scatter plot of the data with a fit generated using linear regression is seen below.

![image](https://github.com/cag325/Project1/assets/144633699/7a260a6c-c477-4c2c-ab3d-4a6afa1d91bf)

Similar to the previous analysis a slightly positive slope was generated from our linear regression analysis potentially suggestive that "High Hospital Presence" counties have worse Covid-19 outcomes (i.e., more death). However, again the statistical significance of this relationship proved to be futile (calculated p-value of 0.991).

![image](https://github.com/cag325/Project1/assets/144633699/4e17013c-872a-4c52-b353-125fad439ec5)

#### Conclusion 2: The hostpial presence prevalence of a county does not affect the proportion of Covid-19 fatalities in that county.



