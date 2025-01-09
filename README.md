# RabbitMQ_microservices

#Saga design pattern

Transaction, ACID

Types of saga patterbm
#Chorography
#Orchestration

Inter communication between services
-synchronous - RestTemplate, Feigh client- directly make the API calls
-asynchronous - message broker - RabbitMq, Kafka etc


1)Create a docker container to access rabbitmq srvices
> docker run -d --hostname myrabbit --name myrabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management

>docker ps


http://loclahost:15672
username: guest
password: guest


types of exchanges

Direct
Topic
Fanout
==================================================================================================================

Practical


RabbitMq

Start docker desktop and give below command
docker run -d --hostname myrabbit --name myrabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management

Check if its running
docker ps

After checking, go to loclahost:15672 and see the rabbitmq dashboard

1)Producer

Create project with Spring Web,RabbitMQ dependency and other dependencies(which you need)
Create MQConfig file for cinfiguration
Create DTO and Messagecontroller

2)Consumer


Create project with Spring Web,RabbitMQ dependency and other dependencies(which you need)
Create MQConfig file for configuration, use @Configuration
Create DTO and MessageListener


Trigger API and test


Git : 

===========================================================================================================================

RabbitMQ dashboard: ![image](https://github.com/user-attachments/assets/7344fff0-d929-4535-9953-e7a74e23fb4a)
Messages: ![image](https://github.com/user-attachments/assets/9ab058a5-0a98-4991-9ce0-705ef5b82fc0)


Testing : ![image](https://github.com/user-attachments/assets/3fa5bc7a-0b93-4fae-984b-10d8ddf1cac2)

