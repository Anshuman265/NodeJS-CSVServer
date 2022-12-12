# CSVServer


Simple node-based CSV adapter for Grafana Simple JSON data source

This is a simple node application to read table or timeseries formatted CSV files as JSON, suitable for Grafana's SimpleJSON data source.

NOTE - CSVServer is really intended for testing and demonstration purposes

## Installation/setup

From a command window, execute the following commands:

```javascript
git clone https://github.com/Anshuman265/NodeJS-CSVServer

npm install

node CSVServer.js
```

## Configuration - Default.ini

On start up, CSVServer initializes a number of internal default settings from values defined in the default.ini file

```
[options]

# default listing port
port=4000

# default CSV data file directory
folder=./csv

# default comma-seperated list of columns treated as datetime types
#datecols=date,time
datecols=date

# default datatime column format (see https://momentjs.com/docs/#/parsing/)
#dateformat=YYYY-MM-DD HH:mm:ss
#dateformat=X

# default flag used to control whether or not Grafana's from and to dates 
#  should be used to filter out unwanted rows from the returned data set
#  valid values : [none, to, from, both]
#datetimefilter=none
```