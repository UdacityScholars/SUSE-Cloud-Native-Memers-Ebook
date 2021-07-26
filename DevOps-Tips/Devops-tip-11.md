# DevOps Tip 10

**Using log aggregation for troubleshooting and future access**

Logging plays a big part on making our services observable so we could act on any event that might occur. Monitoring clusters in production calls for a cluster wide log aggregation tool such as ELK stack. In Production it's recommended to keep your logs separately from the Kubernetes cluster running your monitored application, so that your logs remain accessible for troubleshooting event (and especially) during cluster outage and issues.
There are few logging aggregation that allows you to just do that without starting from scratch

1. Fluentd

Kubernetes-native, fluentd integrates seamlessly with Kubernetes deployments. The most common method for deploying fluentd is as a daemonset which ensures a fluentd pod runs on each pod. Similar to other log forwarders and aggregators, fluentd appends useful metadata fields to logs such as the pod name and Kubernetes namespace, which helps provide more context. You can read more [here](https://docs.fluentd.org/) on how to get started.


2. ELK


The ELK Stack (Elasticsearch, Logstash, and Kibana) is another very popular open-source tool used for logging Kubernetes.


a. Elasticsearch, provides a scalable, RESTful search and analytics engine for storing Kubernetes logs.

b. Kibana - the visualization layer

c. Logstash - the log aggregator used to collect and process the logs before sending them into Elasticsearch. It's similar with Fluentd.

d. Beats - Filebeat and Metricbeat are ELK-native lightweight data shippers used for shipping log files and metrics into Elasticsearch.

[Here](https://www.magalix.com/blog/kubernetes-observability-log-aggregation-using-elk-stack) is a tutorial that could help you get started with ELK stack for your logging solution.

**References**

[A Practical Guide to Kubernetes Logging | Logz.io](https://logz.io/blog/a-practical-guide-to-kubernetes-logging/)