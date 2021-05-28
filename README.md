# Config project ELK

## Prerequisite of project

* docker
* docker-compose

Config environments into operation system:

* ELK_VERSION
* ELASTICSEARCH_URL
* ELASTICSEARCH_PASS

For more details check file `.env_development` in projects `Elasticsearch`, `Logstash`, `Kibana`.

---


**Default ports:**

  - 5044: Logstash Beats input
  - 5000: Logstash HTTP input
  - 9600: Logstash monitoring API
  - 9200: Elasticsearch HTTP
  - 9300: Elasticsearch TCP transport
  - 5601: Kibana

---

## Services:

**Example start project:**

```
cd docker_elasticsearch
docker-compose up -d
```

**Example Restart:**

```
cd docker_elasticsearch
docker-compose restart elasticsearch
```