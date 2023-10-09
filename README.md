[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11725981&assignment_repo_type=AssignmentRepo)
# The impact of price on reviews for the 100 most expensive and 100 least expensive private rooms of Airbnb

_"To what extent do the 100 most expensive private rooms get more yearly reviews than the 100 cheapest private rooms compared across 5 Western-European capitals (Amsterdam, Berlin, Brussels, London, Paris) on an annual time base? An analysis of multiple cities and time-frames."_

# Project Motivation 
<img src="https://github.com/course-dprep/team-project-data-prep-team-10/assets/143409405/4b4503f3-bea1-4c63-bd7a-988ae92ec1b5?raw=true" alt="Alternatieve tekst" height="130">

Leaving a review and sharing it with the world wide web is only a matter of seconds. The rise of the internet gave room for leaving reviews about anything, anywhere, very easily. Whereas a few decades ago people relied more on word of mouth and written reviews in papers, nowadays we have access to millions of reviews in just a few mouse clicks.

We are curious whether the amount of reviews is higher for the top 100 most expensive private room compared to the bottom top 100 least expensive private rooms. The reasoning is that people who book expensive rooms want to know that their rooms is from high quality and thus higher value lots of reviews. However, people who stay at budget Airbnb's are maybe more critical of booking a place with more reviews. In order to gain a deeper understanding of the amount of reviews of private rooms on the most expensive and least expensive Airbnb's we will conduct a research. Due to the unavailability of extensive data, we will conduct the research using a limited datset, which may not meet our desired data volume. Hence, we will compare 2 years worth of reviews and analyze the findings to answer the research question described above.

# Method and Results
## Method
The importance of considering the pricing on reviews is to gain a better understanding of the relationship between the yearly reviews and pricing of housing. The research method chosen is an analysis of the ouput of the available data in 5 citites in 2022 and 2023 on Airbnb. The 2 categories are coded as the 100 cheapest private rooms (0) and the 100 most expensive private rooms (1).

In this research, we have selected 5 capitals from western European countries. The reason for this is that those cities are most likely to have similar circumstances and thus will provide a solid background to research the question. The five selected cities are:
* Amsterdam
* Berlin
* Brussels
* London
* Paris

Two data points are used. The top 100 most expensive and the 100 cheapest private rooms will be further examined in the research.

## Variable types
The following variable types are used in our research:
```

| Variable     | Description                       | Data class     
| -------------| ----------------------------------| ------------
| City         | City of observation               | character  
| Price        | Listing price of room per night   | numeric  
| Date         | June 2023 & December 2022         | Date  
| Room type    | private room                      | character  

```

##  Type of analysis
To adress our research question, we first decided to take a close look at the output of our code. After which we will create barcharts the chosen variables. The dependent variable in this research is the amount of reviews that a private rooms has received and the independent variable is the price of the private room. We decided on adding 5 different cities to see if the location might also have an affect. By adding a control variable, the aim is to get a better understanding of the effect.

## Results
After running our code, we figured out that the results were very inconsistent and thus hard to generalize conclusion about the data.

By visualizing the data into barcharts we got the following insights. In Amsterdam the cheap private rooms consitently had more yearly reviews than the expensive rooms. On the other hand, Berlin, London and Paris showed opposite results as the expensive private rooms consistently got more reviews. For the city of Brussels the results were surprisingly different, as in 2022 the cheap private rooms got slightly more reviews whereas in 2023 the expensive private rooms got slightly more reviews. Therefore, it at first glance seems that expensive private rooms are getting more reviews. However, this finding is only consistent for 3 out of the 5 cities and thus further research needs to be conducted to gain a deeper understanding of the effects of the amount of yearly reviews and the pricing of private rooms.

# Repository Overview
```
 
  ├── data
  ├── gen
   ├── analysis
   ├── data-preparation
   └── paper
└── src
   ├── analysis
   ├── data-preparation
      ├── Download_Data_Relative
      ├── Makefile
      ├── Output_Data_Relative
      ├── Transform_Data_Relative
   └── paper
├── .gitignore
├── README.md
├── makefile
```
# Dependencies
For a smooth execution of the project, follow the installation guides on [Tilburg Science Hub](https://tilburgsciencehub.com)
* R
    * [Setting up R and R studio](https://tilburgsciencehub.com/building-blocks/configure-your-computer/statistics-and-computation/r/)
* Make
    * [Setting up Make](https://tilburgsciencehub.com/building-blocks/configure-your-computer/automation-and-workflows/make/)
 * Github
     * [Setting up Git and Github](https://tilburgsciencehub.com/building-blocks/configure-your-computer/statistics-and-computation/git/)

# Example of workflow research reproduction

# How to run the project
* Running the code by using Make
  1. Fork this repository
  2. Open your terminal and run the following code
   ``` git clone https://github.com/{your username}/team-project-data-prep-team-10.git ````
  4. Make will run all the code and will generate a jpng file with the barchart results of the analysis
  5. Ensure that the pipeline is cleaned of all unnecessary data files, running the following code in the terminal:
     ``` make clean```

* Run the project using the repository context
  1. ./src/data-preparation -> Download_Data_Relative.R
  2. ../src/data-preparation -> Transform_Data_Relative.R
  3. ../src/data-preparation -> Output_Data_Relative.R

# Resources
* [Insideairbnb](http://insideairbnb.com/get-the-data/)

# Authors 
This repository is developed by team 10 for the course Skills: Data Preperation & Workflow Management (Fall) under supervision of Hannes Datta. This course belongs to the marketing program Marketing Analytics of Tilburg School of Economics and Management. The team consists of the following members:
* Max Baaten 
* Denise Baltus 
* Rick Massuger 
* Sjuul Visschers 
