# Diabetes is an expensive, life-altering disease.
It's effect can be felt around the world but some countries feel the burden of diabetes more significantly than others. In fact low and middle income countries currently hold 75% of all diabetic patients. As the number of diabetic patients continues to increase, this inequity become more significant and overhwleming. As of 2018, there are over 425 million diabetics globally. By 2045, this number is predicted to increase to 635 million! As the world braces for this tremendous increase in diabetes (as well as all the associated complications and comorbidities), some countries will be more significantly affected than others.

This begs the question, how are rates of diabetes changing in countries around the world? What are some common factors among countries seeing the biggest increase? I used data from the [Global Health Data Exchange](https://www.thelancet.com/lancet/visualisations/gbd-compare) to analyze the incidence and effect of diabetes globally, and find answers to these questions.

## Data Analysis
First the Global Health Data Exchange [data set][1] containing the diabetes incidence rate in 2017 for 196 countries was downloaded. Then a cluster analysis was conducted in order to identify groups of nations. This analysis yielded 5 clusters and identified 14 countries facing the highest incidence rates of diabetes. In order of incidence rate, these countries are:  Fiji, Kiribati, American Samoa, Mauritis, Marshall Islands, Micronesia, Malta, Northern Mariana Islands, Bahrain, Tonga, Portugal, United Arab Emirates, Trinidad and Tobago, and Denmark. The analysed data set can be found [here][2]

Then, overall disease burden data for the [American Samoa][3] and the [United States of America][4] was downloaded. This showed both 2017 data and percentage change from 1993-2017. These data sets were analyzed using [JupyterLabs Python notebook][5]. Pivot tables were created to quickly analyze the data and compare the top contributers to overall disease burden in both countries. Type 2 Diabetes was the biggest contributer to disability adjusted life years (DALYs) in the American Samoa but was not even in the top 5 for the United States. 

In order to compare the effect of diabetes in these countries, a dataset detailing [diabetes incidence rates between 1993-2017][6] and another detailing [diabetes deaths between 1993-2017][7] for the American Samoa, the United States and the global averages were downloaded. These were plotted to identify trends over time and can  be seen in the images below.

![Diabetes Incidence Rates][diab_inc]
![Diabetes Deaths per 100,000][diab_death]

## Discussion
Analysis of the initial data question, how are rates of diabetes changing around the world, found that 7 of the 10 nations with the fastest growing rate of diabetes are from the Oceania region. Furthermore, two of these nations are considered territories of the United States, the country that spends the greatest amount of money on healthcare globally. The United States also has a significant rate of diabetes, but is not in this top cluster of nations. This begged the question, how do overall disease burdens in the United States and the American Somoa differ? Why are the outcomes for these nations so different? These are important questions for policy makers, public health officials, and those who care about health equity issues to consider. From the graphs above, it is clear that though a bit higher than the global average, the United States still sees significantly lower rates of both diabetes incidence and deaths than the American Samoa. The American Samoa is seeing an extremely troubling increase in these rates over the years, greater even than the already troubling increases globally. Given the relatively small overall population of the American Samoa, the number of diabetic patients may seem small. However, it is critical that this increase in the rate is taken seriously. When a significant portion of the population is suffering from diabetes, this can increase the impact faced by healthcare systems exponentially due to the care required for comorbidities and complications. Routine surgical procedures become more risky, annual checkups become more important, and money spent on medications increases.

[1]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/GBD%20Diabetes.csv
[2]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/GBD%20Diabetes.xlsx
[3]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/American%20Samoa%20Raw%20Data.csv
[4]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/USA%20Raw%20Data.csv
[5]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/Global%20Burden%20of%20Disease.ipynb
[6]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/Diabetes%20Incidence.csv
[7]: https://github.com/njeeva/burden-of-diabetes/blob/master/data-files/Diabetes%20Deaths.csv
[diab_death]: https://github.com/njeeva/burden-of-diabetes/blob/master/Diabetes%20Deaths%20Over%20Time.png
[diab_inc]: https://github.com/njeeva/burden-of-diabetes/blob/master/Diabetes%20Incidence%20Over%20Time.png
