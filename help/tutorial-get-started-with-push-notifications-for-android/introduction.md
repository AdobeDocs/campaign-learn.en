---
title: Getting started with Push notifications for Android - Introduction
description: This tutorial walks you through the steps involved in sending push notifications from Adobe Campaign and receiving these notifications in your Android™ app.
feature: Push
jira: KT-6438
doc-type: article
activity: setup
team: TM
role: Admin, Developer
level: Experienced
recommendations: noCatalog
exl-id: 91ff4bae-8598-4227-b4c9-4e436ce7400d
---
# Getting started with Push notifications for Android - Introduction

Adobe Campaign allows you to send personalized and segmented [!DNL push] notifications to [!DNL iOS] and [!DNL Android™] mobile devices. This tutorial walks you through the steps involved in sending [!DNL push] notifications from Adobe Campaign to an [!DNL Android™] app.

## Prerequisites

Before you can begin, you must have the following:

1) **Android™ Mobile application**

    This tutorial does not cover the detailed steps required to set up the mobile application. You must have an **[!DNL Android™] mobile application with the [!DNL Campaign SDK] integrated**.

    You can find a detailed description of the required steps in the product documentation:

    [Integrating Campaign SDK into the mobile application](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-push-notifications/integrating-campaign-sdk-into-the-mobile-application.html)

2) **[!DNL Mobile App channel] package installed**

    The [!DNL Mobile App channel] package must be installed on your [!DNL Campaign] instance. The following video explains how to check if the [!DNL Mobile App channel] is installed on your instance and if not, how to install it.

>[!VIDEO](https://video.tv.adobe.com/v/326544?quality=12&learn=on)

## Tutorial Overview

The objective is to send a personalized promotional [!DNL push] notification to the subscribers of the [!DNL Neotrip] [!DNL Android™] mobile app. The [!DNL Neotrip] app is configured with the [!DNL Campaign SDK] and  the [!DNL Mobile App channel] is activated on the [!DNL Campaign] instance.

The following configuration steps are required:

### Step 1: Extend the app subscription schema to personalize [!DNL push] notifications

To be able to personalize the [!DNL push] notification, you must first [extend the app subscription schema](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md). THis allows the system to store the personalization values that are received from the app when the user subscribes to the service.

### Step 2: Configure the Android™ service and create the mobile application in Campaign

Next, [the Android™ service must be configures and the mobile application created in Campaign](/help/tutorial-get-started-with-push-notifications-for-android/configure-an-android-service-in-campaign.md). In this step, the [!DNL Neotrip] app is defined as the target for the push notification.

### Step 3: Configure and send the push notification

Now the push notification is ready to be [configured and sent](/help/tutorial-get-started-with-push-notifications-for-android/configure-and-send-push-notifications.md).

## Start the tutorial

Step 1: [Extend the app subscription schema](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md)
