# Kickstarter-analysis
Performing analysis on kickstarter data to uncover trends
                                                                    # Kickstarter Project

## Overview of Project
Louise wants to fund her play "Fever",which is something she is doing for the first time and she is estimating a budget of 10000$.

### Purpose
The purpose of this analysis is to determine what factors help in making a successful project.Excel historical data will be used to help Louise identify these factors and help her reach
her goal.
 
## Analysis and Challenges
###Analysis
    Data in the excel were wrangled and set in the proper format to do the analysis (dates were changed from Unix time to a date, Parent categry and sub categories were split into two different
columns).

####Theatre outcomes based on launch date
For the theatre outcomes based on launch date, a pivot table was inserted, with the launch date to in the rows, and the outcomes as columns, the data in the pivot table counts
the number of outcomes (successful, failed and canceled). Also a filter with the parent category and year was added to help analyse the different parent categories.

####Outcomes based on Goal
For the outcomes based on goal, the goal ranges were set as requried, then the countifs() was used with three different criteria
1.Outcome
2.Pledged amount
3.Parent category

### Analysis of Outcomes Based on Launch Date
Good news! The analysis of the outcomes based on launch date showed that plays were always more successful than failed all over the dates analysed, also, the rate of cancellation
was mostly low. Plays is a good category to launch a project.
However, some dates have influenced successful projects more than other dates and it is recommended to launch the projects at these dates. 

### Analysis of Outcomes Based on Goals
In case the aim is a relatively smaller project, mostly goals with values less than 19999$ tend to have a more success rate than other goals values. For bigger projects,values between 35000$-45000$
were more successful than much bigger projects requiring bigger goals. Regarding Louise's project.

### Challenges and Difficulties Encountered

There has been several difficulties, for the data set provided in sheet "kickstarter", the date required to be changed from Unix format to date format, the formula to make the date change
is available on the internet, so a search was done to uncover the formula.
Also the category and subcategory needed to be split into two different columns, so the excel feature "text to columns" was used to do that and split them wherever "/" is found. This
feature was mentioned in module 1 and reviewed the module to find the solution.

For the outomes based on goals, the challnges faced were the following:
1-The ranges required some attenctin to be used in the right way when doing the countifs() function.
2-Attention was also requried to base the sheet only on the parent category "Plays" because Louise's project is a play.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Two conclusions can be drawn from outcomes based on Launch date.
1-June has the highest sucssess outcomes to launch the "fever" play project, and december has the least success rate. It is recommended for louise to start her project
in June and avoid starting it in december.
2-Plays tend to have a more success rate than the failure rate and very low cancellations, so it is good for Louise that she is in the right category "Plays".
In Louise's case, it recommended to launch her play in June. It is good for her that she is in the Plays category.

- What can you conclude about the Outcomes based on Goals?
The conclusion that can be drawn is that smaller goals tend to have more success rates than big goals.Also when goals become extremely large, the probability that a project
will fail is much higher (higher than 80%) than the probability of success (lower than 20%). More precisely, projects with goals between 45K$ and 50K$ will 100% fail, so this goal
must be avoided by any means.
Lastly,goals have no infuence on a project being canceled. The rates were always 0% , and there was no canceled projects.
In Louise's case, she is expecting a budget of 10000$ wich is a good budget for her play as projects with less than 19999$ tend to have higher success rates than failure rates.

- What are some limitations of this dataset?
Some limitations observed with the data provided is that for big budget projects there is a very little number of projects that is provided, which makes it difficult to study the
data for projects with bigger budgets and could also potentially affect the decision. Ranges of 35000 to 45000 in outcomes based on goals line graph is a good example where it
may not be representative of the reality.
 
- What are some other possible tables and/or graphs that we could create?
    -Tables based on the backers count could also be analyzed to know how many people will come with respect to dates/categories.
    -A table to study thye effect of spotlight on the rate of success, fail and cancellation.
    -A table with the range of days the project is running (from lauch to end)and how would that affect the succes rate.
    -Tables to study the country effect on the rate of success.
    -Stacked bar graphs can also be used to analyze the data with each bar having all three categories.