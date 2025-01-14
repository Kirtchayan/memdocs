---
# required metadata
title: Windows 365 Switch known issues
titleSuffix:
description: Learn about known issues with Windows 365 Switch, including workarounds and updated fixes.
keywords:
author: ErikjeMS  
ms.author: erikje
manager: dougeby
ms.date: 09/26/2023
ms.topic: troubleshooting
ms.service: windows-365
ms.subservice: 
ms.localizationpriority: high
ms.technology:
ms.assetid: 

# optional metadata

#ROBOTS:
#audience:

ms.reviewer: elluthra
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure; get-started
ms.collection:
- M365-identity-device-management
- tier2
---

# Windows 365 Switch known issues

This page lists recent known issues with [Windows 365 Switch](windows-365-switch-overview.md).

## Support for only one Cloud PC

Currently, Windows 365 Switch only supports one Switch-enabled Cloud PC. The user is automatically signed into the first available Switch-supported Cloud PC from the list of Cloud PCs assigned to the user. Using Switch, the user can choose which Cloud PC to sign in to by selecting the ellipses (...) > choose the Cloud PC > **Add to Task view**. Only one Cloud PC can be added to Task view at a time.

## Limited gestures

Some gestures aren't supported in the Cloud PC, like three finger gestures to change app or four finger gesture to bring up the Task view and show the desktop. These gestures instead get triggered on the physical device. Other than these gestures, all the usual Windows 11 gestures are supported.

## Bluetooth and hardware settings can't be managed from the Cloud PC

Cloud PCs lack hardware components like bluetooth adapters. Users can't change it from the Cloud PC Settings app or quick Settings. 

**Troubleshooting steps**:

Users must switch back to their physical device and change the settings in the Settings app.

## Reconnect button not working

If the **Reconnect** option in the disconnect message dialog is used, reconnecting might not work as expected or may result in an unusable Cloud PC session.

**Troubleshooting steps**:

Let the disconnect complete and then launch a new connection using Task view.

## Navigation between sign in prompts and your Cloud PC

After selecting a Cloud PC from the Task view, users might be prompted to sign in using their account credentials. In some builds of Windows, after providing the credentials, the user might not be returned to the Cloud PC connection.

**Troubleshooting steps**:

Select the Task view button for the Cloud PC again. The connection continues in the background. The user should be connected to their Cloud PC within a few minutes

<!-- ########################## -->
## Next steps

[Troubleshooting](troubleshooting.md)
