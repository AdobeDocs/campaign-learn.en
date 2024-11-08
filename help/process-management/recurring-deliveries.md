---
title: Create recurring and continuous email deliveries
description: Learn how to set up a recurring and a continuous delivery and understand the differences between the two approaches.
feature: Workflows
jira: KT-7982
thumbnail: 342637.jpg
doc-type: feature video
activity: use
team: TM
role: User
level: Intermediate
exl-id: 469aecd7-4774-42c6-b07f-82792dfdc9c2
---
# Create recurring and continuous email deliveries

This tutorial explains how to set up a recurring and a continuous delivery and the differences between the two approaches.  

## Recurring and Continuous Delivery Tracking {#recurring-and-continuous-delivery-tracking}

The recurring and continuous deliveries differ in the way contact data is managed:

* The **continuous delivery** lets you add new recipients to an existing delivery and avoids you having to create a delivery each time a new recipient is added. You can update the creative directly in the campaign workflow and it updates the template in the delivery template resource folder.  
  
  A continuous delivery creates a SINGLE delivery and delivery logs (broadLog) and tracking logs, that reference that one delivery, are added each time it executes.

![Continuous Delivery](/help/assets/delivery_continuous.jpg)

* A **recurring delivery** creates a delivery instance each time it executes. For example, if the workflow is scheduled to run once a week, that would result in 52 Deliveries after one year. It also means that the broad log and tracking logs are separated by delivery instance.

![Recurring Delivery](/help/assets/delivery_recurring.jpg)

## How to set up a recurring delivery {#how-to-set-up-a-recurring-delivery}

The video explains how to configure a recurring delivery and a scheduler activity.

>[!VIDEO](https://video.tv.adobe.com/v/342638?quality=12&learn=on){transcript=true}

## How to set up a continuous delivery {#how-to-set-up-a-continuous-delivery}

This video shows how to configure a continuous delivery with an incremental query.

>[!VIDEO](https://video.tv.adobe.com/v/342637?quality=12&learn=on){transcript=true}
