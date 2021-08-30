# Capstone-Project-2_Classification-Insurance_Cross_Selling
Change this description HERE


# AlmaBetter EDA Capstone Project 1 Worldbank EdStats

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


### Data Visualization Methods Used
* Time Series Lne graphs
* Pie Chart Plots
* World Map Chloropeth Plots
* Heat maps
* Size-Heat maps

### Python Libraries used
For Graphing : 
* Matplotib
* Seaborn 
* heatmapz
* Dash-Plotly

Datawrangling : 
* Numpy
* Pandas
* Json
* pprint - Pretty Printer 


## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](https://drive.google.com/drive/folders/1zbIOG82jvDXavYuGazysc0j89GRzWz__?usp=sharing) within GDrive
    


## The Structure of the main IPYNB notebook :

* Initial Library imports 
* Exploring File : EdStatsCountries.csv
  * Reading data and exploring which columns are necessary
  * Geographic and Economic Special- Macro- country codes
  * Grouping countries by Geographic and Economic groups ( Size-Heatmap )

* Exploring File : EdStatsSeriies.csv
  * Reading data and exploring which columns are necessary
  * Understanding the indicator series : 
    * What about what topics are these indicators 
    * How many indicators per topic
  * Utility Function : get_indicator_details() : 
    * This function return the details of an indicator as dictionary , 
    * useful for retrieving definition and name during plots

* Exploring File : EdStatsData.csv
  * Reading data and exploring which columns are necessary
  * Removing Columns for Future Years , 
  * Removing Rows which are Empty
  * Understanding the availability of Data for each Year
    * Both before and after cleaning with Bar Plots

* Utility Function : Comparative analysis
  * get_pivot_similiarity():
  * this function takes two countries as an input and calculates how similar they are based on all available indicators , from 1970 to 2015

* Utility Function for full Report Generation 
  * generate_report():
  * This function takes a list of countries and one indicator as Input 
  * It generates multiple different plot so that we can instantly get an idea of what is going on for that indicator
  * the plots generated include :
    * Line graph of values of that indicator for all countries in the list passed , over time from 1970 to 2015
    * Pie Chart Plot for those counties for one particular year passed as input 
    * Similarity Heat Map - for visualizing which countries are more similar to each other , for each country pair inside the list of countries
      * this function is based on the Utility function for Comparative analysis called : get_pivot_similiarity
      * the output generated is similar to that of a correlation plot .

* World Map Visualization : 
  * Dash Plotly library used for making a world map chloropleth plot 
  * Indicators such as Population , Population Growth and GDP(PPP) are visualized in this section

* Case Study : BRICS Countries : 
  * BRICS Countries : Brazil Russia India China South-Africa
  * Study of Population Growth 
  * Study of How the expenditure on education impacts the education outcomes
  * Study of correlation between Educated, GDP and  Mortality 

* Case Study : Comparison between Education in India and America
  * Study of Primary and Primary and Tertiary Education Outcomes and Expenditures
  * Comparative study of Drop-Out rate 




## Contributing Team Members:

