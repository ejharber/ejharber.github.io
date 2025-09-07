---
title: "NeuroReality™: A Data Distribution Service-based Inter-Process Communication Middleware"
collection: publications
category: conferences
# permalink: /publication/2024-neuroreality-telepresence
excerpt: 'This paper introduces NeuroReality™, a DDS-based publish-subscribe middleware designed for distributed real-time systems in telepresence and teleoperation applications, offering low-latency, high reliability, and high throughput communication that outperforms traditional server-client architectures.'
date: 2024-11-16
venue: '2024 IEEE Conference on Telepresence'
paperurl: 'https://ieeexplore.ieee.org/document/10841742'
citation: 'S. Asjad, E. Harber, V. Santos, and D. Tyler. (2024). &quot;NeuroReality™: A Data Distribution Service-based Inter-Process Communication Middleware.&quot; <i>2024 IEEE Conference on Telepresence</i>. pp. 168-171.'
---
This work presents NeuroReality™, a novel Inter-Process Communication (IPC) middleware that leverages the Data Distribution Service (DDS) standard to enable robust, reliable, and fast communication for distributed real-time systems used in telepresence and teleoperation applications.

**Key Technical Contributions:**
- **DDS-based Architecture**: Replaces traditional server-client models with a publish-subscribe paradigm, eliminating single points of failure and improving scalability
- **Cross-Platform Integration**: Seamlessly integrates with ROS2 and other DDS-based frameworks, addressing IPC challenges across different operating systems and sub-processes
- **Quality of Service Control**: Leverages DDS QoS configurations to prioritize critical data streams like haptic feedback signals
- **UDPv6 Multicast Transport**: Utilizes UDPv6 multicast for efficient high-throughput, low-latency data delivery to multiple subscribers

**Performance Achievements:**
- **Local Communication**: Achieved 5.72 ms average latency at 1 kHz data rates over wireless networks
- **Long-Distance Performance**: Maintained 45.38 ms average latency for 3800km communication (Cleveland to Los Angeles)
- **Scalability**: Demonstrated superior performance compared to server-client architectures when scaling from 1 to 15 concurrent ROS2 topics
- **Video Transmission**: Successfully transmitted 1080x720 video at 30 FPS with lower latency than commercial solutions like Zoom

**System Architecture:**
The middleware features automatic node discovery through join codes and certificate exchange, dynamic data transfer with packet prioritization based on network bandwidth and data importance, and robust error handling with acknowledgment-based retransmission. The system breaks serialized data into numbered packets and adaptively manages transmission based on network conditions and data priority.

**Real-World Validation:**
Extensive testing demonstrated NeuroReality's effectiveness in both local (wireless university network) and intercontinental scenarios. The system maintained stable communication where traditional server-client architectures failed, particularly for high-frequency data transmission over long distances. Video streaming tests showed qualitatively better performance than established commercial platforms.

This middleware addresses critical challenges in modern robotic applications, particularly for remotely operated multi-robot systems and telepresence applications requiring synchronized real-time performance. The work represents a significant advancement in enabling scalable, reliable communication infrastructure for next-generation teleoperation systems.