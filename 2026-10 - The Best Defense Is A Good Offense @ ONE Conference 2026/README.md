# The Best Defense Is A Good Offense: A Pragmatic Path to Continuous Purple Teaming

__Presented at ONE Conference 2026 in The Hague__

## Description
Attackers automate. With AI-native adversaries now using frontier models like Mythos or Astra to adapt tradecraft and scale operations at machine speed, the gap between attacker tempo and defender tempo is widening fast. Yet most organizations still validate their defenses once or twice a year and assume the results hold up. They rarely do: infrastructure changes, detection rules quietly break, and an attacker only needs to slightly vary their approach to get past controls that worked six months ago. Meanwhile, regulations like DORA and NIS2 increasingly expect you to demonstrate that your defenses actually work right now, not just that they were tested at some point in the past.

This talk makes the case for Continuous Purple Teaming (CPT): using automated, repeatable attack simulations to continuously answer the one question that matters: are our security controls protecting us against the threat that matters today?

CPT validates your controls in two directions. Bottom-up, simulations act as a regression test for your detection stack, verifying that what you could detect yesterday you can still detect today. Top-down, you simulate the threats most relevant to your organization and get an immediate, fact-based view of your coverage across frameworks like MITRE ATT&CK. Because every result combines the offensive view (how dangerous is this technique?) with the defensive view (did our controls block or detect it?), CPT also tells you which gaps to fix first, so your team spends its limited time where it counts.

Fixing those gaps is where most programs stall, and where CPT changes the game for your SOC and detection engineering teams. By isolating the exact attacker behavior behind each simulation and pairing every gap with targeted guidance, CPT turns findings into custom detection rules in a fraction of the usual time. The result is detections built on behavior rather than tools, protecting you not just against yesterday's known attacks but against the AI-equipped attacker of tomorrow.

## Outline
- Introduction and problem statement
  - Brief 'whoami'
  - Current security landscape and issues (talent shortage, increased need for rare specialist knowledge)
  - The next generation of the 'defenders dilemma': how to counteract scaling attackers and changing technologies
- The need for Continuous Purple Teaming (CPT)
  - Offensive engagements as well as purple teaming are often one-off or periodic manual effort
  - Clever automation is the key to address the changing technology and security landscapes, and no longer optional
    - Drivers in compliance frameworks such as DORA or NIS2
    - Analogy with software testing as a continuous process, why are detection rules not 'regression tested'?
- A pragmatic approach
  - Why repeatable simulations are at the core of CPT
  - Introducing the core feedback loop: "Simulate -> Measure -> Prioritize"
  - Why CPT is best positioned to prioritize remediation: it combines insights from offense (how impactful is a technique) and defense (which of our controls work against this technique in practice)
- Walking the pyramid
  - Recap of the 'pyramid of pain' for defenders, and introducing it for attackers
  - How focusing on advanced TTP simulation increases resilience by driving the development of mature detection rules
  - Concrete examples of attack simulations and corresponding detections at every level of the pyramid
  - Bad examples:
    - E.g. simulating the execution of `mimikatz.exe` to detect its file hash (brittle detection)
  - Good examples:
    - Simulating the 'critical path' of a TTP (e.g. the sequence API calls made by Mimikatz)
    - Simulating permutations of an advanced procedure like process injection ("modular BOF" approach)
  - The good examples serve as a demonstration of how quality simulations lead to the engineering of detection rules high up in the pyramid, which in turn leads to a resilience against changing procedure implementations
- Conclusion
  - Recap of key takeaways
  - How can attendees get started with a CPT program at their organization
