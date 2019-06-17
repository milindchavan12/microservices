# Micro Services

The word **Micro** refers to the scope of Service Functionality and not the lines of code. 

And the word **Service** is independently deployable component in the *bounded context*.

Now a formal definition :

**Microservices** - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are

- Highly maintainable and testable
- Loosely coupled
- Independently deployable
- Organized around business capabilities.

## Service Registry:
A service registry is a phone book of services with their locations, letting clients look up services by their logical names. The first thing our microservices have to do is self registration. This means that they need to register the network location on startup, and lately deregister on shutdown. When making a request to a service, the client needs first to discover the location of a service instance by querying the registry. And then it can invoke the needed microservice. 

Famous service registries are Eureka, Zookeeper, or Consul
