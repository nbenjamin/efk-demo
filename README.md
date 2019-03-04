# efk-demo
Fluentd demo

In this example shows how to use elastic search, kibana and fluentD.

![screen shot 2019-03-04 at 4 57 37 pm](https://user-images.githubusercontent.com/870715/53765741-e2a91f00-3e9e-11e9-8452-04ba15183d10.png)


### How to run

Execute the following command to start efk
```bash
docker-compose -f docker-compose.yaml up
```

##### Elastic Search URL
```properties
http://localhost:9200/
```

##### Kibana URL
```properties
http://localhost:5601
```

Currently, we configured httpd server logs to publish directly on fluentD, so when you execute the following command 
message will trigger to elastic search and you find those in Kibana.
