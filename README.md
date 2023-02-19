# flink-experiments


- Prerequisites:
    Java 11 or greater

- docker pull flink


- Clone this repository


## Running Flink
```
flink-experiments #>  docker compose up
```


## Submiting a job
Inside the jobmanager container terminal run:

```cd /opt/flink```


```./bin/flink run ./flink-data/jobs/WordCount.jar --input ./flink-data/input/data.txt --output ./flink-data/output```


### Exploring results:
```cat flink-data/output/*/part*```

Or in the UI: http://localhost:8081/#/overview