### IDS702 - Modeling And Representation Of Data (Fall 2020)
#### Data Analysis Project 2

This is a data analysis R project I did for the Modeling and Representation of Data course at Duke University. 
The purpose of the analysis is to provide insights to the 2 questions asked below (texts from Professor Akande's course website). 

Question 1 was taken and adapted from Chapter 7 of Ramsey, F.L. and Schafer, D.W. (2013), “The Statistical Sleuth: A Course in Methods of Data Analysis (3rd ed).”

#### OLD FAITHFUL. Old Faithful Geyser in Yellowstone National Park, Wyoming, derives its name and its considerable fame from the regularity (and beauty) of its eruptions. As they do with most geysers in the park, rangers post the predicted times of eruptions on signs nearby, and people gather beforehand to witness the show. R.A. Hutchinson, a park geologist, collected measurements of the eruption durations (in minutes) and the subsequent intervals before the next eruption (also in minutes) over an 8-day period.
1. Fit a regression model for predicting the interval between eruptions from the duration of the previous one, to the data, and interpret your results.
2. Include the 95% confidence interval for the slope, and explain what the interval reveals about the relationship between duration and waiting time.
3. Describe in a few sentences whether or not you think the regression assumptions are plausible based on residual plots (do not include any plots).
4. Fit another regression model for predicting interval from duration and day. Treat day as a categorical/factor variable. Is there a significant difference in mean intervals for any of the days (compared to the first day)? Interpret the effects of controlling for the days (do so only for the days with significant effects, if any).
5. Perform an F-test to compare this model to the previous model excluding day. In context of the question, what can you conclude from the results of the F-test?
6. Using k-fold cross validation (with k=10), compare the average RMSE for this model and the average RMSE for the previous model excluding day. Which model appears to have higher predictive accuracy based on the average RMSE values?
You should be able to leverage your team’s code for doing cross validation.

#### MATERNAL SMOKING AND BIRTH WEIGHTS. 
These days, it is widely understood that mothers who smoke during pregnancy risk exposing their babies to many health problems. This was not common knowledge fifty years ago. One of the first studies that addressed the issue of pregnancy and smoking was the Child Health and Development Studies, a comprehensive study of all babies born between 1960 and 1967 at the Kaiser Foundation Hospital in Oakland, CA. The original reference for the study is Yerushalmy (1964, American Journal of Obstetrics and Gynecology, pp. 505-518). The data and a summary of the study are in Nolan and Speed (2000, Stat Labs, Chapter 10) and can be found at the book’s website.

There were about 15,000 families in the study. We will only analyze a subset of the data, in particular 1236 male single births where the baby lived at least 28 days. The researchers interviewed mothers early in their pregnancy to collect information on socioeconomic and demographic characteristics, including an indicator of whether the mother smoked during pregnancy. The variables in the dataset are described in the code book at the end of this document.
Note that this is an observational study, because mothers decided whether or not to smoke during pregnancy; there was no random assignment to smoke or not to smoke. Thus, we cannot make causal inference statements from the results of a standard regression model.

In 1989, the Surgeon General asserted that mothers who smoke have increased rates of premature delivery (before 270 days) and low birth weights. We will analyze the data to see if there is an association between smoking and birth weight. To simplify analyses, we’ll compare babies whose mothers smoke to babies whose mothers have never smoked. The data file you have access to has only these people, although there were other types of smokers in the original dataset.
Our questions of interest include the following.

1. Do mothers who smoke tend to give birth to babies with lower weights than mothers who do not smoke?
2. What is a likely range for the difference in birth weights for smokers and non-smokers?
3. Is there any evidence that the association between smoking and birth weight differs by mother’s race? If so, characterize those differences.
4. Are there other interesting associations with birth weight that are worth mentioning?
5. Analyze the data and investigate these questions using a linear model. 
