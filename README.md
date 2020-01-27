# Ambulance Distribution Allocation Algorithms and Emergency Response Simulation (CS166 Final Project)

We need to optimize the placement of ambulances in a city to respond to emergency calls as quickly as possible. In a serious emergency, a person's chance of survival depends strongly on how fast an ambulance can reach them.

We use a network to represent neighborhoods/areas in a city. Each node represents a neighborhood and each the approximate average travel time between two adjoining neighborhoods.

Some of the neighborhoods have an ambulance station, where ambulances are parked, while others do not. An emergency call can come from any of the neighborhoods but different neighborhoods have different rates at which emergencies occur – some neighborhoods are higher risk than others.
When an ambulance goes out for a call, it has to complete the call by moving from its depot to the relevant neighborhood and then back to the depot. Only after returning to the depot can it go out on another call. The time it takes an ambulance to get to the call is the sum of the shortest path edge weights from the depot center to the call center plus a random value. The random value represents the time it takes to get to the precise location of the emergency and to assist the person there.

In this project, I explored the effects of using the **naive dispatch strategy**, in which we evenly distribute the ambulances
across despots, and the **strategy that uses the k-medoids algorithm**. 
