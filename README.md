# CLUSTERING CUSTOMERS AND ANALYZING THE INFLUENCE OF FACTORS ON SATISFACTION LEVELS IN INVISTICO AIRLINES.

This repository contains the submission for the final project of Programming For Data Analysis class at UEH University.

## Team Members
- DS001 - K46 - Đoàn Vũ Minh Thanh
- DS001 - K46 - Nguyễn Đình Đại Nhơn
- DS001 - K46 - Đoàn Anh Thư
- DS001 - K46 - Huỳnh Thị Cẩm Nhung
- DS001 - K46 - Lê Thị Tuyết Nhung
- DS001 - K46 - Huỳnh Trần Anh Thy

## Overview

1. **Data**:The dataset includes detailed information about flight data as well as customer ratings (on a scale of 1-5) regarding various criteria related to the flights they have taken. The dataset consists of 129,880 observations, with 23 variables.
2. **Data preprocessing**: Handling missing values, discretizing data columns, handling likert scale.
3. **EDA**:

    The chart shows the number of customers in each age group for each rating level.
![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/7e1a77cd-405a-4888-967b-1549459098c9)


    The chart illustrates the relationship between the 'Seat comfort' criterion for each type of 'Flight Distance' and the overall satisfaction for the flight.
![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/145bec7e-608e-4acb-a2b6-a663b0d659dc)


    The chart represents the number of ratings within the range [0-5] that customers rated as "satisfied."
![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/d15cdb57-f2b7-429e-a637-db33969b8d4c)



    The chart shows the satisfaction of passengers for different types of travel experiences.
![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/ea6c305b-4638-4e5c-b8d4-4b897b75f29b)

4. **Classification**: Using K-Nearest Neighbours, Decision Tree, Support Vector Machine, Naive Bayes
   - Result 2 best model : 
       + Decision Tree:

     
           ![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/f4e34686-9f77-4b86-ae21-6fb8a8ff6108)
         
       +  Support Vector Machine:
    
         
           ![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/75786275-9197-4dcb-bc03-c44170c78889)



6. **Clustering** : Using K-Means
 As observed, for the number of clusters k = 5, the Silhouette score has the highest value, surpassing the threshold of 0.5, specifically at 0.602. This indicates that this cluster might closely align with the underlying patterns in the data. Therefore, the decision is made to proceed with clustering using 5 clusters.
![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/0041ae9c-b48d-47a4-b185-27c77d5db3c7)

![image](https://github.com/Gizdabet/LTPTDL/assets/135012930/9129d2f6-abea-4512-9474-e5bb56520560)

The characteristics of the clusters are as follows:
- 0 :
  + There are two groups of passengers, those traveling in Business class and those in Eco Plus class. The majority of passengers are in the Business class (> 25,000) compared to Eco Plus (~ 4,000).

  + The ratings for the 'Gate location' criterion fall within the range of 2-3 points.

  + These passengers belong to the premium segment of the airline, and with the low ratings for the 'Gate location' criterion, it seems they are quite dissatisfied with the gate location. Possible reasons could be the distant locations of the gates, difficulty in finding them, or other factors. Further data is needed to understand the exact reasons behind this dissatisfaction.

- 1 :
  + There are two groups of passengers, those traveling in Business class and those in Eco Plus class. The majority of passengers are in the Business class (> 24,000) compared to Eco Plus (1,363).

  + The ratings for the 'Gate location' criterion fall within the range of 4-5 points.

  + These passengers belong to the premium segment of the airline, and with the high ratings for the 'Gate location' criterion, it shows their satisfaction with the convenient gate locations for boarding the aircraft.

- 2 :
  + There are two groups of passengers, those traveling in Eco Plus class and those in Eco class. The majority of passengers are in the Eco class (> 30,000) compared to Eco Plus (2,200).

  + The ratings for the 'Gate location' criterion fall within the range of 3-4 points.

  + These passengers belong to the economy segment of the airline, and with the moderate ratings for the 'Gate location' criterion, it shows that this group of customers does not have high demands regarding the gate location. They are satisfied with the average gate positions for boarding the aircraft.
- 3 :
  + This group consists of passengers traveling in Eco class.

  + The ratings for the 'Gate location' criterion fall within the range of 1-2 points.

  + These passengers belong to the economy segment of the airline, and with the low ratings for the 'Gate location' criterion, it shows that they are dissatisfied with the gate locations for boarding the aircraft. This indicates that they might not find the gate positions convenient or suitable.
- 4 :
  + There are two groups of passengers, those traveling in Business class and those in Eco Plus class. The majority of passengers are in the Business class (> 11,000) compared to Eco Plus (1,621).

  + The rating for the 'Gate location' criterion is 1 point.

  + These passengers belong to the premium segment of the airline, and with the lowest rating for the 'Gate location' criterion, it indicates that they are currently dissatisfied with the gate locations for boarding the aircraft. Possible reasons could be the distant locations of the gates, difficulty in finding them, or other factors. Further data is needed to understand the exact reasons behind this dissatisfaction.
