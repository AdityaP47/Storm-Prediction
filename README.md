# Storm-Prediction

Software Requirements Specification (SRS)
  Purpose and Scope
	This document is made to provide a detailed description of the prerequisite needed in order to use Storm Prediction Model . It will explain the features, classes, interfaces, constraints, reaction to external stimuli and working of the system.
This document is intended to be easy to understand for every tester or developer who without any prior knowledge of the software can still understand all its underlying working.     	This document is also intended for researchers/stakeholders interested in an understanding of adoption of Machine Learning for Prediction of Weather parameters over “Numerical-Based weather Prediction”.
   Definitions
	Below mentioned are few definitions/terminologies which are kept in mind while building this project.
EF-Scale:Enhanced Fujita Scale is our main parameter for dependent variable. The scale is used to analyse/measure the severity of Storm based on the damage they produce. EF-scale uses numbers ranging from 0 to 5 to know the impact of    storms/tornadoes. Wind speed is positively correlated with EF-scale points and thus EF - scale can be classified by wind  parameter as shown below:


Om: This column in the dataset tells us about the count number of tornadoes. These numbers are assigned based on the time of occurrence of each event.
Yr,Mo,Dy,Tz: Year, Month , Date and Time Zone in the dataset columns respectively. 
F : F-scale values, which turn into EF-scale values post January of 2007 , since previously EF-scale wasn’t introduced.
Inj: Injuries (which is “summing up of state totals”)
Fat: Fatalities (which is “summing up of state totals”)
Loss : Estimated Property Loss scaled to numerical values 0 to 9 based on the below table:
 
Tornado damage beared (in USD)
Unknown
<50$
50-500$
500-5000$
5000-50000$
50000-500000$
500000-5000000$
5000000-50000000$
50000000-500000000$

0
1
2
3
4
5
6
7
8


 
Slat & Slon : Starting Latitude and Longitude of Storm.
Elat & Elon : Ending Latitude and Longitude of Storm.
Len : Length of storm in miles.
Wid: Width of storm in yards.
 
 
The code creates a correlation matrix to assess the factors which affect the dependent variable in the dataset (EF-scale score) and then 
5 ML algorithms namely : Logistic Regression, Decisioon Tree, Random Forest , KNN and SVM are used to model the output. The performance of each algo is evaluated and compared

 
