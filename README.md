# Kaggle_Study

# 개요.
[오승은](https://github.com/dhtmddms)
, [강지원](https://github.com/gonekng)
, [장민지](https://github.com/jmj3047)
, [김영재](https://github.com/Kimyoungjae777)
, [엄태현](https://github.com/eomtaehyeon)


    작업 툴 : Kaggle, VS Code, Google Colab, R Studio, Notion, Powerpoint, Google Cloud, MySQL 등
    사용한 코딩 언어 : Python, R, JAVA
    인원 : 5명
    기간 : 2022.03.10. ~ 2022.08.30.
    내용 : 
     - Kaggle을 통해 빅데이터 분석을 공부합니다.
     - Kaggle을 통해 Machine Learning/ Deep Learning의 모델을 공부합니다.
     - Kaggle을 통해 데이터 전처리 과정을 공부하고 EDA의 개념을 정리하고 확립합니다.

<br>

 # 수행한 Kaggle Competition.

[Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic)

 - 공부 기간 : 2022.04.01. ~ 2022.04.12.
 - Description : 
    - Welcome to the year 2912, where your data science skills are needed to solve a cosmic mystery. We've received a transmission from four lightyears away and things aren't looking good.
    - The Spaceship Titanic was an interstellar passenger liner launched a month ago. With almost 13,000 passengers on board, the vessel set out on its maiden voyage transporting emigrants from our solar system to three newly habitable exoplanets orbiting nearby stars.
    - While rounding Alpha Centauri en route to its first destination—the torrid 55 Cancri E—the unwary Spaceship Titanic collided with a spacetime anomaly hidden within a dust cloud. Sadly, it met a similar fate as its namesake from 1000 years before. Though the ship stayed intact, almost half of the passengers were transported to an alternate dimension!

<br>

- Data Description : In this competition your task is to predict whether a passenger was transported to an alternate dimension during the Spaceship Titanic's collision with the spacetime anomaly. To help you make these predictions, you're given a set of personal records recovered from the ship's damaged computer system.

<br>

- Files and Field Descriptions : 
    - train.csv - Personal records for about two-thirds (~8700) of the      passengers, to be used as training data.
        - PassengerId - A unique Id for each passenger. Each Id takes the form gggg_pp where gggg indicates a group the passenger is travelling with and pp is their number within the group. People in a group are often family members, but not always.
        - HomePlanet - The planet the passenger departed from, typically their planet of permanent residence.
        - CryoSleep - Indicates whether the passenger elected to be put into suspended animation for the duration of the voyage. Passengers in cryosleep are confined to their cabins.
        - Cabin - The cabin number where the passenger is staying. Takes the form deck/num/side, where side can be either P for Port or S for Starboard.
        - Destination - The planet the passenger will be debarking to.
        - Age - The age of the passenger.
        - VIP - Whether the passenger has paid for special VIP service during the voyage.
        - RoomService, FoodCourt, ShoppingMall, Spa, VRDeck - Amount the passenger has billed at each of the Spaceship Titanic's many luxury amenities.
        - Name - The first and last names of the passenger.
        - Transported - Whether the passenger was transported to another dimension. This is the target, the column you are trying to predict.
    - test.csv - Personal records for the remaining one-third (~4300) of the passengers, to be used as test data. Your task is to predict the value of Transported for the passengers in this set.
    - sample_submission.csv - A submission file in the correct format.
        - PassengerId - Id for each passenger in the test set.
        - Transported - The target. For each passenger, predict either True or False.
    

[Tabular Playground Series - Apr 2022](https://www.kaggle.com/competitions/tabular-playground-series-apr-2022)

- 공부 기간 : 2022.04.01. ~ 2022.05.01
- Description : You've been provided with thousands of sixty-second sequences of biological sensor data recorded from several hundred participants who could have been in either of two possible activity states. Can you determine what state a participant was in from the sensor data?

<br>

- Data Description : In this competition, you'll classify 60-second sequences of sensor data, indicating whether a subject was in either of two activity states for the duration of the sequence.

<br>

- Files and Field Descriptions : 
    - train.csv - the training set, comprising ~26,000 60-second recordings of thirteen biological sensors for almost one thousand experimental participants
        * sequence - a unique id for each sequence
        * subject - a unique id for the subject in the experiment
        * step - time step of the recording, in one second intervals
        * sensor_00 - sensor_12 - the value for each of the thirteen sensors at that time step
    - train_labels.csv - the class label for each sequence.
        * sequence - the unique id for each sequence.
        * state - the state associated to each sequence. This is the target which you are trying to predict.
    - test.csv - the test set. For each of the ~12,000 sequences, you should predict a value for that sequence's state.
    - sample_submission.csv - a sample submission file in the correct format.


[American Express - Default Prediction](https://www.kaggle.com/competitions/amex-default-prediction)

- 공부 기간 : 2022.05.22. ~ 2022.08.25.
- Description : 
     - Whether out at a restaurant or buying tickets to a concert, modern life counts on the convenience of a credit card to make daily purchases. It saves us from carrying large amounts of cash and also can advance a full purchase that can be paid over time. How do card issuers know we’ll pay back what we charge? That’s a complex problem with many existing solutions—and even more potential improvements, to be explored in this competition.
     - Credit default prediction is central to managing risk in a consumer lending business. Credit default prediction allows lenders to optimize lending decisions, which leads to a better customer experience and sound business economics. Current models exist to help manage risk. But it's possible to create better models that can outperform those currently in use.
     - American Express is a globally integrated payments company. The largest payment card issuer in the world, they provide customers with access to products, insights, and experiences that enrich lives and build business success.
     - In this competition, you’ll apply your machine learning skills to predict credit default. Specifically, you will leverage an industrial scale data set to build a machine learning model that challenges the current model in production. Training, validation, and testing datasets include time-series behavioral data and anonymized customer profile information. You're free to explore any technique to create the most powerful model, from creating features to using the data in a more organic way within a model.

- Data Description : 
    - The objective of this competition is to predict the probability that a customer does not pay back their credit card balance amount in the future based on their monthly customer profile. The target binary variable is calculated by observing 18 months performance window after the latest credit card statement, and if the customer does not pay due amount in 120 days after their latest statement date it is considered a default event.

    - The dataset contains aggregated profile features for each customer at each statement date. Features are anonymized and normalized, and fall into the following general categories:

        - D_* = Delinquency variables
        - S_* = Spend variables
        - P_* = Payment variables
        - B_* = Balance variables
        - R_* = Risk variables
        - with the following features being categorical:

            ['B_30', 'B_38', 'D_114', 'D_116', 'D_117', 'D_120', 'D_126', 'D_63', 'D_64', 'D_66', 'D_68']

    - our task is to predict, for each customer_ID, the probability of a future payment default (target = 1).

    - Note that the negative class has been subsampled for this dataset at 5%, and thus receives a 20x weighting in the scoring metric.

- Files : 
    - train_data.csv - training data with multiple statement dates per customer_ID
    - train_labels.csv - target label for each customer_ID
    - test_data.csv - corresponding test data; your objective is to predict the target label for each customer_ID
    - sample_submission.csv - a sample submission file in the correct format