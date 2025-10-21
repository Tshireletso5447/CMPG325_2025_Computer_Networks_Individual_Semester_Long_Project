# CMPG325_2025_Computer_Networks_Individual_Semester_Long_Project

## Bus Topology Implementation

**File:** `bus-topology.pkt`

**Design Approach:**
- Used Hub-PT to simulate traditional coaxial bus topology
- Implements single collision domain and shared medium
- Demonstrates broadcast traffic behavior

**Devices:**
- 1 × Hub-PT
- 4 × PC-PT (PC-Bus1, PC-Bus2, PC-Bus3, PC-Bus4)

**IP Configuration:**
- PC-Bus1: 192.168.10.10/24, 2001:DB8:ACAD:10::10/64
- PC-Bus2: 192.168.10.11/24, 2001:DB8:ACAD:10::11/64
- PC-Bus3: 192.168.10.12/24, 2001:DB8:ACAD:10::12/64
- PC-Bus4: 192.168.10.13/24, 2001:DB8:ACAD:10::13/64

**Testing Results:**
- ✅ Successful IPv4 communication between all devices
- ✅ Successful IPv6 communication between all devices
- ✅ Broadcast domain verified through simulation
- ✅ Single collision domain confirmed

**Evidence:**
<img width="1290" height="546" alt="Screenshot 2025-10-20 113013" src="https://github.com/user-attachments/assets/c707564b-daff-42cb-9577-655a8c4a318a" />

## Mesh Topology Implementation

**File:** `mesh-topology.pkt`

**Design Approach:**
- Switch-based full mesh topology implementation
- 6 inter-switch connections (n(n-1)/2 formula verified)
- Demonstrates redundancy and multiple communication paths

**Devices:**
- 4 × Switch 2960 (SW-Mesh1, SW-Mesh2, SW-Mesh3, SW-Mesh4)
- 4 × PC-PT (PC-Mesh1, PC-Mesh2, PC-Mesh3, PC-Mesh4)

**IP Configuration:**
- PC-Mesh1: 192.168.20.10/24, 2001:DB8:ACAD:20::10/64
- PC-Mesh2: 192.168.20.11/24, 2001:DB8:ACAD:20::11/64
- PC-Mesh3: 192.168.20.12/24, 2001:DB8:ACAD:20::12/64
- PC-Mesh4: 192.168.20.13/24, 2001:DB8:ACAD:20::13/64

**Mathematical Verification:**
- Nodes (n): 4
- Connections: n(n-1)/2 = 4×3/2 = 6 ✓

**Testing Results:**
- ✅ Full IPv4 connectivity between all device pairs
- ✅ Full IPv6 connectivity between all device pairs
- ✅ Redundancy verified - network functional with any single link failure
- ✅ Multiple communication paths confirmed

**Evidence:**
<img width="1290" height="546" alt="Screenshot 2025-10-20 113013" src="https://github.com/user-attachments/assets/a98ff444-e346-4ccd-b832-6629f1a2cda2" />
