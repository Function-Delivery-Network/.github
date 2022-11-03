## Function Delivery Network

### Motivation for FDN
Serverless computing despite having many advantages, usage of serverless computing across the edge-cloud continuum suffers from the following pain points:
- Public cloud serverless compute platforms are limited to homogenous nodes
- No support for seamless deployment of the FaaS functions across the edge-cloud continuum
- Absence of serverless computing over multi-cloud and hybrid-cloud
- Myriad of serverless compute platforms and their monitoring platforms
- Serverless compute platforms do not account for the data access behavior of functions
- Absence of user-workload requests orchestration across multiple serverless compute platforms


### Introduction to FDN

The aspects mentioned above highlight some factors that make it difficult for users to adopt serverless computing for the edge-cloud continuum.

To this end, we develop an extension to the concept of Function-as-a-Service (FaaS) as a programming interface for serverless computing across the
edge-cloud continuum. This extension is a network of distributed heterogeneous serverless compute clusters spread across the edge-cloud continuum 
called **Function Delivery Network (FDN)** analogous to Content Delivery Networks. A serverless compute cluster consists of a serverless compute platform on top
of compute nodes deployed in a specific region, either at the edge, in the Cloud, or on-premise. 
- FDN provides seamless integration across the edge-cloud continuum by allowing the user to deploy and invoke the functions across heterogeneous serverless compute clusters in the continuum. 
- FDN also distributes the data required by the functions across the edge-cloud continuum by allowing the users to organize their data objects into storage buckets.

Based on these, FDN provides **Function-Delivery-as-a-Service (FDaaS)**, which can deliver user workload functions invocations to a subset of serverless compute clusters spread across the
continuum based on :
1) function-awareness 
2) data-awareness. 
The invocations are then load balanced across the selected subset of clusters based on the set load balancing algorithm. The automatic management of 
resources in the proposed serverless-based FDN facilitates application development by shifting the burden to the cloud platform.

### FDN Architecture
