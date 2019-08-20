## BI dashboard for point of sale (POS) system

### Overview
The following details a dashboard system that derives its' data from a point of sale (POS) system. It was deployed in Python (Flask, Dash) and HTML/JS front-end. This project was created by a team of three: a designer, frontend programmer (HTML/JS) and me (Python).

Please note: this dashboard system is designed for RTL languages, specifically Hebrew. Graphs and information display are designed to account for differences that derive from RTL languages. In some cases, this might seem counter-intuitive or mirrored from LTR design.

An example is deployed on Heroku (https://www.heroku.com/) on the following address: https://young-everglades-25667.herokuapp.com/ (please allow for a couple of minutes loading time).

### BI dashboards

This example includes 4 dashboards:
1. Daily summary (7 days)
2. Categories summary
3. Upcoming events 
4. Forecast

<img src="https://github.com/AsafGazit/BI-dashboards/blob/master/img/mm.PNG" alt="Main menu screenshot" width="50%" height="50%">

### Baselines

For most information presented, two baselines for comparison are used: last week's value and 12 weeks average. For example, this week's Tuesday's revenue is displayed in context to last week's Tuesday's revenue and the 12 weeks Tuesday average. 
This aims to allow for relevant benchmarks which filter some seasonality effects in an intuitive way for the user.

### Interactive

The dashboards allow for drill down information using simple interaction. For example, in daily summary every, clicking on a day revenue bar will show that day's hourly revenue distribution.

<img src="https://github.com/AsafGazit/BI-dashboards/blob/master/img/hoursdetails.PNG" alt="Prophet forecast screenshot" width="50%" height="50%">

### Upcoming events schedule

To alert the business of any upcoming events, an events dataset which was compiled and compared with past performance. This allows to capture and highlight events which might have an impact on ongoing operations.

<img src="https://github.com/AsafGazit/BI-dashboards/blob/master/img/events.PNG" alt="Upcoming events screenshot" width="50%" height="50%">

### Forecast

The forecast page use's Facebook's Prophet (https://facebook.github.io/prophet/) to project the upcoming 90 days.

<img src="https://github.com/AsafGazit/BI-dashboards/blob/master/img/forecast.PNG" alt="Prophet forecast screenshot" width="50%" height="50%">
