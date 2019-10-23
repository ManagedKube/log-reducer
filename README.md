Log Reducer
==============

The problem this project is trying to solve is that pushing logs like VPC Flow Logs to your logging solution can put strain
on the logging system resources and can cost you a lot of money.  If you are running your own logging cluster or using a
SaaS service such as Splunk, SumoLogic, Loggly, etc.  This project will help you out.

VPC Flow logs are very useful but enabling this can generate a lot of logs per day.  Ingesting all of these logs into your
logging system can be costly.  It will increase your overall usage of the system.  This might mean you need more nodes or
you need to pay for a higher tier of daily ingest level.  

Each individual VPC flow log is not very useful.  The aggregated set of the logs and the information it gives you is useful.
By ingesting all of the VPC Flow Logs into your system means most of what is ingested will never be searched on or utilized.
Instead you want to ingest a representative sample of the logs and produce insights from it and put that into your logging
system.

