ELK with logtrail plugin 

Follow these steps:

1. create image with installer plugin
in **/elk/image/** run
`docker build -t elasticsearch-davidb .`
2. In **/elk/** run `docker-compose up`

3. you should see kibana web on localhost:5601


If you want to send some data in Kibana

1. configure **filebeat.yml** in **/elk/beats/etc/filebeat/**
    - mostly is local docker adress only needed
2. In **/elk/beats** run `docker-compose up`