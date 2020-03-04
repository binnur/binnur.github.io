---
layout: post
date: 2020-03-03 15:47:45
title: "Think Better, Learn Faster: Rapid Learning Cycles for Hardware"
categories: product-management readings
author_name : binnur
author_url : /author/binnur
author_avatar: binnur
show_avatar : true
read_time : 7
feature_image: feature-birds
show_related_posts: true
square_related: recommend-plant
---
> *“A complex system that works is invariably found to have evolved from a simple
> system that worked. A complex system designed from scratch never works and
> cannot be patched up to make it work. You have to start over with a working
> simple system.”* — John Gall

As you may have noticed from some of the projects I shared, I like to dabble with hardware. I feel there is a great opportunity to augment human experiences by delivering products that work at the intersection of hardware and software.

In the past few years, there has been an increased focus on building
customer-driven products with Lean Startup, Lean UX, Agile development, and
such. I don’t believe anyone would disagree if I stated *hardware is hard*.
However, hardware development has also shifted to reduce risk through 3D
printing, robotics for automation, small-batch manufacturing vendors.
Yet, the process of building products at the intersection of hardware and
software is still challenging, and the accelerated demand for compressing
product delivery to meet key market windows, i.e. market-driven
schedules, doesn’t help.


## Importance of Right Balance: Risk vs. Speed

