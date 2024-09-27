# Event Driven Architecture

Event-driven architecture (EDA) is a software architecture pattern promoting the production, detection, consumption of, and reaction to events. An event can be defined as a significant change in state. 
An event-driven system typically consists of event emitters (or agents), event consumers (or sinks), and event channels.

Table of Contents
=================

   * [Components](#components)
      * [Event Emitters](#event-emitters)
      * [Event Consumers](#event-consumers)
      * [Event Channels](#event-channels)
   * [Advantages](#advantages)
   * [Disadvantages](#disadvantages)
   * [Use Cases](#use-cases)

## Components

### Event Emitters
Event emitters are the components that emit events. They can be a user, a system, or a sensor.

### Event Consumers
Event consumers are the components that consume events. They can be a system, a user, or a sensor.

### Event Channels
Event channels are the medium through which events are transmitted from emitters to consumers. They can be a message queue, a message broker, or a stream.

## Advantages

### Scalability
EDA allows for the decoupling of components, which makes it easier to scale individual components independently.

### Flexibility
EDA allows for the addition of new components without affecting existing components.

### Resilience
EDA allows for the isolation of components, which makes it easier to recover from failures.

### Real-time
EDA allows for the processing of events in real-time.

## Disadvantages

### Complexity
EDA can introduce complexity due to the asynchronous nature of events.

### Debugging
EDA can make debugging more difficult due to the asynchronous nature of events.

### Consistency
EDA can make it more difficult to maintain consistency across components.

## Use Cases

### Microservices
EDA is commonly used in microservices architectures to enable communication between services.

### IoT
EDA is commonly used in IoT applications to handle events from sensors.

### Real-time Analytics
EDA is commonly used in real-time analytics applications to process events in real-time.

## Examples

### Event Sourcing
Event sourcing is a design pattern that uses EDA to store the state of an application as a sequence of events.

### CQRS
Command Query Responsibility Segregation (CQRS) is a design pattern that uses EDA to separate the read and write operations of an application.

Sources:
- [Top Kafka Use Cases You Should Know - Byte Byte Go](https://www.youtube.com/watch?v=Ajz6dBp_EB4&ab_channel=ByteByteGo)
- [CQRS and Event Sourcing - Martin Fowler](https://martinfowler.com/bliki/CQRS.html)
- [MQTT - HiveMQ](https://www.hivemq.com/blog/how-to-get-started-with-mqtt/)