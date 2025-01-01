# DataStructuresProject

# Shipping Line Management System

Main Idea: ships are assigned on a fixed route through multiple ports and call for shippment quotes(shippment orders), applications of graph, stack, queue and linked list

to deliver an order, the order information (quote): destination, origin and the shippment(abstract class).

the management system will be divided into subsystems for better design.

quote subsystem:

1- view quotes:
0- graphic view of quotes in table form.
2- add quotes:
3- remove quotes

vessel subsystem:

four types of vessels:

1- container ships
2- tanker ships
3- bulk carrier ships
4- ro-ro ships

operations:

1- view vessels:
0- graphic view of vessels, storage in table form.
a- add vessels.
b- remove vessels.

Logging subsystem (optional):

1- generate system admin command history and view in relational form with each command being tied to a point in time.
2- keep history of each client that used the quote subsystem and their respective quotes.
3- generate reports detailing each vessel's work related information.

Routes subsystem:

1- add routes.
2- view routes:
0- routes will be displayed in table form with ID as primary key and an adjacency list for storage.


a vessel with the right destination or a connecting port would flag quotes for shippment with the corresponding vessel name
 and expected time of shippment.

quotes would be stored in queue format to prioritize early quotes.

vessels will only flag as much as they can ship depending on their weight and shipment type.

searches on vessels would be done using DFS which utilizes stacks.

the vessels will be stored in one tree format regardless of vessel type or DWT for binary search time and to optimize space usage.

shippment flags, system information updates and route chartings will be logged.

how are routes charted?

all ports and their relations to other ports will be stored in a graph structure that would be "charted" to create a route.

actual routes are an euler cycle.

routes will be stored as circular linked list.
