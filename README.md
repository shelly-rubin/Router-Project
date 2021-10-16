# Router-Project
Implementations of an 8-bit simplified route

Logisim - The router is a gate-level circuit design that is used to facilitate the routing data packets from their source to their respective destinations, by creating and maintaining an address-port routing table.

The router receives a packet that consists of data and the address that the packet must be delivered to. The router then looks up the output port corresponding to the destination address, stored in a table as described below. If an entry exists for the destination address in the routing table, the router forwards the packet to the required port. If such an entry does not exist, the router routes the data packet to a default port (port 00 in this implementation).

If Setup mode is on, the Routing Table is filled in. There are 4 ports (2-bits are required to describe them). By the end of the Setup Phase, the Routing Table is ready and would now be used in order to direct any data or message to its corresponding port (or to the default port, if the destination for the input message is not defined in the table).

Active Phase: in that phase, any input address is now searched for in the Routing Table, and the output would be the port relevant for that specific address, as described above.

Logisim files - 8_bit_router.circ is the Logisim file. In addition, there are .png files(images of the circuit's modules in the project) encoder1.png, encoder2.png, encoder3.png, addresses.png, ports.png, compare.png, and router.png.
