# Assignment 01 - Data Visualization of Macau Weather Dataset - Dashboard
> As the assignment of the course, I made a simple dashboard as my analysis and data visualization by running the jupyter code that in the summition.
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
In the dataset that this Assignment provided, I transfer the data **Time** to **Date**, **Month** and **Year** for the convenience of data analysis and visualization. Also, I added a new column **Season** to the dataset for the further analysis of the weather in different seasons.

### Pointout:
In the colum - **Total rainfall (mm)** , data **VST** will be replaced to **0** because it means that the rainfall at the time is less than **0.1 mm** for easier to analyis.

***

## Dashboard Layout
The dashboard layout is simple and clear, which includes a title, a day selecter, a summary and a few graphics(will be talk later). By using the day selecter, the dashboard are generally like this:

![alt text](Picture/Overview.png)

***

## Figure1 - Temperature Trends Over Time in Macau






