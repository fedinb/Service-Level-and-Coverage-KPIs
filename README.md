# Service Level and Coverage KPIs

This code is meant for calculating both weekly and daily Service Level and Stock Coverage values based on inventory reports shared on a daily basis.

Whole process divided in 5 steps is listed below:
1. When new file is uploaded to planning tool, its copy is sent to OneDrive folder. MS Power Automate deals with that.
2. Now when there is a list of files with data per each day, we can stack them with code and use for analytics.
3. Code collects the data and creates a few dataframes for two versions of main KPIs: both daily and weekly Service Level and Stock Coverage.
4. Dataframes for weekly tracking are used in plots that will be sent on Mondays (when all data for previous week is available).
5. Dataframes for daily tracking are united in one table and sent from Tuesday to Friday.

In daily monitoring case, process that starts with non-delimited text files ends with such an e-mail.

![E-mail screenshot](https://github.com/fedinb/Service-Level-and-Coverage-KPIs/blob/main/Daily%20KPI%20e-mail.png)
