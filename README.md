# AlmaBetter EDA Capstone Project 2 - Classification : Insurance Cross-Selling
Change this description HERE




This project is a part of the [AlmaBetter Premium Program](https://www.almabetter.com/) , Banglore/Bengaluru ,Karnataka , India

#### -- Project Status: [Completed]

## Project Summary :
#### About the Dataset :
We are provided with a dataset  named World Bank EdStats that contains 4000 indicators describing education access(primary, vocational and tertiary), progression, literacy, teacher, population etc. 

The World Bank is an international financial institution which provides monetary assistance to governments of low and middle countries for socio-economic development. Each year, the World Bank collects various statistics through international statistical communities and globally coordinated programs to monitor the growth and progress of various economies. 

#### Problem Statement : 
We were provided with 5 datasets and asked to find insights and trends for different groups of countries and come up with a rough estimate as to which countries are alike and which are dissimilar.

#### Approach taken :
The idea of the project is to analyze the data and mark the variation of indicators across the globe, and also group the countries according to their similarities and differences.

#### Insights from exploring the Data :
From the BRICS countries, we can conclude that the populations of India and China showed growth over the years, with India’s growth rate overtaking China’s after the 2000s.
India’s pre-primary and tertiary enrollment percentage is pretty low when compared to other BRICS countries, but increasing from 1995.
The mortality rate has dropped for every country, the highest drop being observed in India, where more focus was laid on education over the years .
Immigration in USA from 1990-2000 increased the population growth rate for that 10-yr time period
The countries having the highest drop-out rate affected the GNI per capita for those countries

#### Challenges faced:
It was very challenging to completely understand the data and to comprehend the relevance of each CSV file 
As the percentage of missing data was huge, it took a lot of effort to decide on the final data to keep for analysis
Filtering out the best indicators from 3700 indicators to keep for analysis
Deciding on the set of countries to work based on economy and geography

#### Future scope of work:
Working out on Top European powers and compare their positions based on different indicators
Considering the amount of indicators in the data, if we dig deep enough, various micro trends can be unearthed, which we were not able to extensively cover during this short duration.
This dataset can also be used to measure compensation of teachers, if we are to advise the education ministry on management of funds.
Learning Assessment Indicators for Mathematics and Science can be used to predict populations that tend to have a knack for technology.


### Python Libraries used
For Graphing : 
* Matplotib
* Seaborn 
* Scikit-learn


## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](https://drive.google.com/drive/folders/1zbIOG82jvDXavYuGazysc0j89GRzWz__?usp=sharing) within GDrive   
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...


## The Structure of the main IPYNB notebook :

* Initial Library imports 

* Exploring File : main_data.csv
  * Reading data and exploring which columns are necessary
  * Removing Rows which are Empty
  * Understanding the availability of Data for each Year
  * Both before and after cleaning with Bar Plots


* Utility Function : Comparative analysis
  * get_pivot_similiarity():
  * this function takes two countries as an input and calculates how similar they are based on all available indicators , from 1970 to 2015

* Utility Function for full Report Generation 
  * generate_report():
  * This function takes a list of countries and one indicator as Input 

* Case Study : BRICS Countries : 
  * Hypothesis description
  * hypothesis testing
  * hypothesis conclusion




## Contributing Team Members:

|Name     |  Email   | 
|---------|-----------------|
|Saifuddin Raja(https://github.com/saif-raja) |     saifuddin.raja24@gmail.com    |
|Mayank Kumar(https://github.com/saif-raja) |    mayankkumar77952@gmail.com    |
|Shivam Mishra(https://github.com/saif-raja) |     smmishra8298@gmail.com    |
|Hari Om Bharadwaj(https://github.com/saif-raja) |     herrysharma5050@gmail.com    |
|Sarvesh Yadav(https://github.com/saif-raja) |     skyttsearch@gmail.com    |


