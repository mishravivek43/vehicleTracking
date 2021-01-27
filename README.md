# vehicleTracking

There are Two Files =>
1 is the cloud Deployment and Architecture of the Project
Over here since there can be number of vehicles are present we are using Microservices to make it faster and cheaper to update location real time
The front End can be Written in Angular/React 
Where as the backend can be written in Nodejs Microservices (Lambda Functions)
Apart from that there will Two databases mainly for storage and search.
We are using MongoDb for Realtime Storage and Elastic Search to get faster search Results for any vehicles of group of vehicles in a state/country
We can use Amazone API Gateway for quiuing the requests or can use RabbitMQ for the same purpose or  both depend on the scaling and needs
Kubernetes is used to manage various servers and containers and for scaling.
We can use grafana kind of free tools for alerts and analytics.
From Vehicle after Registeration , We only need there vehicleId and Locations time to time basis. And a token every 24 hour once to validate the source.
Token Will be expired after 24 hours of continous navigation than user will have to authorise it.
The Vehicle will be marked paused if being stationary for more than 10 seconds
We can also add non-active hours for vehicles and state related rules to curb unnecessary api hits
A user with distinguished roles can perform various operations on database and analytics part.



