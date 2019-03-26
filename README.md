# Learning Elasticsearch and Kibana

Connect to Kibana node:

```
docker exec -it kibana /bin/bash
```

Then run

```
curl http://elasticsearch:9200/
```

Kibana URL: `http://localhost:5601`

## Commands

The below commands can be run either from a command line as it stated below via Postman.
**Note:** Pay attention to the type of the request: GET/POST/PUT etc.

`curl http://localhost:9200/_cluster/health\?pretty` - check cluster health
`curl -X PUT "localhost:9200/customer?pretty"` - Create and index called `customer`