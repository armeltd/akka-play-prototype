# akka-play-prototype

Simple project with Play and Akka Cluster to boostrap a POC quickly a technical feature on a microservice stack similar to tdc local stack

## Architecture

### Overview
![architecture](doc/architecture.png)


### Technical features
 - Async computing with scala Futures
 - Akka actors messages (local and remote)
 - Akka cluster (with constructr)
 - Play endpoints


### Versions
 - Scala 2.12.6
 - Play 2.6.12
 - Akka 2.5.14

## Build
```
sbt docker:PublishLocal
```
## Run
```
docker-compose up -d
```

## Usage
```
./call.sh 10
```
Sends 10 requests on the S1 service each of them propagaging messages to other services