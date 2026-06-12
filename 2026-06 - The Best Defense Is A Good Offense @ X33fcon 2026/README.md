# The Best Defense Is A Good Offense: A Pragmatic Path to Continuous Purple Teaming

__Presented at X33fcon 2026 in Gdynia, Poland__


## Description
Attackers are scaling their operations faster than ever, leaving many defenders stuck in a reactive and fire‑fighting posture. Automation on the defensive side is now required to move from one‑off tests to continuous assurance of your controls. This talk introduces "Continuous Purple Teaming" as a way to evolve from periodic manual exercises to a repeatable process that exposes real defensive gaps and verifies that fixes actually work.

During the talk, we will go over the various elements of a mature continuous purple teaming program: We will explore how realistic and repeatable attack simulations are at the foundation of continuous purple teaming, and we will introduce a "Simulate, Measure, Prioritize" feedback loop to discuss how to focus efforts on the defensive gaps that matter most. We will also show how attack simulations can act as a "regression test" for defenses, alerting on gaps as they emerge rather than months later during the next manual red team exercise.

We will use the "Pyramid of Pain" as a guiding framework and discuss how it applies not just to detection engineering but also to attack simulation. By focusing on advanced simulations, detections are pushed beyond simple indicators towards behaviors and techniques, making them harder for attackers to evade and easier to maintain across tooling changes or subtle tradecraft variations. The talk will address practical challenges in simulating complex techniques (how does one _really_ simulate "process injection"?) and provide concrete patterns to overcome them.

Finally, we will show how to bring repeatable attack simulations (red) and defensive efforts (blue) together into a pragmatic framework that attendees can take home. You will leave with concrete examples, design patterns, and starting points for building a continuous purple teaming program in your own environment.