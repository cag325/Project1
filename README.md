# Analysis of Hospital Presence and Education in Connection to Covid Deaths (Using PA and OH County data) 
Project 1 for ChE 2410

Obtaining knowledge of disease and illness spread is an important concern of modern science. We often seek to identify the potential factors that promote or inhibit the spread of illness amongst populations. Moreover, we often attempt to identify characteristics amongst the population itself that affect the spread of illness. In wake of the Covid-19 pandemic significant research has been devoted to understanding the contributing factors to its spread in the context of population influences. Furthermore, current research seeks to rationalize any differences in Covid-19 fatalities amongst various counties. 

The purpose of this research was to analyze if education or hospital presence contributed to differences in Covid outcomes for Pennsylvania (PA) and Ohio (OH) counties in the year following the start of the pandemic (i.e., using 2020 data). The motivation behind this research was not revolutionary but rather sought to understand if any fundamental characteristics of a population contribute to differences in Covid outcomes. One would likely assume that counties with a higher population of college educated individuals would possess a greater level of basic knowledge of disease spread mitigation practices and health practices in general or be capable of informing themselves of such through scientific literature. Such knowledge would lead one to suspect their outcomes following Covid-19 infection would be better than those who are less educated. Similarly, one would also likely assume that counties with a greater hospital presence would enable more patients to receive medical care following Covid-19 infection and subsequently contribute to a better outcome on average than counties with less or no hospital presence. These assumptions therefore needed to be evaluated on a scientifically rigorous standard to test their validity. 

To evaluate the validity of such assumptions, college education data and hospital data were collected for all counties in PA and OH. Categorization of the data was then necessary prior to analysis. In the case of education, we sought to categorize counties as "High Education Populations" and "Low Education Populations" based on the percent of college educated individuals in that county. The criteria of the education grouping were whether 25% or greater of the population had a college education. Thus, counties with a population in which 25% or greater of the population was college educated were assigned to the "High Education Population" while those with less than a 25% college educated population were assigned to the "Low Education Population". 

The hospital data was similarly categorized into two groups for the purpose of analysis. In the case of hospital data categorization, identifying the appropriate parameter to represent "Hospital Presence" was non-trivial. With the county data at hand, the number of hospital beds in total per county was chosen to represent the "Hospital Presence" in a county. This selection of a representative parameter was assessed as the best amongst the consistent data collected. "High Hospital Presence" counties were those in which the total number of hospital beds in that county was greater than or equal to 500 beds while those attributed to the title of "Low Hospital Presence" counties had less than 500 hospital beds. This chosen statistic may be questioned by external reviewers because counties with a greater number of hospital beds are very likely to be counties with a greater population size. Such an argument is valid; however, the analysis below attempts to correct for this discrepancy by using Covid deaths in proportion to population size. Despite this correction it is fair to claim that analysis of different parameters that reflect "Hospital Presence" is needed to truly understand if any connection between Covid-19 outcomes and "Hospital Presence" exists. 
#### Hypothesis: We hypothesize that counties classified as "High Education" will exhibit more favorable outcomes following Covid-19 infection, characterized by lower mortality rates, when compared to counties classified as "Low Education." Similarly, counties categorized as "High Hospital Presence" are expected to demonstrate improved outcomes compared to "Low Hospital Presence" counties. Furthermore, we anticipate a strong interaction between the education classification and hospital presence classification, contributing to the overall Covid-19 outcomes within these counties.

# Results Summary 
Beginning with the analysis of the effects of education on Covid-19 deaths, counties were categorized based on the percent of the population with a college education. "High Education" counties were those with a population makeup of 25% or greater with a college education while those that did not satisfy the criteria were termed "Low Education" counties. A scatter plot of the data with a fit generated using linear regression is seen below.

