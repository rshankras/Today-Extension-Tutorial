---
title: "developer portal changes!"
slug: developer-portal-changes
---

# Introduction

This section is about the changes to be done in Apple's developer portal for sharing data between the apps

# Sharing data between apps

The following steps needs to be followed to share data between the main app and app extension.

- Create unique App ID in apple developer account and make sure to enable App Groups under Services section. For creating a new App ID, use the bundle identifier from your project.

![Image Asset](assets/appservices.png "App Services")

- Add the UserDefaults suite name (group.makeschool.MyCurrentAddress) to the App Groups section as a container group.

![Image Asset](assets/appgroupassignment.png "App Group Management")

- Download and install the newly created developer profile on to your Mac.
- Select this developer profile in Xcode under Signing (Debug) and Signing (Release) section.

![Image Asset](assets/assignprovisioningprofileInxcode.png "Assign Provisioning Profiles in Xcode")

- Enable **App Groups** under **Capabilities** for the Project target and make sure to add the container name Under App Groups (group.makeschool.MyCurrentAddress).

![Image Asset](assets/capabilities.png "Enable App Groups under Capabilities")

# Summary

These are the developer portal related changes required for sharing data between the main app and app extension.



