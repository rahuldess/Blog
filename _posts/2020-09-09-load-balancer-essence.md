---
layout: post
title: "Load Balancer (Essence)"
comments: true
description: "Load Balancer"
keywords: "loadbalancer"
author: RahulSambari
---

##### Load Balancer Definition:
In simple terms, Load balancing (LB) is defined as the methodical and efficient distribution of network or application traffic across multiple servers in a server farm.

##### ADC Definition:
An application delivery controller (ADC) uses various techniques to improve the performance of web applications.<br>

In the usual configuration, the ADC sits in front of a group of web and application servers and mediates requests and responses between them and their clients, effectively making the group look like a single virtual server to the end users.<br>

There is no standard definition of what an ADC does or how it does it, but the techniques used to enhance performance commonly include
- Load balancing 
- Caching
- Compression
- Offloading of SSL processing.


##### TidBits:
- Load balancers detect the health of back end resources and do not send traffic to servers that are not able to fulfill request.
- Load balancing is the most scalable methodology for handling the multitude of requests from modern multi-application, multi-device workflows.
- You can put LB's in either Hardware and Software based.
- There are three types of load balancers, L4, L7 and GSLB load balancers.
  - <u>Layer 4 (L4)</u> load balancers work at the transport level. That means they can make routing decisions based on the TCP or UDP ports that packets use along with their source and destination IP addresses. L4 load balancers perform Network Address Translation but do not inspect the actual contents of each packet.
  - <u>Layer 7 (L7)</u> load balancers act at the application level, the highest in the OSI model. They can evaluate a wider range of data than L4 counterparts, including HTTP headers and SSL session IDs, when deciding how to distribute requests across the server farm.
  - <u>Global server load balancing (GSLB)</u> can extend the capabilities of either type across multiple data centres so that large volumes of traffic can be efficiently distributed and so that there will be no degradation of service for the end user.

- Load balancing is more computationally intensive at L7 than L4, but it can also be more efficient at L7, due to the added context in understanding and processing client requests to servers.
- To promote greater consistency and keep up with ever-evolving user demand, server resources must be readily available and load balanced at Layers 4 and/or 7 of the Open Systems Interconnection (OSI) model.
- A load balancer, or the ADC that includes it, will follow an algorithm to determine how requests are distributed across the server farm. There are plenty of options in this regard, ranging from the very simple to the very complex algorithm such as 
	- Round Robin
	- Least Connection Method
	- Least Response Time Method
	- Least brand with Method etc …

##### Credits:
