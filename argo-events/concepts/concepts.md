Argo events has 4 main components: event source, sensor, eventbus and trigger.

An eventsource is configurations to consume events from external sources. It transforms the events into the cloudevents and dispatches them to eventbus.  
Sensor defines event dependencies(input) and triggers(output). It listens to events on the eventbus and execute triggers.  
Eventbus acts as a transport layer by connection eventsources to sensors. Eventsources publish the event and sensors subscribe to the events to trigger workloads.  
A trigger is a resource/workload that is executed by sensor when event dependencies are resolved.    
<img src='./argo-events-architecture.png' width=750px height=250px>