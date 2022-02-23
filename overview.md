# Overview of the Elastic Stack

## X-PACK

Additional features for Elasticsearch and Kibana.

For example:
- Security (authorization, authentication, permissions)
- Monitoring of elasticsearch (memory, CPU usage)
- We can setup alerting based of monitoring (email, slack, etc.)
- Reporting
- Machine learning
- Graph - show relationship in our data
- SQL - enables a possibility to send SQL queries to Elastic search via HTTP


## KIBANA

Analytics and visualisation platform which works directly with Elasticsearch engine

## BEATS

Collection of so-called data shippers. These data shippers have one purpose. We install the on servers and they sand data to Elasticsearch.
- FILEBEAT - used to collect data from log entries
- METRICBEAT - collects sys and service metrics. Includes modules for common services (nginx and MySQL)
- PACKETBEAT - Network data. HTTP requests or DB transactions
- WINLOGBEAT - Collects Windows Events lOGS
- AUDITBEAT - Collects audit data from Linux
- HEARTBEAT - Monitors service uptime

## LOGSTASH

Has been used to process logs from applications and send them to Elasticsearch. Logstash can receive a data, manipulate this data or send events based on the data.
Logstash recieves events from one or more inputs, process then, and sends them to one or more stashes.
To work with unprocessed data we use GROK - it's a basically regexp pattern which helps us process strings inside logstash.



![Screenshot 2022-02-23 at 14 02 33](https://user-images.githubusercontent.com/90422557/155324476-9dc14895-3c8f-4df1-834d-12ebf49a85a1.png)



