---
layout: post
title: "Microservices Key points"
date: 2019-08-19 19:30:20 +0530
description: From the Book "Building Microservices" Designing Fine-Grained Systems by Sam Newman.
img: # Add image post (optional)
tags: [Notes, Microservices] # add tag
---

# Microservices Key points
## Book : Building Microservices: Designing Fine-Grained Systems by Sam Newman
### Chapter 1
 *  Microservices should be small and focused on doing one thing well
 *  “Gather together those things that change for the
same reason, and separate those things that change for different reasons.”
 *  Microservices should be **Autonomous**. APIs should be good and decoupled.
 *  Key Benefits:
	* **Technology Heterogeneity** : User technology of your choice.
	* **Resilience**: If one component of a system fails, but that failure doesn't cascade, you can isolate the problem and the rest of the system can carry on working
	* **Scaling**
	* **Ease of deployment**
	* **Organizational Alignment**: Small team with small codebase is more productive than large teams with large codebase. 
	* **Composability**: Reuse of functionality.
	* **Optimizing for Replaceability**
	
### Chapter 2
 * **An Evolutionary Vision for the Architect:**
 	* The Architect should be just like a town planner just like the game SimCity. A town planner’s role is to look at a multitude of sources of information, and then attempt to optimize the layout of a city to best suit the needs of the citizens today, taking into account future use.
* **Zoning**:
	* From the metaphor of the architect as a town planner, zones are areas in the city which are build to do a certain type of job. For example industrian zone, residential zone. In the similar way, zoning in microservices are our service boundaries, or perhaps coarse-grained groups of services. As an architect we need to think more about what happens between the zones than inside the zone.
	* The guideline is to "be worried about what happens between the boxes, and be liberal in what happens inside."
* 
