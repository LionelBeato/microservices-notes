# Microservices Notes

Notes for the WIN program microservices quiz

## What are microservices? ## 

Microservices, or more specifically *microservices architecture*, is the arrangement of loosely coupled services that act as a singular application. An application structured with this architecture in mind will in fact be a collection of services. An individual service in this application may itself be referred to as a microservice. Microservices are inherently more agile due their high cohesion. A service that needs to only access one type of resource will be more agile than a service that is accessing many. 

It's important to note that this architectural design will enable more cross-team collaboration as services can be easily designed to interface with one another despite of implementation details. 

Microservices are framed in contrast to *monolithic* applications -- or simply *monoliths*.

## When should I utilize microservices? ##

The are many scenarios where one would prefer to design microservices for their applications. In the industry there is a concept of *fault tolerance* [defined as follows](https://www.imperva.com/learn/availability/fault-tolerance/)
:

> Fault tolerance refers to the ability of a system (computer, network, cloud cluster, etc.) to continue operating without interruption when one or more of its components fail.

So, whenever one needs a system that continues its operations despite of any singular component failure, one should consider utilizing microservices. 

Another scenario is one where there are many technology stacks associated with an application. System failure may be mitigated by utilizing microservices here as well. 

Finally, [we can fine tune authorization and authentication per microservice.](https://dzone.com/articles/authentication-and-authorization-in-microservices) Contrast this with traditional monoliths, where this is a potential for users to access resources they shouldn't. 

## What are the logistics of microservices? ##

Several factors need to be considered when deciding on the finer details of microservices. For example, microservices are designed to be scalable, so utilizing them with on-site data centers may not be ideal. It makes more sense to migrate your application to the cloud for expansive scalability. 

Microservices communications are routed between single-server systems, which may make network communication trickier. [Design patterns have emerged to tackle this problem.](https://dzone.com/articles/design-patterns-for-microservice-communication) Note that limiting a microservice's connectivity has the chance of improving security. 

It's important to identify your business functions in your applications so that they may be targeted for microservices creation. Follow the principle of ["smart endpoints but dump pipes."](https://medium.com/@nathankpeck/microservice-principles-smart-endpoints-and-dumb-pipes-5691d410700f)

A big logistical benefit from microservices is the fact that [it can be designed with *decentralized governance* in mind](https://www.wipro.com/en-US/blogs/dr-gopala-krishna-behara/microservices-governance/): 

>Microservices Governance is a methodology or approach to establish policies, standards, best practices and guidelines on the adoption of Microservices to enable enterprise agile IT environment.<br></br>
Microservices promote the polyglot model regarding technology stack for supported languages, tools, and data stores. Reusability of assets and tools is the main concept of Microservices, rather than centralized. A decentralized model is best suited for Microservices governance. Decentralized governance gives Microservices teams the freedom to develop software components using different stacks.

This reduces red tape and top-down decision making. Thus, teams can utilize their preferred tools and languages and retain more ownership over their services. This in turn increases the rate of deployment and versioning. 

## Anything else I should know ##

Be aware that *all stakeholders* should be involved in the management of APIs for microservices as explained by [Layer 7 Co-Founder and Chief Strategy Officer Dimitri Sirota](https://techcrunch.com/2012/11/11/5-rules-for-api-management/):

>It needs to address each constituency or user group engaged in building and running an API. These include API Architects / Developers, Security Architects, IT Operations and Business Analysts (API marketers). The Layer 7 platform has a product component that addresses each of these stakeholders (API Gateway, API Identity Broker, API Service Manager, API Developer Portal).

One major downside to microservices is [the increase of a system's attack surface.](https://www.securitymagazine.com/articles/89283-ways-to-reduce-your-attack-surface). There are many ways to mitigate this as detailed in the link provided.

When working with something like kubernetes, defining your security context will be the first step one should take when securing. [See this link for more information](https://unofficial-kubernetes.readthedocs.io/en/latest/concepts/policy/security-context/). As with everything related to containers and microservices security, *automation* is an essential underlying concept. 





