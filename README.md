# Ebonya-Washington-s-AER-Regression-model
An article by Ebonya Washington in the American Economic Review argues that having a daughter (as opposed to a son) might a!ect how politicians vote on women’s issues. In particular, she argues that having a daughter causes Congressional representatives to vote more liberally on women’s issues. We will use Washington’s data

## QUESTIONS AND ANSWERS TO THE PROBLEM
a). Examine whether legislators of different parties have the same number of children. Do the results surprise you? Why or why not?

### Answer.
The results show that Republican legislators have significantly more children on average, 2.73 compared to Democratic legislators at 2.22. This half-child difference is statistically significant 
t = –3.26, p = 0.001.
This is not especially surprising, as it may reflect general underlying demographic or cultural differences between the parties, for example, Republicans are often more likely to come from regions or backgrounds with higher fertility rates and stronger traditional family values, while Democrats may come from more urban and less family-oriented contexts.

b). What is the relationship between the number of female children and the AAUW score? Do you think this relationship estimates the causal effect of having a female child?

### Answer:
The relationship between the number of female children and the AAUW score is estimated to be negative (-2.78), though not statistically significant (p = 0.12). That is, representatives in this sample with more daughters do not, on average, vote more liberally on women's issues.
However, this relationship is not necessarily causal. Legislators do not randomly get daughters or sons. Family composition might be correlated with other factors, such as religion or region or social values, that are also related to voting behavior. Thus, this simple regression likely captures correlation, not causation.

c). What is the relationship between the number of female children and the AAUW score when controlling for the total number of children? Do you think this relationship accurately estimates the causal effect of having a female child? If you believe a causal claim is possible, discuss what assumptions you have to make. If not, explain why.

### Answer:
Controlling for the total family size, the coefficient on the number of daughters becomes positive (+5.78) and statistically significant (p = 0.025), indicating that given the same family size, legislators with more daughters tend to have higher AAUW scores, hence voting more liberally on women’s issues.
But this relationship likely still reflects correlation rather than causation. To interpret it as causal, we would have to assume that the gender composition of children is randomly assigned and uncorrelated with other unobserved characteristics (like political ideology, religious beliefs, or regional background) that also affect voting behavior.
Of course, these assumptions are unlikely to hold precisely, so while the sign and significance of the coefficient are consistent with Ebonya Washington's argument, we cannot definitively claim a causal effect from this regression alone.

d). How does this change the results? Why? Is it a good idea to add this control?

### Answer:
Adding party fixed effects changes the model substantially, given the large ideological differences between Democrats and Republicans. The coefficient on the number of daughters is still positive and significant, at +3.14 (p = 0.01), but the overall explanatory power of the model rises sharply (R² = 0.79).
This indicates that most of the variation in AAUW scores is explained by party affiliation, rather than family composition. Having more daughters does, however, predict slightly more liberal voting on women’s issues within parties.
Adding party fixed effects is a good idea because it controls for systematic ideological differences between parties and isolates the within-party variation-that is, whether Republican or Democratic legislators with more daughters behave differently from their fellow party members.
Yet, we should still be very careful with the interpretation of causality: it may still reflect unobserved confounding, where regional culture, education, or personal values drive family outcomes and voting patterns.

e). Regress the AAUW score on the number of female children, controlling for the total number of children for Republicans, Democrats, and the full sample. Plot the coefficients and 95% confidence intervals. Interpret your results.

### Answer: 
The plot shows that, in the full sample, having more daughters is associated with higher AAUW scores-that is, more liberal voting on women's issues. However, once the analysis is separated by party, the effect of daughters becomes small and statistically insignificant within both Democrats and Republicans. This suggests that the positive association in the full sample is driven largely by differences across parties, rather than within them. The Democrats are already very liberal while Republicans' voting behavior remains largely conservative even if they have more daughters. The overall pattern is thus consistent with the hypothesis that legislators with daughters tend to vote more liberally, but the evidence of a causal within-party effect is weak.
