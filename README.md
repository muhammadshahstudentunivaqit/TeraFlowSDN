# TeraFlowSDN (Multi-Area SDN)

This repository documents my hands-on work with TeraFlowSDN in a multi-area network environment. The goal was to understand how a modern SDN controller can manage and orchestrate a distributed network using container based infrastructure.

This work was carried out as part of my learning and experimentation in Software Defined Networking (SDN), focusing on practical deployment.



## Implemention
- Built a multi-router topology using Containerlab
- Configured IP addressing and routing paths
- Enabled IP forwarding across all nodes
- Connected hosts and verified basic connectivity
- Deployed the TeraFlowSDN controller container
- Attempted integration between controller and network topology


## Topology
<img width="4444" height="2489" alt="ASDN LLD" src="https://github.com/user-attachments/assets/0215b0cc-6089-40aa-8f4c-6f6a59a2d622" />

## Network Architecture

The setup consists of:

- Centralized SDN controller (TeraFlowSDN)
- Multiple routers (FRRouting containers)
- Area Border Routers (ABRs) connecting different areas
- End hosts connected to edge routers
- Container-based topology using Containerlab




## Technologies Used
- Containerlab
- FRRouting (FRR)
- Docker
- Linux Networking (IP routing, sysctl)
- TeraFlowSDN Controller



## Challenges Faced
During implementation, I encountered several issues:

- Missing protobuf modules (`context_pb2`, `acl_pb2`)
- Controller failed to start due to dependency issues
- Official TeraFlowSDN repository becoming unavailable
- Dependency issues inside Docker container

Although the issues prevented full controller operation but it provided valuable debugging experience/learning.



## What I Learned
- Understanding of SDN architecture(Control plane vs Data plane)
- Hands-on experience with container-based network emulation
- Importance of dependency



## Conclusion
Although the full TeraFlowSDN setup could not be completed due to repository and dependency issues, this work provided a strong foundation in SDN concepts and practical deployment challenges.
