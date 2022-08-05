# Project: Investigate a Dataset (Soccer Database)

## Project Workflow

- <a> Introduction </a>
- <a> Data Wrangling</a>
- <a>Exploratory Data Analysis</a>
- <a> Conclusions</a>


<a id='intro'></a>
## Introduction

This database contains a vast amount of soccer data from 2007 to 2015 in a .sqllite file. I used DB Browser to export the needed dataset as a .csv file. There are 8 tables in this database but the scope of my analysis will be limited to two, that is, player and player attributes. With this table we are exploring the questions our scouting team asked us, using the 2016 season.
- How many of the players were left footed?, what is the proportion of left footed players comapred to the total population.<br> 
- Does height have an effect on a players jumping ability?<br> 
- The scouts are intrested in recommending Ronaldo because of his ariel threat but they want to know; Has time has affected his jumping ability?,  also, determine abilities he improved on the most and area(s) he drastically declined as an attacker using the first season(2007) and last season (2015).<br>
- Is there a correlation between weight, height and acceleration?<br>


 Table 1: Player
<br> There are 6 columns in this dataframe.
   - Player api id	(serves as a primary key)
   - Player name	
   - Player fifa api id (serves as a primary key)
   - Birthday: Player's birthday
   - Height: Player's height
   - Weight: Player's weight
   
 Table 2: Player Attributes 
 <br> There are 41 columns in this columns. To mention a few.
   - Player fifa api id (foreign key)
   - Player api id (foreign key)	
   - Date: Year, month and day
   - Overall rating: Player's rating
   - Potential: Player's potential
   - Preferred foot: Player's preferred foot (left or right)
   - Finishing: Player's finishing ratings	
   - Vision: Player's vision ratings	
   - Penalties:	Player's penalty ratings
   - Marking: Player's marking ratings	


## Data cleaning process 
### After discussing the structure of the data and any problems that need to be
###   cleaned, let's perform those cleaning steps in the second part of this section.
>##### 1) Looking at the player dataframe, birthday column will be dropped as it is of no use to this analysis.
>##### 2) In the player attribute dataframe,drop all missing values and duplicates if any.
>##### 3) In the player attribute dataframe, drop all the columns that won't be used in the analysis.
>##### 4) In the player attribute dataframe, date has a wrong datatype and only year is needed after changing the datatype.
>##### 5) In the player attribute dataframe, convert all abilities from float to int as abilities are usually measured in whole numbers.
 
 

<a id='eda'></a>
## Exploratory Data Analysis



> After data wrangling, visuals were used to make our result meaningful and easier to understand. Here, the dataframe statistics and visualization was explored with an aim to address the research questions that was posed in the Introduction section. 

> #### Using this combined table, EDA was used to look at a single variable before exploring the relationships between variables, Bivariate visualization.


## Research Questions 

- How many players were left footed?, what is the proportion of left footed players comapred to the total population ?
- Does height have an effect on a players jumping ability?
- The scouting department is intrested in recommending Ronaldo because of his ariel threat but they want to know if time has affected his jumping ability?, determine this using the first season(2007) and last season (2015)
- Is there a correlation between weight, height and acceleration?


## Limitations
- The units of weight and height were not included in the documentation, infact there was no documentation.
- Due to missen documentation i was limited to some data sets because i couldn't understand some abbreviations in other data sets.
- The dataframe was quite large so i couldn't explore some aspects without my system hanging. This delayed the speed of this report drastically.
- The scope of this data analysis was limited to player and player attributes only.    
    


```python

```
