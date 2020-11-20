# cashapp

## Consolidated Cases & Issues Project ##

Combine data from:

* Salesforce Service Cloud support cases for legacy customers
  * related JIRA issues 
* Paragon support cases for media services customers
  * related TT/SIM-T issues

### Project Overview ###

* Discovery around available data for media services
* Obtain data access
* Extract data from AWSDW & Paragon 
* Discover data structure
* Load data into the AWS Elemental ecosystem
* Map requirements to available data fields
* Transform, join data
* Analyze

### CCR data flow diagram ###
https://github.com/lizpdx/cashapp/blob/main/flow.png

### Create Redshift table for data from S3 ###
https://gist.github.com/lizpdx/f928a176faad21c5fc9f0b31c2ebe933

### HS code to pull data into Redshift from S3 ###
https://gist.github.com/lizpdx/38ff0e0025222d83588aee9ba7eadbe0

### Tableau Prep flow to combine 4 data sources and publish to Tableau Server ###
https://github.com/lizpdx/cashapp/blob/main/Prep.png



## Other Projects ## 

### SQL code for ticket metrics ###
https://gist.github.com/lizpdx/96d374b3cea61377c3cc1a33caec3ce4

### Ruby script to create JIRA tickets ###
https://gist.github.com/lizpdx/40a697a196395454fbcb2ef54aa4ec39
