# Module 3 Challenge
## Overview of Election Audit
For this challenge, we used python to run an election audit and analysis, to report and analyze the winners of the election, as well as county specific statistics. The purpose was to provide a code that would provide useful information to determining election outcomes and data regarding voter habits and distributions, at the request of an election comission. 
## Election-Audit Results
The following is an overview of the results of the Audit itself, taken from the printout of the terminal when the code is run:

![Screen Shot 2022-09-29 at 12 27 53 PM](https://user-images.githubusercontent.com/112847821/193124575-31579e9e-ff2f-4f81-9f68-f3dd415e1bee.png)

-Denver County had the most votes by far, with 306,055 total votes cast, making up a whopping 82.8% of the total vote count.
-The following is a breakdown of the number of votes each candidate received, as well as their percentage of the total votes, as per the Terminal Printout:

![Screen Shot 2022-09-29 at 12 29 30 PM](https://user-images.githubusercontent.com/112847821/193125537-b83dd0f6-a243-485c-91e5-8af932351ddf.png)

-Diana DeGette won the election by a landslide, receiving 272,892 total votes, 73.8% of the total vote. 
## Election Audit Summary
This script is obviously useful for this election, and thereby other congressional elections, as it allows us to examine total votes per county, and candidate specific votes per county as well, allowing us to properly audit and report election results. However, it can certainly be modified to be used for any election. 
Most obviously, this could be adapted from reviewing 3 counties to looking at a higher number of counties, state turnouts, and other such distributions. For example, we could add in a modified version of the below loop, that would allow us to also loop through state voter data, as well as county data:

![Screen Shot 2022-09-29 at 12 46 53 PM](https://user-images.githubusercontent.com/112847821/193127784-e2e8e87d-788c-4d93-8ba5-7a4083a8a16a.png)

We would of course have to also create a dictionary for the state and state vote values of course, using code like the following in addition to lines 21 and 22 under section #1

![Screen Shot 2022-09-29 at 12 48 48 PM](https://user-images.githubusercontent.com/112847821/193128062-b019e3ae-91d5-4978-bb4a-ddfcae545eba.png)

Here, we could also add the following:
>state_list[]

>state_dict{}

Substituting state based variables for the county based variables originally used and putting the loop before or after the county loop allows us to also examine state data. Of course, it would be most useful if the county loop was nested within the state loop, so that data was returned for all counties within a specific state, so as to provide cohesive and useful data. 
Additionally, we could also utilize additional calcuations to provide us with more granular audit information. For example, we could breakdown the candidate votes by county, allowing us to examine what the candidate distribution was like in a specific county. 
To accomplish this, we could insert a series of if-statements to allow us to also determine and store those variables, in a for loop like in step 6, like the below:

>if candidate_name = (whichever candidate we are examining) in county_dict:

>   candidate_county_votes=countyvotes

And then we can use this variable to print, store, or whatever we would like. 
