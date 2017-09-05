---
title: Register a Twilio account to send SMS
description: 
category: SETUP
author: Todd Baginski
author_github: syntaxc4
optional: true
---

{% include header.md %}

When a chat is started between two users in the application, the app will send an SMS to notify the user the message was sent to them. 

This app uses a Twilio trial account to send SMS.

If you wish to enable the SMS capabilities in the application you must create a Twilio trial account and register and verify a phone number to send SMS.

## Create and configure a Twilio trial account

1. Register a trial account

   * Open https://www.twilio.com/, then click **Get a free API key**. 
   * You will be redirected to **Sign up for free page**. Fill in the form, then click **Get Started**.
   * Twilio will show a page verify you're a human. Finish it.

2. Create a project

   After the human verification is complete, you will be redirected to a page to let you create a project.

   * Input a name, for example: **Developer Finder**, then click **Create Project**.

   * After the project is created, copy aside the **ACCOUNT ID** and **AUTH TOKEN** values.![](Images/twilio-api-credentials.png)

     > **Note:** These 2 values will be used for the **Twilio Account SID** and **Twilio Auth Token** ARM template parameters.

3. Get a phone number:

   * In the **Phone Numbers** section, click **Manage Numbers**.
   * Twilio will redirect you to the **Phone Numbers Dashboard**.
   * Click **Get Started**.
   * Click **Get you first Twilio phone number**.

     > **Note:** Twilio will pre-select a phone number.  Use the number it gives you.
   * Click **Choose this number**:

     ![](Images/twilio-phone-number.png)

   * Copy aside the phone number.

     > **Note:** This phone number will be used for the **Twilio From Phone Number** ARM template parameter.

## Verify a phone number

1. Click **Verified Caller IDs** on the **Phone Numbers page**:

   ![](Images/twilio-verified-caller-ids.png)

2. Click the red **⊕**:

   ![](Images/twilio-verify-a-phone-number.png)

3. Follow the instructions to verify the phone number.