# lmlogstash
Logstash repo for LogicMonitor Logs. 

In order to use this pipeline you will need to install the "logstash-output-lmlogs" logstash plugin. 
```
logstash-plugin install logstash-output-lmlogs
```

Don't forget to edit your pipelines.yml file and add the following lines to your pipeline config. 
```
- pipeline.id: nutanix
  path.config: "/etc/logstash/nutanix/*.conf"
```

Documentation can be found here -> https://www.logicmonitor.com/support/lm-logs/logstash-logs-ingestion
