# MechaCar Statistical Analysis

### Overview of the statistical analysis:

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, the following were performed:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.

- Run t-tests to determine if the manufacturing lots are statistically different from the mean population.

- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.


### Results:

**Deliverable 1:** Linear Regression to Predict MPG:

Summary: *The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using R, a linear model was designed that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.* 

Below is a short interpretation of the multiple linear regression results:

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

*The data analysis result shows that the vehicle_weight, spoiler_angle, and AWD provided a non-random amount of variance to the mpg values in the dataset with the following p-value results: 0.0776, 0.3069, and 0.1852, respectively. Both vehicle_length and ground_clearance have the most random amount of variance with p-values of 2.60e-12 and 5.21e-08, respectively. Refer to image below.*

2. Is the slope of the linear model considered to be zero? Why or why not?

*The slope of the linear model is not zero since the p-value is 5.35e-11. refer to image below.* 

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

*As you can see from the image provided below, the multiple R-squared is about 71% (0.7149) which is the percent prediction of mpg values are correct. Also, the p-value is below the significance level of 0.05% therefore, this linear model is effective.*

Summary of the p-value and the r-squared value for the linear regression model:

![](./pictures/pic2.png)

**Deliverable 2:** Summary Statistics on Suspension Coils:

Summary: The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using R, the following summary statistics table were created to show:

- The suspension coil’s PSI continuous variable across all manufacturing lots.

Total Summary:

![](./pictures/pic3.png)

- The following PSI metrics for each lot: mean, median, variance, and standard deviation.

Lot Summary:

![](./pictures/pic4.png)

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

*The current manufacturing data is meets the design specification based on total specification which shows a variance of 62.3 psi. However, if the variance is calculated for each lot, only lot 1 (0.98) and lot 2 (7.47) meets the design specification which is well below the PSI limit of 100 pounds. Lot 3 exceeded the limit, with a variance of 170.29*

**Deliverable 3:** T-Tests on Suspension Coils:

Summary: Using R, t-tests were performed to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

t-test results across all manufacturing lots:

![](./pictures/pic5.png)

t-test results for each lot:

Lot 1

![](./pictures/pic6.png)


Lot 2

![](./pictures/pic7.png)


Lot 3

![](./pictures/pic8.png)











**Data Analysis Summary:** *All generated data visualizations are presented side by side on a dashboard as shown on the image below.* 

![](./pictures/pic10.png)

____________________________________________________
 

![](./pictures/pic9.png)

**1. Gender Breakdown:** *Based on the data report, the total number of trips in August is 2,344,224. In  this visualization, the data was analyzed to show the gender breakdown of Citi Bike riders to help our investors understand a little more about the customers in NYC and can be applied in Des Moines. The data shows that majority are male riders (1,530,272) followed by females (588,431). Visualization created from the module.*

![](./pictures/pic8.png)

**2. August Peak Hours:** *This visualization shows the peak hours for bike trips during the month of August. This will help our investors get a ballpark estimate of how many bikes we might need in Des Moines. The data can help determine which parts of the day most of the bikes are needed and can also be useful for determining when to do maintenance on a bike knowing the peak usage hours. Visualization created from the module.*


![](./pictures/pic3.png)

**3. Checkout Times per Users:** *This visualization shows the length of time that bikes are checked out for all riders. Visualization created from the challenge.*


![](./pictures/pic4.png)

**4. Checkout Times by Gender:** *In this visualization,  the data shows the length of time that bikes are checked out for each gender. The highest number of bike used is >2,000 at a tripduration of 5hrs by male riders. The shorter (<1hr) and longer (23hrs) the tripduration, the less number of bikes are used regardless of gender. Visualization created from the challenge.*

![](./pictures/pic5.png)

**5. Trips by Weekday per Hour:** *In this visualization,  the number of bike trips by weekday for each hour of the day is shown in a form of a heatmap. The data shows the peak hours of when bikes are mostly used on weekdays are around 7-9AM and 4-7PM which makes sense because these are the hours where people are reporting (AM) and leaving work (PM). And bikes are mostly used throughout the day on weekends. Visualization created from the challenge.*

![](./pictures/pic6.png)

**6. Trips by Gender (Weekday per Hour):** *In this visualization, the number of bike trips by gender for each hour of each day of the week is shown in a form of a heatmap. Again, the peak hours are the same from the previous slide (Trips by Weekday per Hour) and most of the users are male riders followed by female riders. Visualization created from the challenge.*

![](./pictures/pic7.png)

**7. Number of Trips:** *In this visualization, the number of bike trips by gender for each hour for each day of the week is shown as a heatmap. Most of the users are subscribers and male riders. Visualization created from the challenge.*

**Deliverable 3:** Create a Story and Report for the Final Presentation.

The visualizations shown below are presented on a Tableau Story format. Click the link below to visit the website:

[Link to Tableau Story with Dashboard](https://public.tableau.com/views/NYCCitibikeAnalysisStory/NYCCitibikeAnalysisStory?:language=en&:display_count=y&:origin=viz_share_link)


### Summary:

The bike-sharing program in Des Moines is a solid business proposal especially that we now have the analysis that could help us better design and strategize on how to implement the program in Des Moines. The results shows that most customers are male riders followed by females and some that are not registered (unknown). The bikes are fully utilized before and after work during weekdays and all throughout the day on weekends. 

I would like to see two additional visualizations that will show the following:

1. Identify the most popular bike stations and show how many bikes are used and returned. To give us an idea if we need to supply more inventories in those areas.

2. Show stations that have the highest to lowest bike repairs and utilizations. This will help us move bikes around to temporarily replace damage bikes and help reduce costs. 
