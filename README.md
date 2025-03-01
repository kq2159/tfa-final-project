# tfa-final-project
Group 16: Ellen Wang, Kathy Qian

Out of the two members of our group, we pick "10036" as our ZIP code.

In a first Jupyter notebook called `Top10.ipynb`, 
we analyzed what the top 10 causes of calls to 311 are in your chosen ZIP code, 
and calculated how many total incidents of each of these 10 types there have been in the year 2020. 
The answer is a `pandas.Serie`s which is called top10 (as a Python variable), in descending order by number of incidents, 
and containing as its labels the incident type (a string) and as associated values the total number of incidents of this type in 2020.
The top 10 types and numbers of incidents in the area of zip code 10036 are:
Noise - Residential                    879
Non-Emergency Police Matter            615
Noise                                  614
Homeless Person Assistance             547
NonCompliance with Phased Reopening    496
Noise - Street/Sidewalk                456
Illegal Parking                        432
Noise - Commercial                     416
HEAT/HOT WATER                         395
Homeless Street Condition              374

In a second Jupyter notebook called `Parking.ipynb`, 
we analyzed whether illegal parking incidents are a larger fraction of total 311 incidents in our chosen ZIP code than they are in general. 
Specifically, compute the total number of parking incidents in your ZIP, and the total number of all incidents 
-- is this fraction greater than or smaller than the total fraction of parking incidents across all ZIP codes? 
The answer is in the form of a single bool called `higher_parking_proportion`,
which is True if your ZIP contains a higher proportion of parking incidents than the global value, and False otherwise. 
For instance, if there were 200 parking incidents in your ZIP, and 1000 total incidents in your ZIP, a rate of 20%, 
but the global parking incident rate was 3000 parking incidents out of 10000 total, a ratio of 30%, 
we would assign `higher_parking_proportion = False`.
The proportion of parking incidents in the area of zip code 10036 is approximately 4.781%, 
while the proportion of parking incidents in the global area is approximately 7.487%.
Since 4.781% is smaller than 7.487%, we would assign `higher_parking_proportion = False`.
