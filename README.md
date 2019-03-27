# Learning Elasticsearch and Kibana

## Requirements

TBA

## Install

TBA

## Usage

### Start the cluster

Run `docker-compose up -d`

### Check if everything is working

1. Connect to Kibana node via terminal:

```
docker exec -it kibana /bin/bash
```

1. Then run

```
curl http://elasticsearch:9200/
```

To access Kibana web-interface got to `http://localhost:5601`

### Elasticsearch commands

The below commands can be run either from a command line as it stated below via Postman.
**Note:** Pay attention to the type of the request: GET/POST/PUT etc.

- `curl http://localhost:9200/_cluster/health\?pretty` - check cluster health
- `curl -X PUT "localhost:9200/customer?pretty"` - Create and index called `customer`
- `curl -XPOST 'localhost:9200/shakespeare/_bulk?pretty' --data-binary @shakespeare.json -H 'Content-Type: application/json'` - Bulk load `shakespear.json`