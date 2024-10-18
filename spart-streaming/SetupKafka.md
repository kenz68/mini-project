# Setup Kafka

## List all kafka topics

`kafka-topics --list --bootstrap-server ed-kafka:9092`

## Create new topic `topic-test`

`kafka-topics --create --topic test-topic --bootstrap-server ed-kafka:9092`

## Connect to jupyter docker container

`docker exec -it f2a3e793e86d87aa91dd151b30e3ebe64d4273a45878dfab7ca9d06dbf6025a5 /bin/bash`

### Update `apt-get`

`sudo apt-get update`

### Install NCat to jupyter container

`sudo apt-get install ncat`

### Verify `ncat` installation

`ncat -v`

==> `Ncat: Version 7.80 ( https://nmap.org/ncat )`

### Start `ncat` with port `9999`

`ncat -l 9999`

Enter the text in this console to see logs from jupyter console on `docker`

### Get jupyter server list

`jupyter server list` 

### Spark UI HOST `4041` OR `4042`

`http://localhost:4041/jobs/`


