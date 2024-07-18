# EDA

In this section, I learned the data, cleaned it, analyzed it, and gained insights

I started by cleaning the column names from unwanted spaces, then dropping columns with all zeros and duplicated columns leaving only the first one in every duplication

I found out all the columns were numeric except for the categorical labels, some of them binary and some continues 

There are 6 different labels were 'BENIGN' is regular communication and the rest are attacks

There are 30094 different ports. The main ones are 80, 53, 443

In order to better understand all the Features I split my analyz to different categories:
1. Flow-based Features
2. Basic Features
3. Timing-Base Featurs
4. Content-Base Features
5. Header-Base Featurs
6. Packet-Base Features
7. Flag-Base Features
8. Active-Base Features
9. Idle-Base Features
10. Remaining Features


For each features group I check characteristics like mean, std, min, max values, plotted distribution for continues data and bar-plot for binary data and checked for correlation with a heat map

I can see that most features are really wide spread. most of the values are small around zero and some are much higher. That affects the STD making it much higher than the mean. That means we need to scale them to make better models.

From the correlation heat map we can see that many features have a strong correlation with each other and maybe can be ignored

Some features have infinate size and are hard to work with 

Some binary features are really biased to one tag

In conclusion there are a lot of features. some of them can be droped doe to correlation with other features, values that are too scattered or lack of diversity 

