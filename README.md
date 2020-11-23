
## Consolidated Cases & Issues Project ##

Business use case: provide leadership with a holistic view of critical open cases and associated issues across all Elemental products regardless of deployment platform, in order to be prepared for customer escalation.

Combine data from:

* Salesforce Service Cloud support cases for legacy customers
  * related JIRA issues 
* Paragon support cases for media services customers
  * related Trouble Ticketing ("TT") issues

### Project Overview ###

* Discovery around available data for media services, and obtain access
* Discover data structure
* Extract data from AWS DW TT tables & Paragon case table 
  * AWS Support BI team decided to send data to an S3 bucket in the Elemental account
    * Create Redshift table for data from S3 https://gist.github.com/lizpdx/f928a176faad21c5fc9f0b31c2ebe933
    * Utilized internal tool "Hammerstone" to pull data into Redshift from S3 https://gist.github.com/lizpdx/38ff0e0025222d83588aee9ba7eadbe0
  * TT tables available through subscription via Hoot from AWS "Andes" data lake
* Load data into the AWS Elemental ecosystem
* Transform, join data
* Surface data via Tableau for dissemination to end users


### CCR data flow diagram ###
https://github.com/lizpdx/cashapp/blob/main/flow.png


### Tableau Prep flow to combine 4 data sources and publish to Tableau Server ###
https://github.com/lizpdx/cashapp/blob/main/Prep.png



## Other Projects ## 

### SQL code for ticket metrics ###
Business use case: provide visibility into Elemental Support engineer workload for media services support cases, which are assigned to AWS Support when resolved.
https://gist.github.com/lizpdx/96d374b3cea61377c3cc1a33caec3ce4

### Ruby script to create JIRA tickets ###
Business use case: provide visibility into Hosting Engineer workload across the team, and a consistent customer experience with accurately set expectations.
https://gist.github.com/lizpdx/40a697a196395454fbcb2ef54aa4ec39
