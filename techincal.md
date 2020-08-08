

### Introduction 
After reviewing the MockBank project for scaling issues, I have come to the conclusion that we have to move from Monolithic Architecture to Service Oriented Architecture. In this report, I will share the basic information about this architecture and how we can apply that to our project. 

### Service-Oriented Architecture 

According to Wikipedia, 

>Service-oriented architecture (SOA) is a style of software design where services are provided to the other components by application components, through a communication protocol over a network. 

This means we have to break down our entire application into different components called services. These components will interact with each other using a standard communication protocol. 

For example, our project can be divided into the following services. 

#### 1. Log In/Sign-Up 
We can create an independent service for user Login and SignUp Management. It will be similar to Facebook or Google login service. 

#### 2. Payments
Payment management can be an independent service which will be similar to PayPal etc. 

#### 3. Course Management
This service will take care of course addition and deletion. 

### Principles of SOA 

While creating these services, we have to take care of these principles -

#### Abstraction: 
They should follow this OOPs concept where we don't have to worry about the internal logic of this service. We will only worry about what this service does. For example, We just have to know what Payment service does but not worry about internal logic. 

#### Standardized service contract: 
There should be a standard way to talk to each service. 

#### Loose coupling: 
These services should be independent entities with the least amount of dependencies on other services. 

#### Reusability: 
We have to design these services in such a way that we can reuse them again and again without any issue. 

#### Autonomy: 
The service provider who is the owner of the service should have complete power over the logic of the service. For service consumers, they should not have to worry about it. 

#### Discoverability: 

Every service needs to have a great 
description document which can help it be easily discovered. 

## Advantages
Once we have broken down our project into different services, we can easily integrate them over a standard communication protocol. This approach will help us in scaling our project without much difficulty. 

## References


[https://www.geeksforgeeks.org/service-oriented-architecture/](https://www.geeksforgeeks.org/service-oriented-architecture/).