|Name     |  Email   | 
|---------|-----------------|
|Saifuddin Raja(https://github.com/saif-raja) |     saifuddin.raja24@gmail.com    |
|Varun Nayyar(https://github.com/saif-raja) |     nayyar.varun84@gmail.com    |
|Fahad Mehfooz(https://github.com/saif-raja) |    fahad.mehfoooz@gmail.com    |
|Shubham Bareja(https://github.com/saif-raja) |     sbshubham23@gmail.com    |
|Pooja Rana(https://github.com/saif-raja) |     rana.pooja800@gmail.com    |
|Anirudh Upadhyay(https://github.com/saif-raja) |     anirudh31ajm@gmail.com    |




*Instructions: Click on the raw button in the upper right hand corner of this box.  Copy and paste the template into the README.md document on your github.  Fill in the titles, information and links where prompted! Feel free to stray a bit to suit your project but try to stick to the format as closely as possible for consistency across DSWG projects.*

# Project Name
This project is a part of the [Data Science Working Group](http://datascience.codeforsanfrancisco.org) at [Code for San Francisco](http://www.codeforsanfrancisco.org).  Other DSWG projects can be found at the [main GitHub repo](https://github.com/sfbrigade/data-science-wg).

#### -- Project Status: [Active, On-Hold, Completed]

## Project Intro/Objective
The purpose of this project is ________. (Describe the main goals of the project and potential civic impact. Limit to a short paragraph, 3-6 Sentences)

### Partner
* [Name of Partner organization/Government department etc..]
* Website for partner
* Partner contact: [Name of Contact], [slack handle of contact if any]
* If you do not have a partner leave this section out

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* etc.

### Technologies
* R 
* Python
* D3
* PostGres, MySql
* Pandas, jupyter
* HTML
* JavaScript
* etc. 

## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- etc. (be as specific as possible)

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](link)
* [Notebook/Markdown/Slide DeckTitle](link)
* [Blog Post](link)


## Contributing DSWG Members

**Team Leads (Contacts) : [Full Name](https://github.com/[github handle])(@slackHandle)**

#### Other Members:

|Name     |  Slack Handle   | 
|---------|-----------------|
|[Full Name](https://github.com/[github handle])| @johnDoe        |
|[Full Name](https://github.com/[github handle]) |     @janeDoe    |

## Contact
* If you haven't joined the SF Brigade Slack, [you can do that here](http://c4sf.me/slack).  
* Our slack channel is `#datasci-projectname`
* Feel free to contact team leads with any questions or if you are interested in contributing!





[![Build Status](https://dev.azure.com/mhew/data-science-template/_apis/build/status/data-science-template?branchName=master)](https://dev.azure.com/mhew/data-science-template/_build/latest?definitionId=15&branchName=master)

# Data Science Template
This is a starter template for data science projects in Equinor, although it may also be useful for others. It contains many of the essential artifacts that you will need and presents a number of best practices including code setup, samples, MLOps using Azure, a standard document to guide and gather information relating to the data science process and more. 

As it is impossible to create a single template that will meet every projects needs, this example should be considered
a starting point and changed based upon the working and evolution of your project.

Before working with the contents of this template or Data Science projects in general it is recommended to familiarise yourself with the Equinor [Data Science Technical Standards](https://wiki.statoil.no/wiki/index.php/Statoil_Data_Science_Technical_Standards) (Currently Equinor internal only)

## Getting Started With This Template
This template is provided as a [Cookiecutter template](http://cookiecutter.readthedocs.org/en/latest/installation.html) so you
can quickly create an instance customised for your project. An assumption is that you have a working python installation.

To get running, first install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher):

    pip install -U cookiecutter

### Create project
Then generate a new project for your own use based upon the template, answering the questions to customise the generated 
project:

    cookiecutter https://github.com/equinor/data-science-template.git
    
The values you are prompted for are:

| Value                   | Description |
| :---                    | --- |
| project_name            | A name for your project. Used mostly within documentation | 
| project_description     | A description to include in the README.md | 
| repo_name               | The name of the github repository where the project will be held |
| conda_name              | The name of the conda environment to use |
| package_name            | A name for the generated python package. | 
| mlops_name              | Default name for Azure ML. | 
| mlops_compute_name      | Default Azure ML compute cluster name to use. | 
| author                  | The main author of the solution. Included in the setup.py file | 
| open_source_license     | What type of open source license the project will be released under | 
| devops_organisation     | An Azure DevOps organisation. Leave blank if you aren't using Azure DevOps | 

If you are uncertain about what to enter for any value then just accept the defaults. You can always change the generated project later.

*Getting problems? You can always download this repository using the download button above and reference the local copy e.g. cookiecutter c:\Downloads\data-science-template, however ideally fix any git proxy or other issues that are causing problems.*

You are now ready to get started, however you should first create a new github repository for your new project and add your 
project using the following commands (substitute myproject with the name of your project and REMOTE-REPOSITORY-URL 
with the remote repository url).

    cd myproject
    git init
    git add .
    git commit -m "Initial commit"
    git remote add origin REMOTE-REPOSITORY-URL
    git remote -v
    git push origin master

### Continuous Integration
Continuous Integration (CI) increase quality by building, running tests and performing other validation whenever 
code is committed. The template contains a build pipeline for Azure DevOps, however requires a couple of manual
steps to setup:

* Log in to http://dev.azure.com and browse to, or create an organisation & project. The project name should be the same as your github repository name.
* Under *Pipelines -> Builds select* *New Pipeline*
* Select github and then your repository. Login / grant any permissions as prompted
* In the review pane click *run*

You are now setup for CI and automated test / building. You should verify the badge link in this README corresponds 
with your DevOps project, and as a further step might setup any release pipelines for automated deployment.

At this stage the build pipeline doesn't include MLOps steps, although these can be added based uon your needs.

### Finally

* Update the project readme file with additional project specific details including setup, configuration and usage. 
* The docs\process_documentation.md file should be completed phase by phase, and each phase result shall be submitted for review and approval before the project moves on to the next phase. This is to assist with the gathering of essential information required to deliver a correct and robust solution. The git respoitory shall be added to the script that populates the [knowledge repository](https://git.statoil.no/DataScience/projects) to ease future knowledge sharing.

## Generated Project Contents
Depending upon the selected options when creating the project, the generated structure will look similar to the below:

```
├── .gitignore               <- Files that should be ignored by git. Add seperate .gitignore files in sub folders if 
│                               needed
├── conda_env.yml            <- Conda environment definition for ensuring consistent setup across environments
├── LICENSE
├── README.md                <- The top-level README for developers using this project.
├── requirements.txt         <- The requirements file for reproducing the analysis environment, e.g.
│                               generated with `pip freeze > requirements.txt`. Might not be needed if using conda.
├── setup.py                 <- Metadata about your project for easy distribution.
│
├── data
│   ├── interim_[desc]       <- Interim files - give these folders whatever name makes sense.
│   ├── processed            <- The final, canonical data sets for modeling.
│   ├── raw                  <- The original, immutable data dump.
│   ├── temp                 <- Temporary files.
│   └── training             <- Files relating to the training process
│
├── docs                     <- Documentation
│   ├── data_science_code_of_conduct.md  <- Code of conduct.
│   ├── process_documentation.md         <- Standard template for documenting process and decisions.
│   └── writeup              <- Sphinx project for project writeup including auto generated API.
│      ├── conf.py           <- Sphinx configurtation file.
│      ├── index.rst         <- Start page.
│      ├── make.bat          <- For generating documentation (Windows)
│      └── Makefikle         <- For generating documentation (make)
│
├── examples                 <- Add folders as needed e.g. examples, eda, use case
│
├── extras                   <- Miscellaneous extras.
│   └── add_explorer_context_shortcuts.reg    <- Adds additional Windows Explorer context menus for starting jupyter.
│
├── notebooks                <- Notebooks for analysis and testing
│   ├── eda                  <- Notebooks for EDA
│   │   └── example.ipynb    <- Example python notebook
│   ├── features             <- Notebooks for generating and analysing features (1 per feature)
│   ├── modelling            <- Notebooks for modelling
│   └── preprocessing        <- Notebooks for Preprocessing 
│
├── scripts                  <- Standalone scripts
│   ├── deploy               <- MLOps scripts for deployment (WIP)
│   │   └── score.py         <- Scoring script
│   ├── train                <- MLOps scripts for training
│   │   ├── submit-train.py  <- Script for submitting a training run to Azure ML Service
│   │   ├── submit-train-local.py <- Script for local training using Azure ML
│   │   └── train.py         <- Example training script using the iris dataset
│   ├── example.py           <- Example sctipt
│   └── MLOps.ipynb          <- End to end MLOps example (To be refactored into the above)
│
├── src                      <- Code for use in this project.
│   └── examplepackage       <- Example python package - place shared code in such a package
│       ├── __init__.py      <- Python package initialisation
│       ├── examplemodule.py <- Example module with functions and naming / commenting best practices
│       ├── features.py      <- Feature engineering functionality
│       ├── io.py            <- IO functionality
│       └── pipeline.py      <- Pipeline functionality
│
└── tests                    <- Test cases (named after module)
    ├── test_notebook.py     <- Example testing that Jupyter notebooks run without errors
    ├── examplepackage       <- examplepackage tests
        ├── examplemodule    <- examplemodule tests (1 file per method tested)
        ├── features         <- features tests
        ├── io               <- io tests
        └── pipeline         <- pipeline tests
```

## Contributing to This Template
Contributions to this template are greatly appreciated and encouraged.

To contribute an update simply:
* Submit an issue describing your proposed change to the repo in question.
* The repo owner will respond to your issue promptly.
* Fork the desired repo, develop and test your code changes.
* Check that your code follows the PEP8 guidelines (line lengths up to 120 are ok) and other general conventions within this document.
* Ensure that your code adheres to the existing style. Refer to the
   [Google Cloud Platform Samples Style Guide](
   https://github.com/GoogleCloudPlatform/Template/wiki/style.html) for the
   recommended coding standards for this organization.
* Ensure that as far as possible there are unit tests covering the functionality of any new code.
* Check that all existing unit tests still pass.
* Edit this document and the template README.md if needed to describe new files or other important information.
* Submit a pull request.


### Template development environment
To develop this template further you might want to setup a virtual environment

#### Setup using
```
cd data-science-template
python -m venv dst-env
```

#### Activate environment
Max / Linux
```
source dst-env/bin/activate
```

Windows
```
dst-env\Scripts\activate
```

#### Install Dependencies
```
pip install -r requirements.txt
```

    
#### Testing
To run the template tests, install pytest using pip or conda and then from the repository root run
 
    pytest tests

#### Linting
To verify that your code adheres to python standards run linting as shown below:

    flake8 --max-line-length=120 *.py hooks/ tests/

## Important Links
* https://wiki.statoil.no/wiki/index.php/Statoil_Data_Science_Technical_Standards - Data Science Technical Standards (Equinor Internal)
* https://dataplatformwiki.azurewebsites.net/doku.php - Data Platform wiki (Equinor internal)
* https://github.com/Statoil/data-science-shared - Shared Data Science Code Repository (Equinor internal)

## References
* https://github.com/Statoil/data-science-template/ - The master template for this project
* http://docs.python-guide.org/en/latest/writing/structure/
* https://github.com/Azure/Microsoft-TDSP
* https://drivendata.github.io/cookiecutter-data-science/
* https://github.com/audreyr/cookiecutter-pypackage

[//]: #
   [anaconda]: <https://www.continuum.io/downloads>

