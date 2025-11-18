# Service Discovery
Automatically finding services in a network without manually searching.  
Eg: Your phone detecting nearby Bluetooth devices, Wi-Fi networks

In mobile computing, this is harder because :-  
Devices move, Network keeps changing, Battery is limited, Connectivity is unstable  
So service discovery must be fast, energy-efficient, and automatic

---
### Classifications :-
1. **Directory-Based Service Discovery**  
There is 1 central server (directory) that stores all service information.  
**How it works ?**  
Services register with the directory  
Clients send a query to the directory  
Directory sends the service details

2. **Directory-Less (Peer-to-Peer) Service Discovery**  
There is no central server.  
Every device advertises its own services.  
**How it works ?**   
Devices broadcast their services  
Other devices listen and discover

3. **Hybrid Service Discovery**  
Combination of directory-based + peer-to-peer.

---

### Considerations:-
Service discovery for mobile devices must handle:
1. Mobility
2. Limited Resources
3. Dynamic Network
4. Interoperability
5. Security