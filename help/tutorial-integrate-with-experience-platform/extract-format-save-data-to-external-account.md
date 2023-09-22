---
title: Create an export workflow (Part 2) - Extract, format, and save data to an external account
description: In this second part of the Create an Export Workflow tutorial, you learn how to format the data for export and how to save the data to an external account.
feature: Data Management, Workflows
jira: KT-8160
thumbnail: 336391.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
exl-id: ac29b75c-a838-4183-8ec5-034281290725
---
# Create an export workflow (Part 2): Extract, format, and save data to an external account

In this second part of the Create an Export Workflow tutorial, you learn how to format the data for export and how to save the data to an external account.

>[!VIDEO](https://video.tv.adobe.com/v/336391?quality=12&learn=on){transcript=true}

## Assets

JavaScript: Save date

 ```java
  logInfo("=====================")
  logInfo("Starting Execution...")

  optionName = vars.OPTION_NAME;
  logInfo("optionName: " + optionName);
  logInfo("NEXT Run Date: " + vars.nextRunTime);
  
  //Make sure we have valid values before saving for next run
  if (vars.nextRunTime == null || optionName == null){

    logInfo("Unable to find non-null values for optionName/nextRunTime! Throwing Error.")
    throw new Error('Unable to find non-null values for optionName/nextRunTime!  Ending Execution.');

  } else {

    // Save the nextRunTime to the database to establish starting point for next run.
    setOption(optionName, vars.nextRunTime);
    logInfo("Date Saved. [" + optionName + "] = [" + vars.lastRunTime + "]")

  }

  logInfo("Finished Execution.") 
  logInfo("===================")
 ```
