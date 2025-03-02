# FSAE Result Database

By: [Steffano Martinez](https://www.linkedin.com/in/steff2019/) - email: steffano1213@gmail.com


License: MIT 

### What is this repository?
This repository hosts all the results from different FSAE competitions, with said data in json format. Enabling the ability for you or your team to perform any analysis and metrics.

> [!NOTE]
> As of now, this repository has processed **only** the FSAE-Michigan-IC event from 2008- up until the most recent competition. More events will be added in the future.

### Why json? Also, why did you not ask event organizers for the data in the format you wanted?
Two points:
 1. Initially I wanted all the data in a csv format, but then I found out that with json you can have structured data to query quickly, and you can still transform it into csv if you need it.
 2. A contact from the event for Michigan FSAE mentioned that they get the data from multiple streams/sources, and so they just concatenate and get a PDF out.

Also: It looks like most events return a PDF for their results.

### Ok, so how hard is it then to get all the data for all competitions?
Very.

The issue with PDF's is that they tend to not follow a standardized format, there was an illusion from me to think that a table PDF == table parsing with PDF tools, but later realized that they tend to:
1. Have incompleted or unnamed or ghost columns.
2. Row data has trash values.
3. Text is written everywhere outside of a table, for humans to read, but not for parsing. 

> [!NOTE]
> I am working on a template based extraction tool, with the ability for the user to enter some info about the table and have the tool get the data cleaned and structured, but its WIP.

### Can you give an example of how to use this data?
[IC - Michigan Analysis](https://steffmartinez.grafana.net/public-dashboards/33ac6326c70b4c0db4c8de1999ea6e32) 

In the website above, I have a self-hosted grafana dashboard that takes in offline datasources and allows me to quickly visualize graphs to show any metrics, take a look.

### Why would I want to look at past data?

Quantify your overall performance by looking at the trends on your team's previous results. 

With 4 dynamic events, you are able to see how consistent your team is improving or regressing based on vehicle architecture, driver performance, and other factors. 

This can aid you in backing design decisions on top of raw testing data, draw solid vehicle goals, from cost to performance, so that you can stand your ground with more confidence in the static events, remember, its a project management competition, not a race.




