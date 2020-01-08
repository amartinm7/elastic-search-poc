![elastic-search](./_media/elasticsearch-logo.png)

# Elastic-search-poc

Elastic search is an engine based on lucene. 
ELS is adding a cloud layer over lucene to be available over the network.
Said that, we have to think is in how many nodes and how many shards have our cluster. 
Keep in mind that ELS have indexes and aliases to refer to these indexes. 
The aliases helps to manage the indexes when you have to create new ones and keep on working.
Another think is an index can contains several types of documents and every document is an schemeless json document over to search on. 
So you can define as many indexes as you like, and as many types as you want.

We have created a docker-compose file to run ELS with Kibana which the ELS console.
Very important: locate a lot of memory in the docker manager engine in order to handle the ELS infrastructure. 

# ELS Spring Data 

# ELS Jest Client

### Scafoldding the project, common steps

Install gradle wrapper
```
gradle wrapper
```

Create scaffolding project
```bash
spring init --build gradle --name=elastic-search-poc --dependencies=web,data-jpa,mysql,devtools,thymeleaf --package-name=com.amm.artifact elastic-search-poc
```

```bash
./gradlew  build --stacktrace --info
./gradlew --stop && ./gradlew clean build
```


![elastic-search](./_media/illustration-home-hero-get-started-elasticsearch-585x530.png)


https://www.elastic.co/guide/en/elasticsearch/reference/7.5/docker.html
