---
title: "Sample: Disable or enable a user (Microsoft Dataverse) | Microsoft Docs" # Intent and product brand in a unique string of 43-59 chars including spaces
description: "This sample shows how to disable and enable a system user." # 115-145 characters including spaces. This abstract displays in the search result.
ms.date: 04/03/2022
author: paulliew
ms.author: paulliew
ms.reviewer: jdaly
ms.topic: sample
search.audienceType:
  - developer
contributors:
  - JimDaly
  - phecke
---

# Sample: Disable or enable a user

This sample shows how to disable and enable a system user account in an online or on-premise/IFD environment.

> [!div class="nextstepaction"]
> [SDK for .NET: Disable or enable a user sample code](https://github.com/microsoft/PowerApps-Samples/tree/master/dataverse/orgsvc/C%23/DisableOrEnableUser)

## How to run this sample

The user account under which you run this program must have the System Administrator role in order to enable/disable a system user.

Before building this sample, open the solution in Visual Studio and select **View** > **Task List**. There are two TODO comments that you must follow to provide the required information about an existing system user in your organization.

See [How to run samples]https://github.com/microsoft/PowerApps-Samples/blob/master/dataverse/README.md) for information about how to run this sample.

## What this sample does

The sample obtains the identifier of an existing system user and either disables or enables that user account.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

Retrieves the identifier of an existing system user that you specify (see [How to run this sample](#how-to-run-this-sample)).

### Demonstrate

Demonstrates using`SetStateRequest` to disable and enable a system user. Also shows how to retrieve information about a system user.

To view the summary of the specified system user in Customer Engagement, navigate to **Settings** > **Security** > **Users** and select the target system user account in the list. If desired, choose the **Disabled Users** system view to filter the list of all users. The user's status should be "Disabled".

### Clean up

Displays an option to enable the user account that was disabled in the `Main()` method.

Answering "yes" is optional in case you want to examine the disabled user account in Customer Engagement. You can manually enable the user account in Microsoft Entra ID or Microsoft 365 to achieve the same result.

[!INCLUDE[footer-include](../../../../includes/footer-banner.md)]