If you already shipped a few products in different markets, you already know
that one cannot generalize the mantra of *“Move fast and break things”* -- we
cannot always assume all software projects lends itself to agile, rapid
development. New product development is context-dependent and impact analysis
can help identify where going slow will lead to faster results -- think
blockchain and smart contract development, users who are not technically savvy,
medical products where privacy and security are critical. Even Zuckerberg
revisited his mantra in 2014 with *“[Move fast with stable
infra](https://mashable.com/2014/04/30/facebooks-new-mantra-move-fast-with-stability/)”*
as Facebook customer base scaled and diversified.

![NPD Cycle]({{site.baseurl}}/img/assets/NPD-Cycle.png)

I outlined the above NPD Cycle diagram back in 2010, adding it here as it is time to revisit and revise. The new product development, regardless of software or hardware, is challenging — you can do everything right and still fail. The ultimate goal at every step is to ensure we are working on an idea and product that is **viable, feasible, and desirable**. In other words, developing great products is not enough to succeed, we need products that our customers love and agree that are great products.

The reasons behind the success or failure of new products haven’t changed since my research project in 2002, you can read my research highlights [here](https://binnur.github.io/field-research-project). Or, for more recent analysis, checkout CBInsight’s [Top 20 Reasons Startups Fail](https://www.cbinsights.com/research/startup-failure-reasons-top/). With that, let’s focus on what makes hardware development more challenging.


## Challenges with Hardware Development

For additional insights on hardware product development make sure to visit [Bolt’s](https://blog.bolt.io) [Illustrated Guide to Product Development (Part 1-4)](https://blog.bolt.io/ideation/).

![Product Development: Hardware]({{site.baseurl}}/img/assets/NPD-hardware.png)


*   Hardware products tend to require more people hours and coordination among diverse groups from industrial design to electronics, firmware development, certification, supply chain, manufacturing, distribution, retailers, ...
*   Product development requires coordination with outside players who have their own processes, priorities, and schedules.
*   Differences in hardware and software development translate into departmental organizational structures that require greater cross-functional coordination and collaboration.
*   The process of _deploying_ a hardware product is more involved due to the number of tasks and verifications that are required prior to mass production. Many of these tasks have long lead times and introduce schedule and cost risk if not executed properly.
*   Given the investment required due to material costs, risks are higher and mistakes early in the development cycle result in schedule delays and other unanticipated ripples.
*   For new products, the needed scale from the initial product to future updates is unknown, making it difficult to plan. As the company tends to focus on getting through the design and manufacturing process, the actual work of taking the product to the market/customer takes a back seat.


## Rapid Learning Cycles Framework by Katherine Radeka

With over 20 years of new product development experience, I have created and leveraged numerous product development processes from stage-gate to extreme programming (pre-Agile era), and discovery-driven planning for new initiatives. So, I was curious what else I can add to my toolbox when I stumbled upon Katherine Radeka’s book on [“The Shortest Distance Between You and Your New Product”](https://rapidlearningcycles.com), where she tackles the process of developing hardware products with agility.

As a framework, Rapid Learning Cycles does not lay out a specific hardware
development process. However, building on her expertise in developing physical
products, Radeka emphasizes that the key to ***building velocity is to make
decisions at the right time with higher confidence so that those decisions won’t
have to be revisited later***. This is critical as the cost of change increases
as we get closer to the final product.

So, how is The Rapid Learning Cycles framework different from other agile software and Lean Startup principles? For a quick overview check out the [Rapid Learning Cycles and Lean Product Development](http://www.leanfrontiers.com/wp-content/uploads/2016/10/Katherine-Radeka-LPD.pdf) slides from Radeka. As the terminology is different, here is [the mapping between Agile vs. Rapid Learning Cycles](https://s3.amazonaws.com/s3.edu20.com/files/715237/Agile-Roots-RLC-Tabloid.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=ASIAXGYUYJYUAINN6G5A%2F20200302%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20200302T002822Z&X-Amz-Expires=604800&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEEcaCXVzLWVhc3QtMSJGMEQCIAd%2FUS5g0mknQy%2BivOg58xT3G%2Fcv4HoT90wUfZuk7nhyAiBMfPxTijtzIf8XBXiwhUoAkeyYwqdNHunoF2w%2Fm2Vy7Sq0AwggEAAaDDQ5NTU3NTM4NzY4OCIMi9e2L7YCyWTJ4TO%2BKpEDZKwgiVbaOfbfMnypEBrqZU8zgbz8IiI3%2FFaIF90tVAGsBvf1r7EaSL23oZdZwToGXRPFIRC5A9CVJaSfN9vkeSdWB4N6hg9j4lJ%2FW09dnc6oKjbXoE8jruCxT6VlqGlsqciNAe1Pn%2BxgRcbuyOkL8agkgNIJEu1VVceDLlX0BRJG4heyY%2Bfh60dDMnLQ2ANKA23WlhEDkHsiLyXUVUL4%2B4TDPA7Jy2dOWYCGDEslK90KHZzJWwJv6sqsZmkULO%2B6ox838sMD8RCcdjhjosIq2hEI3vZXWLuIuY2BZZe4uoAM4YGj%2FNbQmU%2BbD3ST11oUWKRsn9gX8L73cDAmW4PxX0aUkSTF4Gbukl4Bg6MP1Hdnklt4%2Fp%2FsRU0e3zVlA%2FMcIS%2FatHMfdY%2BFVy8Vwr2B9%2FTYOzQmCM%2Fuf3L4Q06Lq9cXDtYNZjLt0tX%2FuBwLDI98vEwo%2Fd8K4LqGvnjtrv%2FcxCt356QoQELVjtPHQ4ip1%2FOGsbhsQDzOBRTUUNmZjAmr3pX%2BdaVSiPLqCxrYYKUeqmIwmvnw8gU67AHDJZQUHNTMsiqjVS%2BlduwDWnRnu75LrIGU8Rw2ALDLHnhMg50Ro0sNylLPsg1u3C7cTLJkLtRMVdwTzyq4pM%2F7hHyTM6E4V%2Bpu%2FtDedbDB7W3OZICSyTfkeNp6cV3oGeJ2%2FMXqTfbuF5y5qIanTWc%2FPe3rxyoDbuYEEIhnFNKacMKSZUvY0wrHMFE3FjwoC3wcfkbf9enrszuQ7cpFwTNEVgxeyg7ZZR6stCPmgDL0mqJtge2LBgwvBfCGWz86rscOG6fr5A9GAzNQhg5y4m6I5n0SA9oXir7Fo%2FA8m3uiZRgcJSc0lDlyyPhjUg%3D%3D&X-Amz-SignedHeaders=host&X-Amz-Signature=a9a943037699a7185767d3b9c0cc16c15a2037d069dab98e782aa6a8f750f8c8). Similar to Agile, Rapid Learning Cycles uses iterations and timeboxing to emphasize the continuous process of knowledge discovery and decision making while driving a sense of urgency.


### Explicit Process for Problem Discovery

As Rapid Learning Cycles is all about learning, the process starts with a kickoff meeting where the team establishes a shared Core Hypothesis that outlines what is _new, unique, and different_ about this product. The Core Hypothesis guides the learning process by identifying Knowledge Gaps, Key Decisions, when those decisions need to be made and who needs to be involved. This explicit identification of required stakeholders, partner participation, needed communication, and coordination helps increase the quality of decisions and accelerates learning.


### Why Learning Before Doing

The terminology used for Rapid Learning Cycles emphasizes learning and decision
making over doing. This is a critical difference from Agile where the work is
focused on completed, demonstrable part of the product. Key Decisions are like a
domino effect — they have an order and cascading impact. By focusing on
understanding the flow of decisions, their timing, and ownership, Rapid Learning
Cycles continuously reduce uncertainty and increase confidence in decisions.

Initially, this focus on learning vs. building felt like a semantic difference.
However, when I look at the design thinking process, I can see the potentials in
extending the divergence and convergence cycles.

![Design Thinking]({{site.baseurl}}/img/assets/design-thinking.png)


Aside from the typical prototyping phase with _works-like_ and _looks-like_ cycles, hardware products go through many different stages requiring different fabrication techniques with varied cost implications. Each decision impacts the downstream tools, processes, sourcing options, and eventually cost, schedule, and reliability of the final product. This focus on learning with recognition of downstream impacts helps identify rapid low-cost prototyping and manufacturing techniques to reduce uncertainty and increase confidence.


### Process Flexibility with Coordination

Hardware development requires coordination with outside players usually with their own process, priorities, and schedules. Through the utilization of Learning Cycles and Integration Events, Radeka outlines a flexible program management framework where the focus is on empowering the teams, enabling them to focus on the learning required. As a result, each team focuses on problems to solve and given space to solve them. Through the Integration Events, the silos are broken and teams mutually support one another towards successful mission accomplishment.


## Slow Down in Order to Speed Up

The complexity of all the parts and pieces of hardware development reminds us that it is difficult for any one person to have a complete view of the development, production line, and process. Proper execution with a focus on reducing uncertainty and increasing confidence is mandatory to minimize cost and ship on schedule.

In a nutshell, even though Radeka does not spell out the hardware development process, she is focused on providing a framework to ensure efficient and effective teamwork regardless of what the downstream process or product is. If you are working on a product with a high degree of uncertainty, make sure to review Katherine Radeka’s [Rapid Learning Cycles](https://rapidlearningcycles.com) framework.


## Resources
* [Rapid Learning Cycles and The Shortest Distance Between You and Your New
  Product](https://rapidlearningcycles.com) by Katherine Radeka
* [Rapid Learning Cycles and Lean Product
  Development](http://www.leanfrontiers.com/wp-content/uploads/2016/10/Katherine-Radeka-LPD.pdf)
  by Katherine Radeka
*   [Bolt Blog](https://blog.bolt.io)
*   [Why Do So Many Hardware Startups Fail?](https://www.cbinsights.com/research/report/hardware-startups-failure-success/) By [CBInsights](https://www.cbinsights.com/)
*   [The Scrum in Hardware Guide](https://www.scruminc.com/scrum-in-hardware-guide/) by Scrum Inc.




