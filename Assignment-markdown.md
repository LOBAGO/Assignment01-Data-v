# Assignment 01 - Data Visualization of Macau Weather Dataset - Dashboard
## MC464537 LAO PAK KUONG
> As the assignment of the course, I made a simple dashboard as my analysis and data visualization by running the jupyter code that in the submission file.
***

## Notice:
### The dashboard will be run on the localhost, user can input localhost:8050 to a better view in the browser.

***

## Jupyter codes importing:
For finish my assignment, I used the following libraries and modules to import and analyze the data.

    import dash
    from dash import dcc, html
    from dash.dependencies import Input, Output
    import plotly.express as px
    import plotly.graph_objects as go
    import pandas as pd
     
***

## Data processing:
In the dataset that this Assignment provided, I transfer the data **'Time'** to **Date**, **Month** and **Year** for the convenience of data analysis and visualization. Also, I added a new column **Season** to the dataset(in dataframe) for the further analysis of the weather in different seasons.

### Pointout:
In the colum - **Total rainfall (mm)** , data **VST** will be replaced to **0** because it means that the rainfall at the time is less than **0.02 mm**.

***

## Dashboard Layout
The dashboard layout is simple and clear, which includes a title, a day selecter, a summary and a few graphics(will be talk later). By using the day selecter, the dashboard are generally like this:

![alt text](Overview.png)

- all figure will update according to the day that uesr select.
- all figure will have some tools for better view in the picture (e.g: zoomin, zoomout, reset, autoscale, hover data, etc.)
- all figures will have a short introduction below.

***

## Figure1 - Temperature Trends Over Time in Macau

This graphic mainly shows how three temperature measurements (**mean maximum**, **mean**, and **mean minimum**) temperatures—change over a period.

![alt text](Temp-Trand.png)

In this picture, three line shows three trand of temperature

- Blue line refers to Mean Maximum Temperature.
- Rad line refers to Mean Temperature.
- Green line refers to Mean Minimum Temperature.

Using line-chart can be effectively visualizes temperature trends over time, allowing for easy comparison of different temperature measures, identification of patterns and anomalies, and interactive exploration of data.

***

## Figure2 - Average temperature by date in Macau

This graphic mainly shows the average temperature by days in time priod that user selected, which can be used to analyze the temperature changes and the temperature distribution.

![alt text](Average_Temprature.png)

***

## Figure3 - Total rainfall by month in Macau (Heatmap)

This picture shows the total rainfall by month in the time priod that user seleted,
the color of the block represents the amount of rainfall in that month. The deeper the color, the more rainfall in that month.

![alt text](Heatmap.png)

### Point Out:
Thrugh the heatmap, I find out a outstanding data (2008/06) which the total rainfall is 1204 mm, this is the largest number of total rainfall in the dataset. So I try to find out the reason of this highest record:

  - In middle of 2008 June,  Typhoon **Fengshen** affected a large area of southern China, including Macau. The typhoon brought heavy rainfall.
  - According to announsment by goverment, rain priod in Macau in 2008 May is late to 2008 June.
  - El Niño may also is the reason too.
  
***

## Figure4 - Scatter Plot (Mean Temperature vs Mean reaative humidity)

This picture mainly shows the relationship between Mean Temperature and Mean reaative humidity in the time priod that user seleted.

![alt text](Scatter_Plot.png)

This picture shows that a huge number of data refers to 25°C and 80% relative humidity, which is the most common weather condition in Macau.

***

## Figure5 - Box Plot (Temperature by month)

This picture mainly shows the distribution of temperature in each month in the time priod that user seleted.

![alt text](Box_Plot.png)

***

## Figure6 - Bar Chart (Total rainfall by month)

This picture mainly shows the total rainfall in each month (summerize all year) in the time priod that user seleted.

![alt text](Bar_Chart.png)

***

## Figure7 - Densitity contour of temperature and relative humidity

This picture mainly shows the distribution of temperature and relative humidity in the time priod that user seleted.

The density contour lines represent the concentration of data points in specific regions:

- Darker or thicker contours indicate areas with a higher concentration of data points (higher density).
- Lighter or thinner contours indicate areas with a lower concentration of data points (lower density).

![alt text](Densitity_Contour.png)

***

## Figure8 - Stacked Bar Chart (Average Insolation Duration by season)

This picture mainly shows the average insolation duration in each season in the time priod that user seleted. The stacked bar chart contains four bar, which are spring, summer, autumn and winter. The height of the bar represents the average insolation duration in the time priod.

![alt text](Stacked_Bar_Chart.png)

***










