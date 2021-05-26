---
title: How to set up recurring and continuous email campaigns
description: Learn how to set up a recurring and a continuous delivery and understand the differences between the two approaches.
feature: Workflows
kt: 7982
doc-type: feature video
activity: use
team: TM
role: Business Practitioner
level: Beginner
---

# How to set up recurring and continuous email campaigns

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

>[!VIDEO](https://video.tv.adobe.com/v/25040?quality=12)

## How to set up a continuous delivery {#how-to-set-up-a-continuous-delivery}

This video shows how to configure a continuous delivery with an incremental query.

>[!VIDEO](https://video.tv.adobe.com/v/25039?quality=12)
