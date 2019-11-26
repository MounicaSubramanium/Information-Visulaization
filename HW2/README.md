## DS500_Homework2
Solutions for Homework 2 for DS 5500 - Information Visualization: Applications in Data Science

### Problem 1
- Akhil Nair
- Mounica Subramani
- Mrinal Soni
- SuRui Yang

### Problem 2

The visualization I chose to compare and review for Problem 2 of HW1 is by Bishishta. 

https://github.com/bishishta/Information-Visualization/tree/master/DS5500_HW1

The visualization is about the distribution of GPA per Capita across countries over time. Her plot was a clear static line plot. There were 20 sub plots for 193 countries where 10 countries were represented in each plot. We have "Year" in X-axis and GDP per Capita in the y axis.

There was also another plot representing GDP/Capita across continents over time which is again a simple static 2D lne plot. 

The plot that I have mode for problem 2 was similar to the one that represents GDP/capita across continents over time from Bishishta's plots. However the clear representation of distribution of GDP/capita across countries was interesting and it is easy to interpret. It also does justice to the actual question. Her plot was able to explain what was asked in the problem and interpretations were clear. Interpretations based on the second plot for both of us were kind of similar 

### Problem 3

The visualization I chose to compare and review for Problem 3 of HW1 is by Monica Mishra.

https://colab.research.google.com/drive/1v8EY74vQxPubjXHywpDUYo7a3FMj-GuB#scrollTo=KXfw0fJqJwab

The visualization is about the relationship between income (GDP / capita), life expectancy, and child mortality over time. We both have split the problem into three parts and plotted each feature relationship and used interactive dynamic plots for the problem. She also used the Google colab effectively for all her visualization plots. both of us have represented 4 continents instead of six. 

The visualizations are easily interpretable. Her interpretations were also clear and did answer the questions in problem 3. 

### Problem 4
We are investigating the relationship between GDP per capita and life expectancy over time. Here, we are considering GDP per capita income as Y and Life expectancy as X. in the below plot we kind of see a positive linear relation ship between X and Y and hence decide to build a linear regression model. The positive linear relationship denotes that as the income increase the life expectancy is also increasing. It can be due to better healthy lifestyle, health plans etc.

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img1.png)

Below figure is trying to fit the predicted linear model line on the data throws an impression that model is not so good with poor accuracy. It can be assumed that the data needs to processed more and then we can try building a model for processed data.
The hypothesis used for the model is  Y ~ X + error (i.e.,) GDP_income ~ Life_Exp + err

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img2.png)

Below figure denotes plot of log value of Life expectancy against log GDP per capita income. This doesn't seem quite useful still we are trying to build a model and see how it fits the line on the data.

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img3.png)

The hypothesis is log(Y) ~ log(X) + error (i.e.,) log(GDP_income) ~ log(Life_exp) + err

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img4.png)

Taking mean of the vlaues is improving the data and its feature relationship to a btter extent. Now, this shows a very positive correlation between Life expectancy and GDP per capita income. This set of data can now be used to build the model.

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img5.png)

The hypothesis is mean(Y) ~ mean(log(X)) + err0r (i.e.,) mean(log(GDP_income)) ~ mean(Life_exp) + err

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img6.png)

The presence of clear positive linear relationship between variables is the main reason to opt for linear regression model.

The challenge was to capture a clean relationship between the features. This model can further be tested by including year(time) as another variable to the hypothesis. We have already analysed the relationship between GDP per capita income and life expectancy for each country and continent which makes more sense and provides greater insights country wise rather than a global information.

If autocorrelation of time series is not handled then it would greatly affect the evaluation metrics of the model and giving out wrong coefficient there by misleading the modelling part itself.

### Problem 5

There is a linear relationship between the response variable and the predictor variables which is why we come with the assumptions to fit a linear regression model. There is a strong negative linear correlation between child mortality rate and gdp per capita income. This can be interpretted as, as the income increases there is better healthy lifestyle which reduces child death rate drastically.

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img7.png)

The hypothesis used is mean(Y) ~ mean(X) + error (i.e.,) mean(GDP_income) ~ mean(Child_mort) + err
The model's life is not a best fit to the data hence the hypothesis can be tweeked a little bit to get the model into perfect shape. After taking mean of the data the correlation coefficient improved largely from -0.5 to -0.9 indicating a strong negative linear relationship.

![](https://github.ccs.neu.edu/mounicasubramani/DS5500_Homeworks/blob/master/HW2/Images/img8.png)

The hypothesis used is log(mean(Y)) ~ mean(X) + error (i.e.,) log(mean(GDP_income)) ~ mean(Child_mort) + err

The accuarcy of the model is 98%.

If autocorrelation of time series is not handled then it would greatly affect the evaluation metrics of the model and giving out wrong coefficient there by misleading the modelling part itself.
