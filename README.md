perl-AWS-Cloudwatch
===================

Devops code + utility to painlessly upload data into AWS Cloudwatch

Systems like Nagios and Icinga are great -- when you're not on the Amazon cloud.
Once you move to the cloud it's hard to beat AWS Cloudwatch.

Cloudwatch is an amazing, easy, friendly way to aggregate system data, trigger alarms,
and send those alarms to lots of interesting systems.

However there is one drawback to cloudwatch -- it can't (easily) access statistics from
services running on the server.   I found myself longing for the days when I knew how 
much disk space my volume had, when my servers were running low on memory, when my
beanstalkd queues were piling up. 

Plus being able to automatically do stuff - like "muster reinforcements" (aka AutoScale)
for servers which are busy, it's hard to do that without visibility into an application.

Anyway, this solves those problems. 

Includes plugins for Monit, Beanstalkd, Mongodb and Redis.

