---
title: Create approvals and validation workflows - Introduction
description: Learn how to configure different approval validation workflows.
feature: Workflows, Approvals
doc-type: feature video
activity: setup
team: TM
role: User
level: Experienced
recommendations: noDisplay
exl-id: fa4c2180-15bb-424b-a54e-c7d744385fb6
---
# Create approvals and validation workflows - Introduction

Adobe Campaign offers several options for marketers to review and provide delivery content, campaign target, data extraction, and budget approvals. Learn how to [manage approvals](/help/process-management/create-approvals-and-validation-workflows/manage-approvals.md).

## Prerequisite {#prerequisite}

Before enabling approval steps, the marketing team must define individual reviewers:

* The Adobe Campaign reviewer role within an approval activity can either be a single reviewer (Operator) or a group of reviewers (Operator role).
* To enable campaign developers to select the reviewers as approvers in a campaign or a delivery, the reviewers and reviewer groups must be configured in Adobe Campaign by an administrator.

## Configuring approvals {#configuring-approvals}

1. [Configure approvals for campaigns](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-campaigns.md):
    If you have the same set of reviewers for all deliveries in your campaign workflow, apply the campaign approval functionality, by setting up approvals and reviewers at the campaign level. The approval tasks and reviewers are pushed down to each delivery activity of your workflow once the workflow is executed.
2. [Configure approvals for deliveries](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-deliveries.md):
   You can also set up approvals at a delivery level. If delivery approvals steps and reviewers differ from the campaign approval steps and reviewers, the delivery settings override the campaign settings.
3. [Create an approval process in a workflow](/help/process-management/create-approvals-and-validation-workflows/create-approval-process-in-a-workflow.md):
    The approval activity allows the creation of an approval process within a workflow. This way, the targeting selection logic can be approved before the delivery is launched. It also allows approval at multiple levels within the workflow, if needed.

For more information, refer to the [documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/flow-control-activities/approval.html).
