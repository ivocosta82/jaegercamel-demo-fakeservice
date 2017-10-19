# jaegercamel-demo-fakeservice
This project is part of a Camel demo with Jaeger using microservices. This project is deployable to Openshift using S2I
See also jaegercamel-demo1 and jaegarcamel-demo2

This is a really simple service used just as a placeholder, adaptations can be made to mock a more specific functionality. As it is at this moment this service is only intended to be used to demonstrate traceability using opentracing

---
Exposed endpoint: POST http://0.0.0.0:8080/fakeservice


This application expects the following environment variables
+ JAEGER_SAMPLER_TYPE	 - const
+ JAEGER_SAMPLER_PARAM - 1
+ JAEGER_SAMPLER_MANAGER_HOST_PORT - [hostname]:5778
+ JAEGER_AGENT_HOST - [hostname]

In this application the service name is in the code and the variable is not required
