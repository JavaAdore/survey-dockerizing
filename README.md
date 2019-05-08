# survey-dockering
Just contains docker-compse.yml and .env file used to run survey microservices in docker container


# prerequisites
docker & docker-compose are properly installed on your machine

# Steps
clone 
<a href="https://github.com/JavaAdore/survey-rest-gateway">https://github.com/JavaAdore/survey-rest-gateway </a> <br/>
cd survey-rest-gateway <br/>
then build it by <br/>
mvn clean install docker:removeImage docker:build <br/>


# clone
<a href="https://github.com/JavaAdore/survey-eureka-server">https://github.com/JavaAdore/survey-eureka-server </a> <br/>
cd survey-eureka-server</br>
then build it by <br/>
mvn clean install docker:removeImage docker:build <br/>

# clone
<a href="https://github.com/JavaAdore/survey-definition-service">https://github.com/JavaAdore/survey-definition-service</a> <br/>
cd survey-definition-service <br/>
then build it by<br/>
mvn clean install docker:removeImage docker:build<br/>

# clone
<a href="https://github.com/JavaAdore/survey-surveyee-service">https://github.com/JavaAdore/survey-surveyee-service</a> <br/>
cd survey-surveyee-service</br>
then build it by<br/>
mvn clean install docker:removeImage docker:build<br/>

# clone
<a href="https://github.com/JavaAdore/survey-zipkin-server">https://github.com/JavaAdore/survey-zipkin-server </a> <br/>
cd survey-zipkin-server <br/>
then build it by<br/>
mvn clean install docker:removeImage docker:build<br/>



 

#after building all repositories above
configure ports in .env file <br/>

open terminal under root/Administrator user
type 
docker-compose up
enjoy !!
