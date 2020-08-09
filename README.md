# Microservices Notes

Notes for the WIN program microservices quiz

## What are microservices? ## 

Microservices, or more specifically *microservices architecture*, is the arrangement of loosely coupled services that act as a singular application. An application structured with this architecture in mind will in fact be a collection of services. An individual service in this application may itself be referred to as a microservice.

It's important to note that this architectural design will enable more cross-team collaboration as services can be easily designed to interface with one another despite of implementation details. 

Microservices are framed in contrast to *monolithic* applications -- or simply *monoliths*.

## When should I utilize microservices? ##

The are many scenarios where one would prefer to design microservices for their applications. In the industry there is a concept of *fault tolerance* [defined as follows](https://www.imperva.com/learn/availability/fault-tolerance/)
:

> Fault tolerance refers to the ability of a system (computer, network, cloud cluster, etc.) to continue operating without interruption when one or more of its components fail.

So, whenever one needs a system that continues its operations despite of any singular component failure, one should consider utilizing microservices. 

Another scenario is one where there are many technology stacks associated with an application. System failure may be mitigated by utilizing microservices here as well. 

## What are the logistics of microservices? ##

Several factors need to be considered when deciding on the finer details of microservices. For example, microservices are designed to be scalable, so utilizing them with on-site data centers may not be ideal. It makes more sense to migrate your application to the cloud for expansive scalability. 

Microservices communications are routed between single-server systems, which may make network communication trickier. [Design patterns have emerged to tackle this problem.](https://dzone.com/articles/design-patterns-for-microservice-communication) 

