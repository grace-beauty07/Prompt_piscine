# Goal: Practice the "right way" to use AI for learning on a technical topic (wireless routing protocols) — attempt first, then use AI to probe and deepen. 
## Topic: Wireless Routing Protocols

---

# Phase 1: Building My Foundation (Before Using AI)

## 1. Active Reading and Concept Summary

After studying wireless routing protocols in Mobile Ad Hoc Networks (MANETs), I identified three major categories:

- Proactive routing protocols
- Reactive routing protocols
- Hybrid routing protocols

These categories differ based on how routing information is maintained and when routes are discovered.

---

## Proactive Routing Protocols

Example: Optimized Link State Routing (OLSR)

Proactive protocols maintain up-to-date routing tables for all nodes at all times. Nodes periodically exchange topology information regardless of whether data transmission is occurring.

Characteristics:
- Immediate route availability
- Periodic control message exchange
- Higher constant overhead

Advantages:
- Low latency when sending packets
- Suitable for relatively stable networks

Disadvantages:
- Continuous bandwidth usage
- Increased energy consumption
- Scalability challenges in large networks

---

## Reactive Routing Protocols

Example: Ad hoc On-Demand Distance Vector (AODV)

Reactive protocols establish routes only when a node needs to transmit data. Route discovery is initiated through broadcast requests.

Characteristics:
- Routes created on demand
- Reduced idle overhead
- Initial delay during route discovery

Advantages:
- Efficient in highly dynamic networks
- Lower control traffic when idle

Disadvantages:
- Flooding may cause congestion
- Higher latency during route discovery
- Performance degradation as network grows

---

## Hybrid Routing Protocols

Example: Zone Routing Protocol (ZRP)

Hybrid protocols combine proactive routing within a local zone and reactive routing outside that zone.

Characteristics:
- Maintains local routing information
- Uses on-demand discovery for distant nodes
- Attempts to balance delay and overhead

Advantages:
- Reduced flooding
- Improved scalability compared to pure reactive
- Better performance balance

Disadvantages:
- Increased configuration complexity
- Zone radius selection affects performance

---

# 2. Small Network Scenario (Independent Design)

## Scenario Description

I designed a small wireless network with:

- 8–10 mobile devices
- Moderate movement
- Occasional data transmission (messages and small file transfers)
- No fixed central router

## Protocol Selection

I selected AODV for this scenario.

## Justification

- The network topology changes due to mobility.
- Devices do not communicate continuously.
- Maintaining full routing tables would waste bandwidth.
- On-demand routing reduces unnecessary overhead.

If the devices were mostly static and required constant communication, I would prefer OLSR instead.

---

# Phase 2: Strategic AI Use

After completing my independent analysis, I asked AI the following:

"In a 10-node MANET using AODV, what performance issues appear as the network scales to 20 or 30 nodes?"

## AI Insights

AI highlighted:

- Increased broadcast overhead during route discovery
- Higher probability of packet collision
- Increased routing table size
- Greater energy consumption
- Latency growth under congestion

## What AI Added to My Understanding

Before consulting AI, I focused mainly on functional behavior.

AI helped me consider:

- Scalability limits
- Network congestion effects
- Energy efficiency trade-offs
- Performance under high load

AI did not introduce new protocol types but expanded my thinking about second-order effects.

---

# Edge Case Exploration

I asked:

"What security risks exist in reactive routing protocols like AODV?"

AI mentioned:

- Blackhole attacks
- Wormhole attacks
- Packet dropping by malicious nodes
- Route manipulation

This made me realize routing protocol design must also consider trust, authentication, and secure routing extensions.

---

# Phase 3: Real Application – Smart City Network Design

## Scenario

A smart-city wireless network consisting of:

- 1,000 IoT environmental sensors (static)
- 50 traffic light controllers (semi-static)
- 10 emergency response vehicles (high mobility)

---

## Network Design Decisions

### 1. IoT Sensors → Proactive Routing (OLSR)

Reasoning:
- Mostly static placement
- Periodic reporting
- Low delay preferred
- Predictable topology

---

### 2. Emergency Vehicles → Reactive Routing (AODV)

Reasoning:
- High mobility
- Frequent topology changes
- On-demand discovery minimizes unnecessary updates

---

### 3. Traffic Lights → Hybrid Routing (ZRP)

Reasoning:
- Local communication within intersections
- Occasional long-distance coordination
- Balanced overhead and latency

---

# Potential Failure Points

- Broadcast storm during route discovery
- Network congestion during emergencies
- Energy depletion in battery-powered sensors
- Security vulnerabilities
- Network partitioning in case of node failure

---

# Refinement After AI Feedback

AI suggested:

- Clustering architecture
- Hierarchical routing
- QoS prioritization for emergency traffic
- Secure routing extensions
- Authentication mechanisms

## Refined Design

- Divide the city into routing zones.
- Use cluster heads for sensor data aggregation.
- Prioritize emergency vehicle traffic.
- Implement lightweight authentication protocols.
- Monitor network congestion dynamically.

---

# Reflection

## Human vs AI Contribution

Human reasoning: approximately 70–80%  
AI contribution: approximately 20–30%

I made protocol selections and architectural decisions independently.  
AI helped me evaluate scalability, security, and robustness.

---

## Could I Defend This Without AI?

Yes, because I understand:

- Trade-offs between proactive and reactive routing
- Impact of mobility on topology
- Scalability limitations
- Security risks in MANET environments
- Design considerations for real-world deployment

---

## Long-Term Retention

Key insights I expect to remember:

- No routing protocol is universally optimal.
- Trade-offs determine suitability.
- Scalability and security are as important as functionality.
- AI is most effective after independent reasoning.

---

## Final Thought

Using AI after building my own understanding strengthened my reasoning.  
It amplified my learning rather than replacing it.
