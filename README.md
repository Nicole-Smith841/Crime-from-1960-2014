# Crime-from-1960-2014 
This data was obtained through kaggle.com
https://www.kaggle.com/datasets/mahmoudshogaa/us-crime-rates-1960-2014

Here is a link to the Goolge Colab https://colab.research.google.com/drive/1hSLtZvRD4u3JZo5tzqyAfWqP1QUZBKGS?usp=sharing

Where did I find this source?: After looking through various versions of crime data, https://www.kaggle.com/datasets/mahmoudshogaa/us-crime-rates-1960-2014 has what I was looking for. As far as reliability goes, kaggle.com has a good reputation regarding data handling and the kind of data allowed on the platform, therefore, I am taking the data at face value and it being reliable if not accurate for my queries. 

Hypothesis: The trends of data will have highpoints, however the overall data will show an overall  negative trend. 
NOTE: This data set is a compilation of crime across the US, it is not specific to state/city.  

Process: First, load in the necessary data and libraries in python and use df.info() to look at the columns, and types of data  that is being used. Looking at the output, there are 11 columns that are all the same data type, and no null values. 

![Cap 1](https://github.com/user-attachments/assets/696bb1e0-a022-4860-b5e1-185dac934a17)

Next, look for null values and duplicates, even though it showed no null values in crime.info() it is good to be As shown below, there are no duplicates and there are no null values in the data set. crime.info() showed that the Dtype was int64 across the board, as such there does not need to be any conversions into different data types. However, some of the numbers are excessively large so we will convert some columns so that we have no scientific notations. After that, everything is standardized and is ready for the next steps. 

Then, we are going to look at the summary of the data, things like the mean, standard deviation the min and the max. At a glance (excluding Year, Total and Population) it looks like property has the highest mean, property has the highest amount, and Murder had the lowest. 

![Cap 4](https://github.com/user-attachments/assets/a43c978b-cf0e-4fd7-adc9-c07a321b2264)

Now plot/show the data in varying graphs.
Here is a graph of all the crimes over the years 

![Cap 5](https://github.com/user-attachments/assets/0c29fe04-5acf-4cf7-9cfd-0eefc6990c82)

Here is a bar graph showing the amount of crimes per year

![Cap 6](https://github.com/user-attachments/assets/38c13071-26d5-482f-9235-0d77e9194aff)

Here is a line regression chart of crimes over the years

![Cap 7](https://github.com/user-attachments/assets/ffb733db-07af-4c7f-a4ba-a262ca0b1297)

Analysis: (please note that the numbers on the side of the charts are in short-hand and are fractions of the total number) Overall, what are these graphs showing us? For the line graph, it shows that there seems to be quite the difference in numbers between property crimes and everything else. With the more despicable crimes (Murder, Rape, Assault) having the lower crime numbers. In addition, it would seem that there is a negative trajectory for crime with a peak in the 1990’s. The bar chart confirms this with the total number of crimes being in the year of 1992. The line regression chart is interesting as it seems to show that there is a positive trajectory of crimes and after a while, the number should increase. However, due to the unpredictability of life, it could be possible to reject the line regression as there are many other factors in play. 
