# United States Drug Arrests
## Motivating Question
I was recently watching the show Narcos on Netflix and it made me curious about the effectiveness of the War on Drugs in the United States. 
For this project, I am analyzing drug arrest data from 1994 to 2016 in the United States.
The main question that I set out to answer at the start of this project is this: Does the number of manufacturing arrests impact the amount of possession arrests? 
## Data Source
I sourced my data from the [FBI Crime Data Explorer](https://crime-data-explorer.fr.cloud.gov/downloads-and-docs) database. The description of the dataset on the site is not accurate, as it claims to have the monthly number of arrests and to be broken down by age, sex or age, and race. In reality the dataset contains yearly totals with no data on sex, age, or race. The dataset is a compilation of data submitted by participating police agencies.
## Data Cleaning Process
This dataset was already organized and required very little cleaning. I deleted two columns, one contained no data and the other contained irrelevent ID numbers. In R I created a copy of the dataset and I adjusted the arrest numbers to measure the number of crimes for every one hundred thousand people in order to establish measure for the rate of crime.
## Visualization
The scatterplot comparing the rate of arrests for manufacturing and possession clearly shows a sharp decline in the rate of manufacturing arrests and an increase followed by a decrease in the rate of possession arrests. This shows that total manufacture rate does not correlate with total possession rate. The bar graphs compare the rate of arrests for manufacturing and possession of each drug category. The most interesting part of this data is the manufacturing rate compared to the possession rate for opioids and synthetics. The opioid possession rate of arrests closely follows the manufacturing rate until 2014 where the possession rate starts to increase even though the manufacture rate continued to decline. A similar trend can also be seen in the synthetic category. As the manufacturing rate increases so does the possession rate until 2014 where the manufacturing decreases but the possession rate continues to increase.
#### Figure 1
![image](https://user-images.githubusercontent.com/79553303/115976277-1fbe4880-a521-11eb-8158-59b9ba1fc062.png)
#### Figure 2
|   |  |
| ------------- | ------------- |
| ![image](https://user-images.githubusercontent.com/79553303/115975190-82aae200-a517-11eb-9416-96c4f4140c90.png)  | ![image](https://user-images.githubusercontent.com/79553303/115975195-8dfe0d80-a517-11eb-93c6-f937019ab75c.png)  |
## Analysis
I analyzed the opioid and synthetic manufacturing and possession arrest rates using boxplots. The mean of the opioid manufacturing rate is lower in the IQR than the mean of the opioid possession rate. The IQR of the opioid manufacturing rate is lower than the IQR of the opioid possession rate. The IQR of the synthetic manufacturing rate is much smaller than the IQR of the synthetic possession rate. The IQR of the synthetic manufacturing rate is higher than the IQR of the synthetic possession rate. The mean of the synthetic manufacturing rate is lower in the IQR than the mean of the synthetic possession rate. The outlier on the synthetic manufacturing rate was not removed because it shows how the rate increased very rapidly.
#### Figure 3
![image](https://user-images.githubusercontent.com/79553303/115976762-23a09980-a526-11eb-9507-0de224a5199b.png)
#### Figure 4
![image](https://user-images.githubusercontent.com/79553303/115976767-28fde400-a526-11eb-98a0-b4bd53c104f1.png)
