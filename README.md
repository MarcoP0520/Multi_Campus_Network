                                                Multi-Campus Network Simulation – Cisco Packet Tracer
                                                
Tools: Cisco Packet Tracer, Static Routing, DHCP, Subnetting
Tech: Layer 3 Routing, Layer 2 Switching, DHCP IP Addressing, Gateway Configuration

Designed and implemented a multi-campus network architecture simulating three distinct networks: CSUEB, SJSU, and an IT Department hub. Each campus operates independently with internal DHCP services and does not allow direct communication between CSUEB and SJSU, ensuring logical separation and security.

Key Features:

  Three network zones: CSUEB, SJSU, and IT Department.

  DHCP pools configured per router to dynamically assign IP addresses within each subnet.

  Static routing enabled at core routers to allow:

  CSUEB ↔ IT Department communication

  SJSU ↔ IT Department communication

  X CSUEB ↛ SJSU (communication explicitly restricted)

  Public IP simulation using 211.x.x.x subnet for IT department to simulate WAN/internet edge.

  Used Class A and Private IP address ranges across all segments with realistic hierarchical topology and proper gateway routing.

Outcomes:

  Demonstrated understanding of inter-network communication, static routing, and logical segmentation.

  Applied subnetting, routing logic, and gateway configuration to enforce controlled access and isolation.

  Validated the design by testing end-to-end connectivity between departments and ensuring isolation policies were enforced.
  
...................................![image](https://github.com/user-attachments/assets/a51d3f49-c17c-4c8f-930c-6d671d806f8c)

🖥️ Device-to-Device Communication Table

Host	CSUEB_PC1	CSUEB_PC2	SJSU_PC1	SJSU_PC2	IT_PC1	IT_PC2
CSUEB_PC1	—	✅	❌	❌	✅	✅
CSUEB_PC2		—	❌	❌	✅	✅
SJSU_PC1			—	✅	✅	✅
SJSU_PC2				—	✅	✅
IT_PC1					—	✅
IT_PC2						—




CSUEB-RTR Routing Table...

..................................![image](https://github.com/user-attachments/assets/6f907d6a-db82-48dd-891a-70270472ba78)


CSUEB-BDR-RTR DHCP pool Example...

...................................![image](https://github.com/user-attachments/assets/e27e2d6f-1269-45bb-b831-59a8c3655f6c)





