1. The   problem :

    Predicting the Value of a Used Vehicle.

2. The Client

    a. Individual Buyers : Whoever interested in buying a new car wonders about the actual value of the specific car with the one which was asked by the seller. So it is important for all to come to a better understanding of the values of the cars.
    
    b. Dealers : Most dealers would like to learn the value of that individual car, and determine its value later on.
    
    c. Individual Sellers : Most private sellers would need the value of their car since the value is not constant, it changes considering the depreciation, the repairs etc.
    
    d. Websites or Applications created to help private parties or dealers sell their vehicles.
    
    e. .....

3. Data :

    a. I would like to use the data from Kaggle Competitions. The data seems not raw. However, I have also seen an approach to the cleaning process. I will try to come up with new approaches to this.
    
    b. This data includes the data points/observations from 2016. I will search for methods to scrape data for 2017.
    
    
4. My   approach   to   solve  this   problem:

    a. This seems to be a supervised problem.
    
    b. Regression, cause the dependent feature needs to be continous. However, I will combine cross-validation, GridSearch, Random Selection and etc.
    
    c. My dependent feature would be the value of the used cars.
    
    d. My independent features would be the 'name' of the car, seller type, horse power of the car, mileage, any damage or repair, gearbox (automatic or manuel), age of the car...

    e. I am thinking of dividing the data I have with 'train_test_split' feature of scikit learn. If I end up getting the data for 2017, then I would use the data from 2016 as my training data.

5. What are   your   deliverables?   Typically,   this   would   include   code,   along   with   a   paper.

    I will complete this project on Jupiter Notebook. First I will examine data, then wrangle the data and apply ML algorithms. Hopefully I will have learned the basic concepts of data science (Wrangling, Story Telling (EDA) and ML)
    
    a. Data Collection
    b. Data Wrangling
    c. EDA (Exploratory Data Analysis)
    d. Modeling
    e. Presentation

Update :

1. Used Car Value :

Over 370000 used cars [scraped with Scrapy from Ebay-Kleinanzeigen]. The content of the data is in German.

Data Features:
•	dateCrawled : when this ad was first crawled, all field-values are taken from this date
•	name : "name" of the car
•	seller : private or dealer
•	offerType
•	price : the price on the ad to sell the car
•	abtest
•	vehicleType
•	yearOfRegistration : at which year the car was first registered
•	gearbox
•	powerPS : power of the car in PS
•	model
•	kilometer : how many kilometers the car has driven
•	monthOfRegistration : at which month the car was first registered
•	fuelType
•	brand
•	notRepairedDamage : if the car has a damage which is not repaired yet
•	dateCreated : the date for which the ad at ebay was created
•	nrOfPictures : number of pictures in the ad (unfortunately this field contains everywhere a 0 and is thus useless (bug in crawler!) )
•	postalCode 
•	lastSeenOnline : when the crawler saw this ad last online

Problem : Come up with an algorithm which results in a best prediction of the value of a used car.

Approach : Linear Regression (Thinking of applying a combination of algorithms)


2. Condition Based Maintenance of Naval Propulsion Plants Data Set

No of Observations :11934

No of Attributes : 16

Data Set Information:

The experiments have been carried out by means of a numerical simulator of a naval vessel (Frigate) characterized by a Gas Turbine (GT) propulsion plant. The different blocks forming the complete simulator (Propeller, Hull, GT, Gear Box and Controller) have been developed and fine tuned over the year on several similar real propulsion plants. In view of these observations the available data are in agreement with a possible real vessel. 
In this release of the simulator it is also possible to take into account the performance decay over time of the GT components such as GT compressor and turbines. 
The propulsion system behaviour has been described with this parameters: 
- Ship speed (linear function of the lever position lp). 
- Compressor degradation coefficient kMc. 
- Turbine degradation coefficient kMt. 
so that each possible degradation state can be described by a combination of this triple (lp,kMt,kMc). 
The range of decay of compressor and turbine has been sampled with an uniform grid of precision 0.001 so to have a good granularity of representation. 
In particular for the compressor decay state discretization the kMc coefficient has been investigated in the domain [1; 0.95], and the turbine coefficient in the domain [1; 0.975]. 
Ship speed has been investigated sampling the range of feasible speed from 3 knots to 27 knots with a granularity of representation equal to tree knots. 
A series of measures (16 features) which indirectly represents of the state of the system subject to performance decay has been acquired and stored in the dataset over the parameter's space. 







3. Boston Housing

Description

