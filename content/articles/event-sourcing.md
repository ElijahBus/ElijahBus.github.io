---
title: Event Sourcing
description: What Is Event Sourcing
date: 'Nov 2, 2023'
published: true
---

# Event Sourcing
---
✍️ <b>[Elijah Bus](https://linkedin.com/in/elie-busanga)</b>

## Quick Story

<p>... Boss <b>😎Joe</b> has an e-commerce site, <b>👨‍💻Mike</b> is the developer</p> 

<p><b>😎Joe</b> : I am building an e-commerce site, I would like to keep track of the quantity of products in stock, the time and amount of the purchase.</p>
<p><b>👨‍💻Mike</b>: Yes sir, Mike creates a new table 'purchase_logs' and save to the logs every purchase details</p>
<p class="ml-4">
<em>
But, while users are purchasing products. Boss Joe is also updating the quantity of products in stock, but Mike does not know. 
Next morning Mike checks the dashboard and find the quantity of products did not change, while users have been purchasing the products.
</em>
</p>
<p><b>😎Joe</b> : Hi Mike, I would like to have the report of the products I added to the stock the last 7 days</p>
<p><b>👨‍💻Mike</b>: Sorry sir, there is no way we can give you that at the moment</p>
<p><b>😡Joe</b> : We need a meeting ASAP and should magically find a way to get that report</p>
<p><b>👨‍💻Mike</b>: The confused, decides to create another ' update_logs ' table to keep track of the updates of products in stock.</p>

**Questions:**
- How many logs tables will Mike create as the system grows and the need for more reports ?
- Per adventure, there is a race condition, the data is no longer accurate, how will Mike know what the correct state of data should be ?
- The system scale and Mike would like to delegate some responsibilities to other services, is Mike going to recreate the same logs table for each service ?   

## What and why event sourcing

The fundamental idea of Event Sourcing is that of ensuring every change to the state of an 
application is captured in an event object, and that 
these event objects are themselves stored in the sequence 
they were applied for the same lifetime as the application state itself. *([Martin Fowler](https://martinfowler.com/eaaDev/EventSourcing.html))*

Let's sketch it simple how event sourcing would help Mike in his situation:
<br />

![es1.svg](/svg/es1.svg)

## What we get from event sourcing
- Application state can be cleared but then recovered from the events logs
- We can pass on the stream of events to other services
- We can keep the log of events that happened instead of keeping the logs of actions (CRUD)
- Gives more insight in why the application state changed
- Events are decoupled from actions

**Coming next:** Implementation of Event Sourcing in a Node.js application.
<br />

Follow the author at **[@elijahbus](https://x.com/elijahbus)**, so you don't miss the update.