---
title: Create an export workflow (Part 1) - Find the last modified date for a list of recipients
description: In this first part of the Create an Export Workflow tutorial, learn how to create a workflow that finds the last modified date for a list of recipients created from an Experience Platform segment.
feature: Data Management, Workflows
jira: KT-8162
thumbnail: 336387.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
exl-id: 6fd70eea-3be7-4589-a608-05b0a8de93a6
TQID: https://experienceleague.adobe.com/0C-fRmXsfzB-1kePFSNtzUFtqPHDQ1wW1LH2-6Zuw5g
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
---
# Create an export workflow (Part 1) - Find the last modified date for a list of recipients

In this first part of the Create an Export Workflow tutorial, learn how to create a workflow that finds the last modified date for a list of recipients created from an Experience Platform segment.

>[!VIDEO](https://video.tv.adobe.com/v/336387?quality=12&learn=on){transcript=true}

## Assets

JavaScript to establish date ranges:

 ```java
  var DEFAULT_LOOKBACK_DAYS = 90;
  vars.OPTION_NAME = "BroadLog_CaptureTime";

  logInfo("=====================");
  logInfo("Starting Execution...");

  // Establish the last and next RunTimes
  var lastRunTime = getOption(vars.OPTION_NAME);
  var nextRunTime = getCurrentDate();

  //To reset and run through DEFAULT_LOOKBACK, uncomment the following line.
  //lastRunTime = null;

  logInfo("NEXT Run Date Set: [" + nextRunTime + "]");
  logInfo("LAST Run Date Retrieved (" + lastRunTime + ")");

  //Check for null so we can default the lastRunTime using the DEFAULT_LOOKBACK 
  if (lastRunTime == null || lastRunTime == "null" || lastRunTime == "") {

    logInfo("Empty Date Retrieved, setting to default lookback (-" + DEFAULT_LOOKBACK_DAYS + " days)");
    lastRunTime = new Date();
    lastRunTime.setDate(nextRunTime.getDate() - DEFAULT_LOOKBACK_DAYS);
    logInfo("LAST Run Date Set: [" + lastRunTime + "]");

  } 

  //Persist values through execution of this instance of the workflow.
  vars.lastRunTime = lastRunTime;
  vars.nextRunTime = nextRunTime;

  logInfo("Finished Execution.");
  logInfo("===================");
 ```

## Next video

 [Create an export workflow (Part 2) - Extract, format, and save data to an external account](extract-format-save-data-to-external-account.md)
