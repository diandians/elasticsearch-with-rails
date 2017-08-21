# Elasticsearch with rails

This is my first try to use elasticsearch in rails.

## Set up
### Ruby on Rails
Please install ruby and rails on your machine. Windows not recommended. My machine is ubuntu16.04, and I have install rails version 5.0.0.1.

### Elasticsearch 
#### Pre: Install Java on your machine
  Since elasticsearch is written in Java, please install java and set Java environment variables if you haven't install it yet.
#### step 1: Install elasticsearch
  Download elasticseach from [here](https://www.elastic.co/downloads/elasticsearch). Choose zip file and unzip it in your local directory.
#### step 2: Validate Installation
  Get into the directory, ``` cd elasticsearch-[version]```, and run ``` bin/elasticsearch ``` (```bin\elasticsearch.bat``` on windows). Open url: http://localhost:9200 or use curl ``` curl XGET 'http://localhost:9200' ``` Then, you should see something like this:
  ```
  {
  "name" : "T47Fnhf",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "Lgqu4ggsRauT4O-7P2EK2w",
  "version" : {
    "number" : "5.5.2",
    "build_hash" : "b2f0c09",
    "build_date" : "2017-08-14T12:33:14.154Z",
    "build_snapshot" : false,
    "lucene_version" : "6.6.0"
  },
  "tagline" : "You Know, for Search"
}
```
## Basic Usage:
Download it or git clone using ``` git clone https://github.com/diandians/elasticsearch-with-rails.git ```. start rails by ``` rails serve```; at the same time, open anther teminal tab, start elasticsearch by ``` bin/elasticsearch```. Then,you will get there!

## Reference 
More information, please refer to this [article](https://www.sitepoint.com/full-text-search-rails-elasticsearch/)