![image](https://github.com/cag325/Project1/assets/144633699/f43327b0-24f2-4cd8-826c-9052bd249f97)


We observe a small positive slope in our linear fit potentially suggesting that "High Education" counties have surprisingly worse outcomes following Covid-19 infection than "Low Education" counties. However, further investigation into the statistical significance of this relationship demonstrates that this difference is non-existent (calculated p-value of 0.477). This result deviated from prediction given the expectation that education would promote better health practices and subsequently better outcomes following infection. 

![image](https://github.com/cag325/Project1/assets/144633699/8b16c5f1-43eb-4e26-ba8e-b71677c7f94b)

#### Conclusion 1: The education classification of a county does not affect the proportion of Covid-19 fatalities in that county.

The analysis of the effects of hospital presence per county on Covid-19 fatalities was conducted next. As previously stated "High Hospital Presence" counties were those in which at least 500 general hospital beds in total were present in hospitals in the county. Therefore, "Low Hospital Presence" counties were those in which less than 500 general hospital beds existed in the county. A scatter plot of the data with a fit generated using linear regression is seen below.

![image](https://github.com/cag325/Project1/assets/144633699/a07d350d-09a6-4347-ad05-2276df9b14dd)


Like the previous analysis a small positive slope was generated from our linear regression analysis potentially suggestive that "High Hospital Presence" counties have worse Covid-19 outcomes (i.e., more death). However, again the statistical significance of this relationship proved to be futile (calculated p-value of 0.991). Again, this served to contradict our hypothesis that a greater number of hospital beds would lead to better overall health outcomes as compared to counties with less hospital beds. 

![image](https://github.com/cag325/Project1/assets/144633699/4e17013c-872a-4c52-b353-125fad439ec5)

#### Conclusion 2: The magnitude of hospital presence of a county does not affect the proportion of Covid-19 fatalities in that county.

Our final analysis was conducted to investigate any potential interaction effects between our two established factors: education classification and hospital presence. For those unfamiliar with the concept of interaction effects it is the phenomena in which the presence of two variables at the same instance induces an elevated effect on the measured variable. In our case, an example of a strong interaction effect would be observed if Covid fatalities drastically increased in county populations that fit the "Low Education" classification and "Low Hospital Presence" classification. The interaction analysis is depicted below where the "x3" term represents the interaction parameter. Based on the calculated p-value of 0.501 we observe no profound interaction relationship between the two factors.

![image](https://github.com/cag325/Project1/assets/144633699/680ef73b-2a3a-482a-93d7-e0039f1cf34d)

#### Conclusion 3: 
There does not exist a significant extent of interaction between the factors of education classification and hospital presence that promotes an elevated difference in Covid-19 outcomes when comparing counties.

#### Conclusion: As scientists we are obligated to report the works in which the results conflict with our hypotheses and not only the results that support them. We began this research hypothesizing that education differences between counties would contribute to a significant difference in Covid-19 mortalities amongst the counties. However, our statistical analysis refuted our claim and suggested that education differences do not yield a substantial difference in Covid-19 deaths. Similarly, we hypothesized that differences in the extent of hospital presences would yield differences in Covid-19 mortalities when comparing counties. Yet again, our initial prediction was incorrect as the statistical analysis does not support any such relationship. Our final analysis investigating potential interaction effects amongst the two factors once more contradicted our hypothesis by demonstrating an insignificant interaction effect on Covid deaths. In totality, the results refuted the entirety of our hypothesis but provided insight into the minimal effects of these factors on disease outcomes. We do acknowledge that future work exists to study the influence of these factors under the application of alternative definitions, meaning that maybe an important relationship does exist but only in the context of different definitions for the educational classifications and hospital presences.

#### Supplementary Information (SI)
Plots of raw data prior to reconstruction for analysis 

![image](https://github.com/cag325/Project1/assets/144633699/a0fd99f4-e3f2-46d5-86de-2fcb15a31e02)

![image](https://github.com/cag325/Project1/assets/144633699/05580be1-20e2-4fc1-ae88-d0750e648fe1)

![image](https://github.com/cag325/Project1/assets/144633699/8b445384-16c4-4538-bdcb-2bdb549a9e5d)

![image](https://github.com/cag325/Project1/assets/144633699/b3ff6544-6ac6-4387-8ca4-40f2a82c737b)




  