The Boston housing market is highly competitive, and we want to be the best real estate agent in the area. To compete with our peers, we decide to use a few basic machine learning concepts to assist us and a client with finding the best selling price for their home. Fortunately, we have come across the Boston Housing dataset which contains aggregated data on various features for houses in Greater Boston communities. Our task is to build an optimal model based on a statistical analysis with the tools available. This model will then be used to estimate the best selling price for your clients' homes.

Data

The modified Boston housing dataset consists of 490 data points, with each datapoint having 3 features. This dataset is a modified version of the Boston Housing dataset found on the UCI Machine Learning Repository.

Features

RM: average number of rooms per dwelling LSTAT: percentage of population considered lower status PTRATIO: pupil-student ratio by town Target Variable 4. MEDV: median value of owner-occupied homes

Problems :

We would like to build a model using linear regression algorithm to be able to make accurate corrections for the median value of homes using features of the Boston Housing Data Set.

4. Student Intervention

A local school district has a goal to reach a 95% graduation rate by the end of the decade by identifying students who need 
intervention before they drop out of school. As a software engineer contacted by the school district, our task is to model 
the factors that predict how likely a student is to pass their high school final exam, by constructing an intervention system 
that leverages supervised learning techniques. The board of supervisors has asked that you find the most effective model that
uses the least amount of computation costs to save on the budget. We will need to analyze the dataset on students' performance
and develop a model that will predict the likelihood that a given student will pass, quantifying whether an intervention is 
necessary.

Data

The dataset used in this project is included as student-data.csv. This dataset has the following attributes:

Features:
school : student's school (binary: "GP" or "MS")
sex : student's sex (binary: "F" - female or "M" - male)
age : student's age (numeric: from 15 to 22)
address : student's home address type (binary: "U" - urban or "R" - rural)
famsize : family size (binary: "LE3" - less or equal to 3 or "GT3" - greater than 3)
Pstatus : parent's cohabitation status (binary: "T" - living together or "A" - apart)
Medu : mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education or 4 - higher education)
Fedu : father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education or 4 - higher education)
Mjob : mother's job (nominal: "teacher", "health" care related, civil "services" (e.g. administrative or police), "at_home" or "other")
Fjob : father's job (nominal: "teacher", "health" care related, civil "services" (e.g. administrative or police), "at_home" or "other")
reason : reason to choose this school (nominal: close to "home", school "reputation", "course" preference or "other")
guardian : student's guardian (nominal: "mother", "father" or "other")
traveltime : home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
studytime : weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
failures : number of past class failures (numeric: n if 1<=n<3, else 4)
schoolsup : extra educational support (binary: yes or no)
famsup : family educational support (binary: yes or no)
paid : extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
activities : extra-curricular activities (binary: yes or no)
nursery : attended nursery school (binary: yes or no)
higher : wants to take higher education (binary: yes or no)
internet : Internet access at home (binary: yes or no)
romantic : with a romantic relationship (binary: yes or no)
famrel : quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
freetime : free time after school (numeric: from 1 - very low to 5 - very high)
goout : going out with friends (numeric: from 1 - very low to 5 - very high)
Dalc : workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
Walc : weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
health : current health status (numeric: from 1 - very bad to 5 - very good)
absences : number of school absences (numeric: from 0 to 93)
passed : did the student pass the final exam (binary: yes or no)

Problem :

5. Titanic Survival:

I am plannig to use the ‘Titanic practice dataset’ from the Kaggle Competition (Titanic- Machine Learning from Disaster) to predict the types of passengers who are most likely to survive the disaster. In this project proposal, I provide a quick overview of the problem, the dataset.

Description:

The sinking of the RMS Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships. One of the reasons that the shipwreck led to such loss of life was that there were not enough lifeboats for the passengers and crew. Although there was some element of luck involved in surviving the sinking, some groups of people were more likely to survive than others, such as women, children, and the upper-class. In this challenge, we ask you to complete the analysis of what sorts of people were likely to survive. In particular, we ask you to apply the tools of machine learning to predict which passengers survived the tragedy.

Data Set:

A quick review of the training & test datasets shows 12 variables with almost 1300 line items. Each row provides details about an individual passenger such as Age, sex, Passenger Class, family details etc. The independent variable would be the ‘Survived’ field with a binary (1/0) output. A detailed explanation of the data can be found in the kaggle data dictionary.

Features:

pclass : Passenger Class (1 = 1st; 2 = 2nd; 3 = 3rd) name : Name sex : Sex age : Age sibsp : Number of Siblings/Spouses Aboard parch : Number of Parents/Children Aboard ticket : Ticket Number fare : Passenger Fare cabin : Cabin embarked : Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton) Target Variable

survival : Survival (0 = No; 1 = Yes)
