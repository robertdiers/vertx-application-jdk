# vertx-application-jdk
REST application including Vert.x timers, Vert.x JDBC, Vert.x web client and Vert.x RxJava.
 TestController is used to try out the different features and to compare them. 

**Build the service and test it**

`mvn clean install`

Please use JDK (1.8+) to start the server:

`cd target`

`java -jar vertx-example-1.0.0-SNAPSHOT-fat.jar`

**URLs:**

http://localhost:8080/user/getall

http://localhost:8080/user/get?name=John

http://localhost:8080/fancy/get?name=John

Sync
http://localhost:8080/test/sync

Stream
http://localhost:8080/test/stream

ParallelStream
http://localhost:8080/test/parallelstream

RxJava (async)
http://localhost:8080/test/rxjava

Parallel RxJava (async)
http://localhost:8080/test/parallelrxjava

Webclient
http://localhost:8080/test/webclient

JDBC Database
http://localhost:8080/test/database

Docker build using:

`mvn clean install jib:buildTar`

