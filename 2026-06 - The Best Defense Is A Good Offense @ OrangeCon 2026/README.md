# The Best Defense Is A Good Offense: A Pragmatic Path to Continuous Purple Teaming

__Presented at OrangeCon 2026 in Amsterdam__


## Abstract
While attackers scale their operations through automation, many defenders remain trapped in a reactive, manual cycle of fire-fighting. To regain the advantage, we must evolve from periodic "point-in-time" assessments to a model of continuous assurance. This talk introduces Continuous Purple Teaming (CPT): a pragmatic approach to security testing that uses repeatable attack simulations as a regression test for your defenses.

We will explore the "Simulate, Measure, Prioritize" feedback loop and demonstrate how to apply the Pyramid of Pain in the context of attack simulations. By moving beyond brittle indicators and focusing on behavioral TTPs that are grounded in relevant threat intelligence, you can build detections that are resilient to changing tradecraft. Attendees will leave with concrete design patterns and a framework to start building a mature CPT capability in their own environment.

## Description
Manual security assessments provides great insights, but they are labour-intensive and the results are often short-lived. Once an exercise ends, it is difficult to know if those same defenses still hold up after a few months of infrastructure changes or when an attacker slightly tweaks their tradecraft. This talk focuses on turning these one-off exercises into a repeatable process, where automated attack simulations act as a constant regression test for your detection stack.

We will go through the mechanics of a mature CPT program using a feedback loop focused on automated simulation, measurement, and prioritization. A key part of this involves applying the Pyramid of Pain to offensive simulations: We will discuss why simulating the execution of a specific tool is often a dead end for defenders, and why focusing on the underlying procedure is much more effective. For example, we will look at how simulating the specific sequence of API calls used in process injection leads to detections that are far harder for an attacker to evade than a simple file hash or tool-based detection.

Finally, we will bring these concepts together into a pragmatic framework that continuously connects red and blue team efforts. We will discuss how to use simulation data to identify which defensive gaps are the most critical to fix first based on real-world implementation. This session will provide the design patterns and logic needed to start building a continuous purple teaming program in your own environment.