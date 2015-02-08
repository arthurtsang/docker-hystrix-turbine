# docker-hystrix-turbine

## simple turbine docker image.

to build turbine-executable-{turbine-version}.jar check out https://github.com/Netflix/Turbine and run ./gradlew shadowJar.  the file is located under turbine-core/build/libs.

to run, set TURBINE_STREAMS to env, 

docker run -d -p 8080:8080 -e TURBINE_STREAMS="http://ip1/hystrix.stream http://ip2/hystrix.stream" arthurtsang/docker-hystrix-turbine

