---
title: "With Great Responsibilities Come Great Rights (and Guardrails)"
date: 2025-03-20T17:40:51+05:30
draft: false
---
Spiderman said, "***with great power comes great responsibility***" I would say "***with great responsibilities come great rights***"

*And i have seen far too many engineers, team leads, managers, middle management fail because they weren't empowered/enabled to make the decisions for the responsibilities assigned to them. Here is my attempt to provide some thoughts on how do you make it work (what has worked for me)* 

In a social construct we always talk about rights and responsibilities. 

*For example :* you have the right to expect clean roads, but that also means you have to act responsibly as to not litter yourself. 
The municipality on the other hand is responsibile to maintain cleanliness of those roads, but for that, they must have the right to allocate funds, enforce laws, and deploy sanitation workers. 

So, it goes to say that in order for you to carry out your responsibility you need a set of expectations and also the rights to carry out tasks related to it. 

Imagine the situation where the right of a citizen to expect clean roads but the personnel / department responsible for cleanliness do not have the right to buy equipment that can do that.

Hence, if someone is assigned a responsibility, they should also be given the rights and authority to carry it out effectively. Otherwise, they are accountable for something they don’t have the power to influence. 

However, granting rights without reasonable guardrails can lead to unintended consequences.

Lets talk about this in the context of an IT org. Hopefully at the end of it i would have helped my fellow engineers to delegate effectively. 

## The Responsibility Framework: Expectations + Rights

Every responsibility delegated has to HAS TO consist of two key elements:

- **Expectations** – What needs to be achieved, success criteria, and constraints. What is my expectation out of this task when i have delegated it to you. 

- **Rights** – The authority, resources, and decision-making power needed to fulfill the responsibility.
What rights do you have in order to be successful in carrying out this responsibility. 

Without expectations, the person might not know what success looks like. Without rights, they won’t have the tools to make it happen. Both must be clearly defined.


## What is a responsibility anyways? Distinguishing Between Tasks and Responsibilities

A common pitfall in leadership is confusing tasks with responsibilities.

| **Factor**        | **Task**                          | **Responsibility**                   |
|-------------------|---------------------------------|-------------------------------------|
| **Definition**    | A specific action to be completed, the person delegating it has already defined it. | A broader ownership of an outcome where there might be ambiguity involved. |
| **Scope**        | Narrow, and is well-defined             | Broad, involves multiple tasks     |
| **Decision-making** | Little to no autonomy           | Requires judgment and discretion  |
| **Ownership**    | Assigned and completed          | Ongoing accountability. Its your baby until he/she moves out of the house ;)           |
| **Timeframe**    | Short-term, adhoc                       | Continuous or long-term            |
| **Example**      | "Send the report by Friday"     | "Can you ensure that we send a weekly report for all the functions every Friday going forward." |

### Example in a Social Context
- **Task:** "Picking up litter from the park/road."  
- **Responsibility:** "Ensuring the park/road remains clean" This would mean, implementing a waste management system, enforcing fines for people who litter, installation of dustbins at different points, etc etc."  

### Example in an IT Company
- **Task:** "Can you set up monitoring alerts in Datadog for this application."  
- **Responsibility:** "Can you ensure system reliability of these suite of applications?"  

When assigning work, it should typically be to ensure that responsibilities are handed off or delegated and, not just a series of tasks. If a person is accountable for an outcome, they need the ability to decide how to achieve it.

## Applying the Framework in an IT firm

Imagine a Director of Engineering assigning a responsibility to a Staff Engineer or an Architect:

**Responsibility:** Own the architecture and execution of a new product feature or system.

### Expectations (What needs to be achieved?)
- Ensure the system is scalable, secure, and maintainable (*you can define what scalable means, how secure is secure, what is the meaning of being maintainable really?*).
- Adhere to best practices in the current context of cloud architecture and DevOps.
- Collaborate with developers, SREs, and product teams to align system design with business needs.
- Ensure the delivery timeline is met without compromising on quality.
- Provide regular progress updates and architecture reviews.

### Rights (What authority & resources do they have?)
- Authority to make architectural decisions within defined constraints (*with reasonable understanding of constraints, budget and way forward*).
- Access Required cloud resources, CI/CD tools, observability platforms.
- Decision-making power Choose frameworks, libraries, and tech stack for implementation.
- Collaboration Ability to request input from DevOps, Security, and SRE teams.
- Implementation Authority: Can propose refactoring or system optimizations.

Please know that these aren't blanket rights without any guardrails. 


## Setting Guardrails for Rights

While responsibilities require autonomy, there must be limits to decision-making power to avoid unintended consequences. *The last thing you would need is to spend a 100,000 dollars on a decision that was made by the engineer(s) because they have the right to decide on the tooling* :smile: 

### Define Scope of Architectural Decisions Without Approval
**Example:** "You can select cloud-native components (e.g., Kubernetes, serverless) but cannot introduce an entirely new cloud provider without leadership approval."  
**Why?** Ensures flexibility while preventing tech sprawl.

### Restrict Changes That Affect Long-Term Costs
**Example:** "You can optimize infrastructure and reduce costs, but migrating databases or adopting a new third-party service requires financial review."  
**Why?** Prevents unplanned financial commitments while allowing optimization.

### Specify when should you escalate
**Example:** "You can propose changes to system architecture, but deprecating a core service or making a fundamental shift in design requires approval from the Director of Engineering."  
**Why?** Maintains alignment with long-term business strategy.

### Set Decision-Making Boundaries
**Example:** "You can change service-to-service communication patterns but need to discuss with the team before altering API contracts."  
**Why?** Encourages ownership while ensuring smooth cross-team collaboration.

These guardrails ensure autonomy and enables decision making at the -1 level without causing heartburn or preventing unintended consequences.

How this helps:

1. **Empowers peers** – Enabling folks to make decisions without waiting for approvals at every step and also giving them a sense of purpose / satisfaction of being able to execute it well (*if done so*).  
1. **Improved accountability** – Improves on accountability since success criteria is clearly defined.  
1. **Improves efficiency** – Enablement at the lower levels means that, execution happens faster.  
1. **Prevents costly mistakes** – Guardrails ensure financial and strategic oversight.  

I think it would be beneficial to use this checklist whenever assigning a responsibility (*I have tried to do it with the folks whom i mentor and it works, so it might help you*):

- [ ] What needs to be achieved? (Expectations)  
- [ ] What authority and resources do they have? (Rights)  
- [ ] How will success be measured? (Metrics/Checkpoints)  
- [ ] What are the constraints? (Boundaries/Limitations)?  
- [ ] What decision-making rights need approvals or oversight?  