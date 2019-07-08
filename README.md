# Security configuration for ElasticSearch and Kibana

General instructions for setting ES via docker-compose are available at https://www.elastic.co/guide/en/elasticsearch/reference/7.2/docker.html.

To set up the security, follow instructions on https://www.elastic.co/guide/en/elasticsearch/reference/7.2/configuring-tls-docker.html.

Check the cluster is running fine :

```
curl --cacert certs/ca/ca.crt -u elastic:ElasticPassword https://localhost:9200/_cat/health\?v
```

General instructions for setting Kibana via docker-compose are available at https://www.elastic.co/guide/en/kibana/current/docker.html

To set up the security, follow instructions on https://www.elastic.co/guide/en/kibana/current/configuring-tls.html

Configure the password to be used by Filebeat in `config/filebeat.yml`.
