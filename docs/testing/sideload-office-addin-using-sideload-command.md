---
title: Sideload Office Add-ins using the sideload command
description: ''
ms.date: 03/19/201907/24/2018
localization_priority: Priority
---

# Sideload Office Add-ins for testing using the sideload command
 
> [!NOTE]
> The sideloading technique described in this article is only valid for:
> 
> - Excel, Word, and PowerPoint add-ins that run on Windows
> 
> - Add-in projects that were created with the [Yeoman generator for Office Add-ins](https://github.com/OfficeDev/generator-office) and that have a `sideload` script in the `scripts` section of the package.json file. (Projects that were created with older versions of the Yeoman generator for Office Add-ins will not have this script.)
 
To sideload your add-in by using the `sideload` script that the Yeoman generator for Office Add-ins provides, complete the following steps:

1. Open a command prompt as an administrator.

2. Change directories to the root of your add-in project folder.

3. Run the following command to start a local web server instance on port 3000 to serve up your add-in project: `npm run start`

4. Open a second command prompt as an administrator.

5. Change directories to the root of your add-in project folder.

6. Run the following command to boot the host application (e.g. Excel, Word) and register your add-in in the host application: `npm run sideload`

If your add-in project was created with Visual Studio or does not have the sideload script, you can sideload it on Windows by using the method described in [Sideload an Office Add-in from a network share](create-a-network-shared-folder-catalog-for-task-pane-and-content-add-ins.md).

If you're not testing a Word, Excel, or PowerPoint add-in on Windows, see one of the following topics for information about sideloading your add-in:
 
- [Sideload Office Add-ins in Office Online for testing](sideload-office-add-ins-for-testing.md)
- [Sideload Office Add-ins on iPad and Mac for testing](sideload-an-office-add-in-on-ipad-and-mac.md)
- [Sideload Outlook add-ins for testing](/outlook/add-ins/sideload-outlook-add-ins-for-testing)

## See also

- [Validate and troubleshoot issues with your manifest](troubleshoot-manifest.md)
- [Publish your Office Add-in](../publish/publish.md)
