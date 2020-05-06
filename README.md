# Covid_19 Data Analysis


![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/COVID19.jpg)

<b>Dataset I'm using in this Analysis(Raw Data)</b>

https://raw.githubusercontent.com/CSSEGISandData/COVID-19/web-data/data/cases_country.csv
https://raw.githubusercontent.com/gopisuthar/Covid_19/DataAnalysis/Resources/covid19_Confirmed.csv
https://raw.githubusercontent.com/gopisuthar/Covid_19/DataAnalysis/Resources/covid19_Recovered.csv
https://raw.githubusercontent.com/gopisuthar/Covid_19/DataAnalysis/Resources/covid19_Deaths.csv

<b>Load Libraries</b>

1) <b>Pandas</b> for Read CSV File              
2) <b>Matplotlib</b> for Graphical Visualization                            
3) <b>Datetime</b> for Convert data in Date/Time Format              
4) <b>Numpy</b> for Array
5) <b>Folium</b> for Map Visualization
6) <b>Plotly</b> for High-level Graphical Visualization

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_1.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_2.PNG)


<b>Now, Let's Examine Each of the files using .head() method</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_3.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_4.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_5.PNG)

</b>We're going to see information about our columns name and datatype using .info() method</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_6.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_7.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_8.PNG)

<b>Look up dimension of the DataFrame using .shape</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_inspection_9.PNG)

 <b>Data Cleaning and Data Preprocessing</b>
    Lookup for data who creates inconsistency and rename it
:-) I found those data and made some changes as following:
    <b>for Columns:</b>
    Province/State :-> State
    Country/Region :-> Country
  
![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_Preprocessing_1.PNG)

<b>for Raw:</b>
  US :-> USA
  Korea, South :-> South Korea
  Taiwan* :-> Taiwan
  
![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_Preprocessing_2.PNG)

<b>Let's ensure that our changes has made or not?</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_Preprocessing_3.PNG)

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_Preprocessing_4.PNG)

<b>Data Analysis</b>
Examine the Global Cases of Covid-19:

As of 04-may-2020 the table illustrates, Total Confirmed, Deaths, Recovered, Active Cases throughout the world
and the cases are rising rapidly

<b>Covid-19 Global Data</b>
![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_1.PNG)

 Examine the cases by top 5 Countries by number of Confirmed Cases and we shows USA cases are increasing speedily
<b>Top 5 Countries with Confirmed Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_2.PNG)

 Here we can see that most of the people have died in USA as of rapidly confirmed cases are increased day by day
and other hand, Mortality Rate is higher in UK with 15.03% 
<b>Top 5 Countries with Death Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_3.PNG)

 Now, Extract some of the data from dataset for further analysis and make some new dataframe too
<b>Data Over 10000 Confirmed Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_4.PNG)

<b>New Dataframe to set index as 'Country'</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_5.PNG)

<b>Countries with the Highest Mortality Rate %</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/Mortality_Rate.png)

 The graphs filters out countries with at least 10,000 confirmed cases, Belgium has the highest mortality rate around 16%, which is 1%     more than the second leading country, UK at 15%
 
<b>Top 5 Countries with Confirmed Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/Confirmed.png)

USA has the most active cases, which can be expected due to the slow response on testing procedures and protective measures. There were hundreds of college students and citizens who disregarded the social distancing measures. Some of the affected may not display any symptoms (asymptomatic) along with lack of social distancing could significantly influenced the active cases.

<b>Top 5 Countries with Confirmed Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/Active.png)

USA has suffered the most deaths followed by UK and Italy.

<b>Top 5 Countries with Deaths Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/Deaths.png)
  
USA has recovered with Confirmed cases of Covid-19

<b>Top 5 Countries with Deaths Cases</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/Recovered.png)

# Map Visualization

Look up at Geographically view of Global Covid-19 using folium library and uses <b>OpenStreetMap'</b>

<b>Geographic map with Confirmed,Deaths and Mortality Rate of each Country</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_17.PNG)

Now,Take a look of Geographical scatter plotting of last updated confirmed cases over the world

<b>Scatter Map</b>

![](https://raw.githubusercontent.com/gopisuthar/Covid_19/master/Images/data_analysis_20.PNG)





