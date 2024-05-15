
# Predicting PM2.5 and PM10 levels in Kuala Lumpur




## 1. Business Understanding

Air Quality Concerns in Malaysia:

Urbanization and Industrialization: Malaysia has undergone significant urbanization and industrialization in recent decades, leading to increased emissions from vehicles, industries, and other sources. This has raised concerns about air pollution and its impact on public health.

Health Implications: Poor air quality, characterized by elevated levels of pollutants such as PM10 (particulate matter with a diameter of 10 micrometers or less) and PM2.5 (particulate matter with a diameter of 2.5 micrometers or less), is associated with various health issues. Respiratory problems, cardiovascular diseases, and other adverse health effects are linked to long-term exposure to high levels of these pollutants.

Government Initiatives: Recognizing the importance of addressing air quality concerns, the Malaysian government has implemented various initiatives and policies. These may include regulations on emissions, vehicle standards, and industrial practices aimed at mitigating the impact of air pollution.

Public Awareness: With the rise of environmental awareness globally, there is an increased focus on individual and collective responsibility for environmental conservation. People are becoming more conscious of the air they breathe, seeking reliable information on air quality to make informed decisions about their well-being.
## 2. Background

Malaysia government has announced its plans to achieve net zero emissions by 2050. Recent efforts toward a more sustainable future has been implemented by government of Malaysia by promoting the use of electrical vehicles and slowly phasing out the use of petroleum and diesel. However, despite such efforts, Malaysia would still experience the haze phenomena October every year. Such high amount of air particulates in the air would be harmful for health, leading to a significant in rise of death due to air pollution. Not to mention that Malaysia spent at least 20% of its GDP to address air pollution.


## 3. Business Objectives

1. To develop a Predictive Air Quality Modelling
Monitor the status and predict the air quality status around Kuala Lumpur, Malaysia which is a hotspot for industrial parks, high traffic flow and movements and high-rise buildings
2. To measure Malaysia's compliance to 12th Malaysian Plan and UNDP Climate Promise
Data obtained could be further utilized for sustainability educational materials or news reporting for the media to further understand the need to address the severity and the need to reduce air pollution in Malaysia
3. To identify various factors contributing to air pollution in Malaysia
EDA and classification models could help to identify which air pollutants are currently highly emiited in Kuala Lumpur and methods to address them

## 4. Problem Statement

Air pollution, particularly the levels of particulate matter PM10 and PM2.5, is a significant public health concern in urban settings, with Kuala Lumpur's rapid development bringing its air quality into sharp focus. The absence of a predictive model that integrates a range of factors affecting PM10 and PM2.5 levels is a notable gap in research, particularly within the context of Kuala Lumpur. Such a model is vital for designing precise interventions and informing both policy and the public to alleviate the detrimental health impacts of air pollution. This research endeavors to create a sophisticated predictive model for PM10 and PM2.5 concentrations, considering variables like weather, traffic, and industrial activity, aiming to bolster air quality management and protect Kuala Lumpur residents' health. Air pollutants not only increase hospital admissions for respiratory issues—even at low levels, they have a cumulative effect on health, as indicated by Sofwan et al. (2021), who underscore the urgency of monitoring and taking timely preventative action against air pollution. Moreover, providing early warnings to residents through monitoring and prediction of pollutant levels is critical for the government to implement timely measures. There are two main approaches for monitoring: physics-based and data-driven, with the former often failing to capture the dynamic nature of air pollution, as per Chae et al. (2021). While current studies, including those by Usmani et al. (2021), frequently utilize computationally intensive convolutional neural networks, this research will concentrate on optimizing machine learning algorithms that may surpass CNNs in performance, reflecting our focal point in this field.

## 5. Business Success Criteria

1. Multivariate Prediction Accuracy
Develop predictive modelling which can successfully predict PM10, PM2.5 based on various factors
Evaluation metrics such as MAE, RMSE, or R-squared for each pollutants

2. Integration with Air Quality Index with predictions
Successfully integrate predictions with AQI for a comprehensive air assessment
The Air Quality Index (AQI) for PM10 is calculated using the following formula:

AQI = (Breakpoint PM10 High - Breakpoint PM10 Low + Low Index PM10) / (Index PM10 High - Index PM 10 Low) * (Concentration PM10 - Breakpoint PM10 Low)

Sources: EPA US

breakpoints_pm10 = [0, 54, 154, 254, 354, 424, 504] #EPA indices_pm10 = [0, 50, 100, 150, 200, 300, 500]

breakpoints_pm25 = [0, 12, 35.4, 55.4, 150.4, 250.4, 350.4] #EPA indices_pm25 = [0, 50, 100, 150, 200, 300, 500]
## 6. Data Mining Goal

Objective 1 Data Mining Goal: To create a predictive model to predict PM2_5 and PM10 with hyperparameter optimization to achieve R^2 = 0.90.
Objective 2:Data Modeling: Create a LSTM model to predict PM2_5 and PM10 for upcoming years
Objective 3:Data Modeling: Integrate prediction results with Air Quality Index
## Authors for Modelling component (All the RNNs, ARIMA)

- [@juinnsheng](https://www.github.com/juinnsheng)

