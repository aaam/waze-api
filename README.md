##waze api [![Build Status](https://travis-ci.org/Nimrod007/waze-api.svg?branch=master)](https://travis-ci.org/Nimrod007/waze-api) wrapping waze live map

showing route duration, distance, tolls, diractions and notifications.

#### 2 steps and your up & running!

##### download [waze-server](https://github.com/Nimrod007/waze-api/releases/download/1.0/waze-server.jar)
##### run the server (port 8080) :
 ```bash
 java -jar waze-server.jar server
 ```
 
##### send a request:
```bash
curl -v "http://localhost:9090/waze/routesWithDirections?end=156+5th+Avenue%2C+New+York%2C+NY+10010&start=6+East+57th+Street%2C+New+York%2C+NY+10022" -H "Accept: application/json"
```
 
 
##### run the server with custom port:
 ```bash
 java -Ddw.server.applicationConnectors[0].port=9090 -Ddw.server.adminConnectors[0].port=9091 -jar waze-server.jar server
 ```
##### run the server with custom config (see [conf.yml](https://github.com/Nimrod007/waze-api/blob/master/src/main/resources/conf.yml]) for example):
 ```bash
 java -jar waze-server.jar.jar server conf.yml
 ```

====================================
Blog about it:

http://www.nimrodstech.com
====================================
