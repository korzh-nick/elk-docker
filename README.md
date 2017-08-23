# Elasticsearch, Logstash, Kibana with Curator
**fork [ELK-docker](https://github.com/sqshq/ELK-docker.git)**


## Description
- [Elasticsearch](https://hub.docker.com/_/elasticsearch/) - official image with data volume in `elasticsearch/data` directory
- [Logstash](https://hub.docker.com/_/logstash/) - official image 
- [Kibana](https://hub.docker.com/_/kibana/) - official image
- [Curator](https://github.com/elastic/curator) - lightweight 50mb container which could run scheduled tasks against Elasticsearch to manage its indices (delete, optimize, snapshot, etc)


## Setup
1. Install [rsyslog-ansible](https://github.com/korzh-nick/rsyslog-ansible)
2. Install Docker and Docker Compose on the ELK host
3. Clone this repository and hit `docker-compose build`

## Usage
Start everything with one command:
```
docker-compose up -d
```

Keep track of your containers execution. For example, controll Curator scheduled tasks:
```
docker-compose logs curator
```
