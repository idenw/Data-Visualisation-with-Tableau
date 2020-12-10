Data Exploration
In this part, you will create 28 worksheets. The number at the beginning of each item below represents the sheet number. You must put that number before each sheet name. Choose any sheet name you want. For instance, a sheet name for the first item below may be 1-Number of Records

1 - Go to Sheet 1 (your workspace) and find how many records the data set has.
2 - Identify the columns with null values and hide the columns that contains just null values
3 - Combine Stop Date and Stop Time and create a field named Stop Datetime
4 - Create a horizontal bar chart displaying count of violation types. Observe that there are null values. Think about how to deal with the null values. Create a new field named Violation-Updated. Replace null values with Unknown. Change the old Violation field with Violation-Updated.
5 - Create the horizontal bar chart above, but this time your chart will display each violation type’s percentage to the total.
6 - What is the percentage distribution of violation type within the female? (Suggested Chart Type: Horizontal Bar Chart)
7 - What is the percentage distribution of violation type within the male? (Suggested Chart Type: Horizontal Bar Chart)
8 - What is the percentage distribution of violation type within all? (Suggested Chart Type: Horizontal Bar Chart)
9 - What is the numeric distribution of stop outcome? (Suggested Chart Type: Vertical Bar Chart)
10 - Create a new field named Stop Outcome-Updated and change the null values with Unknown. Update the chart according to the Stop Outcome-Updated
11 - What is the percentage distribution of stop outcome within female?
12 - What is the percentage distribution of stop outcome within male?
13 - What is the percentage distribution of stop outcome within male & female?
14 - What is the percentage distribution of Searched Conducted within male & female? (Suggested Chart: Treemap)
15 - What is the numerical distribution of search type? (Suggested Chart: Highlight Table)
16 - What is the number of search type that contains Protective Frisk?
17 - What is the numerical distribution of search type that contains Protective Frisk by gender?
Are you more likely to get arrested at a certain time of day? Are drug-related stops on the rise? When a police officer stops a driver, a small percentage of those stops ends in an arrest. This is known as the arrest rate. In this exercise, you'll find out whether the arrest rate varies by time of day. First, you will calculate the arrest rate across all stops. Then, you'll calculate the hourly arrest rate by using the hour attribute of the index. The hour ranges from 0 to 23, in which: 0 = midnight 12 = noon 23 = 11 PM.
18 - Calculate the arrest rate for every 100 stops.
19 – How many stops are conducted per hour?
20 – Calculate the arrest rate per hour per 1000 stops
In a small portion of traffic stops, drugs are found in the vehicle during a search. You will assess whether these drug-related stops are becoming more common over time. The Boolean column drugs_related_stop indicates whether drugs were found during a given stop. You will calculate the annual drug rate by resampling this column, and then you'll use a line plot to visualize how the rate has changed over time.
21 - How many stops are conducted over years? Add an average reference line.
22 – Calculate the annual rate of drug found stops per 1000 drug related stops.
The rate of drug-related stops increased significantly between 2005 and 2015. You might hypothesize that the rate of vehicle searches was also increasing, which would have led to an increase in drug-related stops even if more drivers were not carrying drugs. You can test this hypothesis by calculating the annual search rate, and then plotting it against the annual drug rate. If the hypothesis is true, then you'll see both rates increasing over time.
23- Create two separate chart that displays annual rate of drug found per 10000 Drug-Related Stops to Search Conducted.
The state of Rhode Island is broken into six police districts, also known as zones. How do the zones compare in terms of what violations are caught by police? In this exercise, you will create a frequency table to determine how many violations of each type took place in each of the six zones.
24 - Create a frequency table (or crosstab) that displays district by violation.
25 – Create a side by side chart that displays numerical distribution of district by violation.
25 – Create a side by side chart that displays numerical distribution of district by violation. (Create a side-by-side bar chart)
26 – Create a side by side chart that displays numerical distribution of district by violation. (Create a stacked bar chart)
Converting stop durations to numbers
In the traffic stops dataset, the stop_duration column tells you approximately how long the driver was detained by the officer. Unfortunately, the durations are stored as strings, such as '0-15 Min'. How can you make this data easier to analyze? In this exercise, you will convert the stop durations to integers. Because the precise durations are not available, you will have to estimate the numbers using reasonable values:
Convert '0-15 Min' to 8
Convert '16-30 Min' to 23
Convert '30+ Min' to 45
27 - Create a calculated field named Stop Duration – Time Adjusted and apply the encoding above. Then, create a view that displays average stop duration time by Violation.
28 - What is the age distribution? How do you characterize the distribution in skewness?