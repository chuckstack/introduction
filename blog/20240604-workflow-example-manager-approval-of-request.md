---
title: "Workflow Example - Manager Approval of Request"
author: "Chuck Boecking"
date: 2024-06-04
tags: [operations,workflow,example]
type: blog
audience: [cio,coo,cto,ceo]
published: true

---

# Workflow Example - Manager Approval of Request

Below is an common workflow challenge. The purpose of this post is to walk you through the options and preferences to solve the below scenario:

> You are a manager in a sales organization. You have a sales rep that just assigned themselves to an account. You need to know when this happens, and you need to be able to approve the change before the sales rep can take action.

## Option 1: Queue-Based Activity Workflow
The single easiest way to implement this example approval workflow is to use queue-based activity logic. Here is how you would implement it:
- Manage record state: you want to allow a record to enter a specific state:
    - Let's say you have two fields: 1. Sales Rep drop down and 2. Sales Rep Approved checkbox.
    - You write a trigger that removes the approval any time the Sales Rep field changes.
- Manage activities: you want a way to know if any record enters your defined state
    - You have list of activities that you monitor.
    - Each activity has a count.
    - If the count is non-zero, there is work to be done.
    - Zoom to the records and approve them.
    - Creating an activity is a easy as creating a SQL view - which in today's world of AI is quite simple.

The beauty (pro) of this option is that little effort is required to execute this workflow:
- write one trigger to ensure the Sales Rep Approval is unchecked upon change, and
- add this activity to your queue in the form of a view.

The downsides (con) of this option are:
- If you are monitoring a hight number of activities (say over 40), an additional activity might get missed in the volume.
- There is no easy way to pass the approval to someone else.

Queue-based activity workflow is a good solution for this scenario. The only real concern would come if there is an already excessive list of activities to monitor. Here is an example of an activity list:
```bash
Activities:
├── Request (high priority): 6
├── Request (low priority): 19
├── Sales Orders Pending Approval: 0
├── Drafted Invoice: 0
├── Big Dollar Quotes: 99
└── Sales Rep BP Approval: 10
```

## Option 2: Ad hoc Workflow
The ad hoc workflow option is more complex than a simple queue of activities. I want to spend a moment talking about what ad hoc workflows are and how they relate to the above scenario. The centerpiece of the ad hoc workflow is the request. Here are the details of a request:
- It is a 'thing' that gets created when action is needed.
- It has state and a target (who has the next action).
- When it reaches its conclusion, it has a resolution.
- Its state, target and resolution can be set by almost anyone.
- The request tracks its history along the way.
- Users are notified when changes occur.
- Open requests are often listed as an item in your list of activities (combining the two workflow types).

Ad hoc workflows are best when either the system or users know who can execute what task/approval. Said another way, ad hoc workflows work best when a) there is a high degree of institutional knowledge about approval procedures and b) the system does a good job of ensuring only authorized roles execute the appropriate tasks.

In the above sales rep approval example, the system knows who to send the request to => its the sales rep's manager. 

The beauty (pro) of this option is its adaptability to almost any circumstance.
- It does not matter what type of action is needed.
- It does not matter who needs to approve it.
- It does not matter how many people it takes to get the action done.

The downsides (con) of this option are:
- There is limited control over who changes what request fields.
- There is a chance the request gets orphaned in an undetermined state.
- The flow of the request is unpredictable.

Ad hoc workflow is a good solution for this scenario. It is especially good if the action being approved is not business critical, and your users already understand and currently use ad hoc workflow.

## Option 3: Tradition Workflow
The traditional workflow is the most restrictive of the workflow options. It is the ad hoc workflow process with guardrails applied. It requires the person who designs the workflow process to think ahead of all possible permutations for a request in terms of state, action, transition, activity and resolution. Once the request is created, it is bound by these guardrails through the request reaches its final state.

The beauty (pro) of this option is its ability to enforce standards.
- Performs well in high-volume workflow processes.
- Ensures requests do not get lost or orphaned.

The downsides (con) of this option are:
- It does not always resemble the real world due to its restrictions.
- Requires the most effort to create the intial workflow process.

## Conclusion
Options 1 and 2 are the most desirable solutions for this scenario. Option 1: queue-based activity is the quick solution. Option 2: ad hoc workflow is the most versatile solution. If you want help implementing your organization's workflows, let us know.

If you wish to learn more, join the [chuck-stack support academy](https://buy.stripe.com/7sIbLIeeU3oT4IEfYY). For more information:
- [FAQ](../faq-academy.md)

Chuck Boecking
- 512.850.6068 (office and cell)
- chuck@chuboe.com
- www.ChuckBoecking.com
- http://www.linkedin.com/pub/chuck-boecking/10/970/17b
