---
title: Technical preview releases
titleSuffix: Configuration Manager
description: Learn about the technical preview branch to test-drive new functionality and capabilities in Configuration Manager.
ms.date: 07/11/2019
ms.prod: configuration-manager
ms.technology: configmgr-other
ms.topic: conceptual
ms.assetid: 9ce0a8cb-f96c-4e41-834c-59ceb54ce44a
author: aczechowski
ms.author: aaroncz
manager: dougeby
ms.collection: M365-identity-device-management
---

# Technical preview for Configuration Manager

*Applies to: System Center Configuration Manager (Technical Preview)*

This article provides details about the monthly technical preview branch of Configuration Manager. The technical preview introduces new functionality that Microsoft is working on. It introduces new features that aren't yet included in the current branch of Configuration Manager. These features might eventually be included in an update to the current branch. Before we finalize the features, we want you to try them out and give us feedback.  

Because this release is a technical preview, details and functionality are subject to change.  

This information applies to all versions of the Configuration Manager technical preview branch. This article lists each new feature along with the technical preview version in which it first appears. For example, version **1901** for January (01) of 2019 (19). Separate articles dedicated to each preview version detail the individual features.  

For information about what's new in the *current branch* of Configuration Manager, see [What's new in Configuration Manager incremental versions](/sccm/core/plan-design/changes/whats-new-incremental-versions).

> [!Tip]  
> To get notified when this page is updated, copy and paste the following URL into your RSS feed reader:
> `https://docs.microsoft.com/api/search/rss?search=%22technical+preview+releases+-+Configuration+Manager%22&locale=en-us`

## <a name="bkmk_reqs"></a> Requirements and limitations  

> [!IMPORTANT]  
> The technical preview is licensed for use only in a lab environment. Microsoft may not provide support services and certain features may not be available in technical previews. Additionally, technical preview software may have reduced or different security, privacy, accessibility, availability, and reliability standards relative to commercially provided software.  

For most product prerequisites, use the information in the [Supported configurations](/sccm/core/plan-design/configs/supported-configurations). The following exceptions apply to the technical preview branch:  

- Each install is active for 90 days before it becomes inactive.  

- English is the only language supported.  

- It only supports the following setup command-line parameters:  

    - `/silent`  
    - `/testdbupgrade`  

- The service connection point installs to online mode. It doesn't support offline mode.  

- The separate articles for each specific version of the technical preview include additional limitations or requirements, as applicable.

- The following features aren't supported with the technical preview branch:  

    - [Migration](/sccm/core/migration/migrate-data-between-hierarchies) to or from this preview branch.  

    - [Upgrade](/sccm/core/servers/deploy/install/upgrade-to-configuration-manager) to this preview branch.  

    - [Site recovery](/sccm/core/servers/manage/recover-sites) from the cd.latest folder.  <!--507106-->

- There's no support for updating to current branch from this preview branch.  

    > [!Note]  
    > When updates are available for a preview version, you still find and install them from the **Updates and Servicing** node of the Configuration Manager console. For a video of the in-console upgrade process, see [Installing Configuration Manager update packages](https://www.youtube.com/embed/KBd_EGFbUT8) on youtube.com.  

- It only supports a standalone primary site. There's no support for a central administration site, multiple primary sites, or secondary sites.  

The technical preview branch of Configuration Manager supports the following products and technologies:

- It only supports the following versions of **SQL Server**:  

    - SQL Server 2017 (with cumulative update 2 or later)
    - SQL Server 2016 (with no service pack or later)
    - SQL Server 2014 (with service pack 1 or later)
    - SQL Server 2012 (with service pack 3 or later)  

- The site supports up to 10 clients, which must run one of the following versions of Windows:  

    - Windows 10  
    - Windows 8.1  
    - Windows 7  

> [!Note]  
> The inclusion of these products in this content doesn't imply an extension of support for a version that's beyond its support lifecycle. Configuration Manager doesn't support products that are beyond their support lifecycle. For more information, see [Microsoft Lifecycle Policy](https://go.microsoft.com/fwlink/p/?LinkId=208270).  

## <a name="bkmk_install"></a> Install and update  

The Configuration Manager technical preview branch for lab use is distinct from the Configuration Manager current branch for production use.  

First install a baseline version of the technical preview branch. After installing a baseline version, then use in-console updates to bring your installation up-to-date with the most recent preview version. Typically, new versions of the technical preview are available each month.

Microsoft supports each technical preview version up until three successive versions are available. For example, when version 1708 released, version 1704 was no longer in support. Versions 1705, 1706, and 1707 remained in support. When a baseline falls out of support, it's still supported for installing a new technical preview site, assuming you immediately update to a supported version. The older baseline is supported until a new baseline version is available. Update to the latest available version from the baseline, and then repeat the update process until you install the latest technical preview version.

> [!TIP]  
> When you install an update to the technical preview, you update your preview installation to that new technical preview version. A technical preview installation never has the option to upgrade to a current branch installation. It also never receives updates from the current branch release.
>
> Several times throughout the year, there are technical preview branch and current branch versions with the same version number. For example, there is a technical preview version 1802 and a current branch version 1802.

### Active baseline versions

Install a baseline version for up to one year after its release. When you install a new technical preview site, if more than one baseline version is currently available, use the latest baseline version.

- **Technical preview version 1907**: The Configuration Manager technical preview version 1907 is available as both an in-console update and as a new baseline version. Download baseline versions from the [TechNet Evaluation Center](https://www.microsoft.com/evalcenter/evaluate-system-center-configuration-manager-and-endpoint-protection-technical-preview).


## <a name="BKMK_TPFeedback"></a> Providing feedback  

We love to hear your feedback about the new features in the technical preview. For more information, see [Product feedback](/sccm/core/understand/find-help#product-feedback).

If you have ideas about new features you would like to see, we want to know that as well. To submit new ideas and to vote on the ideas submitted by others, [visit our UserVoice page](https://configurationmanager.uservoice.com).  


<!--   ##  <a name="bdmk_tpknownissues"></a> General changes introduced in Technical Previews    -->


## <a name="bkmk_tpCaps"></a> Features in the most recent version  

The following features are available with the most recent Configuration Manager technical preview version:

<!-- This is the full list of new features in the latest TP release -->

### Technical Preview version 1907

<!-- - [title](/sccm/core/get-started/2019/technical-preview-1901#bkmk_anchor) <!--ID-->

- [Search the task sequence editor](/sccm/core/get-started/2019/technical-preview-1907#bkmk_tsedit) <!--4621085-->
- [Improvements to Office 365 ProPlus upgrade readiness dashboard](/sccm/core/get-started/2019/technical-preview-1907#improvements-to-office-365-proplus-upgrade-readiness-dashboard) <!--4021125-->

> [!Note]  
> Features that were available in a previous version of the technical preview remain available in later versions. Similarly, features that are added to the Configuration Manager current branch remain available in the technical preview branch.  


## Features in recent technical previews

The following features were released with previous versions of the Configuration Manager technical preview branch since the last current branch release:

> [!Tip]  
> When a new current branch version is available, features that are available in that version are listed in the latest *What's new* article. For more information, see [What's new in incremental versions](/sccm/core/plan-design/changes/whats-new-incremental-versions#supported-versions).

<!-- This is the full list of new features in the past TP releases since the last CB release. 
Each month, add features from the list above to a new H3 section at the top of this section. 
When there's a new CB, add any features not in that CB to the table in H2 "Features in previous technical previews"
-->

### Technical Preview version 1906

- [Improvements to maintenance tasks](/sccm/core/get-started/2019/technical-preview-1906#improvements-to-maintenance-tasks) <!--3555894-->
- [Configuration Manager update database upgrade monitoring](/sccm/core/get-started/2019/technical-preview-1906#configuration-manager-update-database-upgrade-monitoring) <!--4200581-->
- [Multiple pilot groups for co-management workloads](/sccm/core/get-started/2019/technical-preview-1906#bkmk_comgmt_pilot) <!--3555750-->
- [Redesigned notification logic for newly available software](/sccm/core/get-started/2019/technical-preview-1906#redesigned-notification-logic-for-newly-available-software) <!--3555904-->
- [RBAC on folders](/sccm/core/get-started/2019/technical-preview-1906#rbac-on-folders) <!--3600867-->
- [Azure Active Directory user group discovery](/sccm/core/get-started/2019/technical-preview-1906#bkmk_aad-disco) <!--3611956-->
- [Remote control anywhere using cloud management gateway](/sccm/core/get-started/2019/technical-preview-1906#remote-control-anywhere-using-cloud-management-gateway) <!--4575930-->
- [Improvements to Community Hub](/sccm/core/get-started/2019/technical-preview-1906#bkmk_hub) <!--3555935-->
- [Add joins, additional operators, and aggregators in CMPivot](/sccm/core/get-started/2019/technical-preview-1906#bkmk_cmpivot) <!--4054074-->
- [Improvements to CMPivot](/sccm/core/get-started/2019/technical-preview-1906#improvements-to-cmpivot) <!--4619340,4683130-->
- [Improvements to Configuration Manager console](/sccm/core/get-started/2019/technical-preview-1906#bkmk_console) <!--4223683-->
- [Support for Windows Virtual Desktop](/sccm/core/get-started/2019/technical-preview-1906#bkmk_winsku) <!--3556025-->
- [More frequent countdown notifications for restarts](/sccm/core/get-started/2019/technical-preview-1906#more-frequent-countdown-notifications-for-restarts) <!--3976435-->
- [Co-management auto-enrollment using device token](/sccm/core/get-started/2019/technical-preview-1906#bkmk_comgmt) <!--4454491-->
- [Additional options for third-party update catalogs](/sccm/core/get-started/2019/technical-preview-1906#additional-options-for-third-party-update-catalogs) <!--4469002-->
- [Clear app content from client cache during task sequence](/sccm/core/get-started/2019/technical-preview-1906#bkmk_tscache) <!--4485675-->
- [New Windows 10, version 1903 and later product category](/sccm/core/get-started/2019/technical-preview-1906#new-windows-10-version-1903-and-later-product-category) <!--4682946-->
- [Management insights rule for NTLM fallback](/sccm/core/get-started/2019/technical-preview-1906#bkmk_ntlm) <!--4572953-->
- [Filter applications deployed to devices](/sccm/core/get-started/2019/technical-preview-1906#bkmk_appcategory) <!--4451056-->
- [Improvements to OS deployment](/sccm/core/get-started/2019/technical-preview-1906#bkmk_osd) <!--4668846, 2840337, 4512937-->
- [Direct link to custom tabs in Software Center](/sccm/core/get-started/2019/technical-preview-1906#bkmk_swctr) <!--4655176-->

### Technical Preview version 1905

- [Improved control over WSUS maintenance](/sccm/core/get-started/2019/technical-preview-1905#improved-control-over-wsus-maintenance) <!--4110109-->
- [Improvements to Configuration Manager console](/sccm/core/get-started/2019/technical-preview-1905#bkmk_console) <!--4616810-->
- [Configure the default maximum run time for software updates](/sccm/core/get-started/2019/technical-preview-1905#bkmk_timeout) <!--3734426-->
- [Windows Defender Application Guard file trust criteria](/sccm/core/get-started/2019/technical-preview-1905#bkmk_wdag) <!--3555858-->
- [Application groups](/sccm/core/get-started/2019/technical-preview-1905#bkmk_app-group) <!--3555907-->
- [Task sequence as an app model deployment type](/sccm/core/get-started/2019/technical-preview-1905#bkmk_tsdt) <!--3555953-->
- [BitLocker management](/sccm/core/get-started/2019/technical-preview-1905#bkmk_bitlocker) <!--3601034-->
- [Task sequence debugger](/sccm/core/get-started/2019/technical-preview-1905#bkmk_tsdebug) <!--3612274-->
- [Delivery Optimization in client data sources dashboard](/sccm/core/get-started/2019/technical-preview-1905#bkmk_do) <!--3555759-->
- [Improvements to Community Hub](/sccm/core/get-started/2019/technical-preview-1905#bkmk_hub) <!--4224401-->
- [View SMBIOS GUID in device lists](/sccm/core/get-started/2019/technical-preview-1905#bkmk_smbios) <!--4526580-->
- [OneTrace log viewer](/sccm/core/get-started/2019/technical-preview-1905#bkmk_onetrace) <!--3555962-->
- [Software Center infrastructure improvements](/sccm/core/get-started/2019/technical-preview-1905#bkmk_swctr) <!--3555950-->
- [Improvements to Software Center tab customizations](/sccm/core/get-started/2019/technical-preview-1905#improvements-to-software-center-tab-customizations) <!--4063773-->
- [Improvements to app approvals](/sccm/core/get-started/2019/technical-preview-1905#bkmk_approve) <!--4224910-->
- [Retry the install of pre-approved applications](/sccm/core/get-started/2019/technical-preview-1905#bkmk_retry) <!--4336307-->
- [Install applications for a device](/sccm/core/get-started/2019/technical-preview-1905#bkmk_device-app) <!--4402180-->
- [More frequent countdown notifications for restarts](/sccm/core/get-started/2019/technical-preview-1905#bkmk_restart) <!--3976435-->
- [Synchronize collection membership results to Azure Active Directory groups](/sccm/core/get-started/2019/technical-preview-1905#bkmk_aadcollsync) <!--3607475-->
- [Configure client cache minimum retention period](/sccm/core/get-started/2019/technical-preview-1905#bkmk_cache) <!--4485509-->
- [Improvements to OS deployment](/sccm/core/get-started/2019/technical-preview-1905#bkmk_osd) <!--4512937,4224642-->
- [Add a SQL AlwaysOn node](/sccm/core/get-started/2019/technical-preview-1905#bkmk_sqlao) <!--3127336-->

### Technical Preview version 1904

- [Office 365 ProPlus upgrade readiness dashboard](/sccm/core/get-started/2019/technical-preview-1904#bkmk_o365) <!--4021125-->  
- [Configure dynamic update during feature updates](/sccm/core/get-started/2019/technical-preview-1904#configure-dynamic-update-during-feature-updates) <!--4062619-->  
- [Community Hub and GitHub](/sccm/core/get-started/2019/technical-preview-1904#community-hub-and-github) <!--3555935,3555936-->  
- [CMPivot standalone](/sccm/core/get-started/2019/technical-preview-1904#bkmk_cmpivot) <!--3555890-->  
- [Software Center infrastructure improvements](/sccm/core/get-started/2019/technical-preview-1904#bkmk_swctr) <!--3555950-->  
- [Improved control over WSUS maintenance](/sccm/core/get-started/2019/technical-preview-1904#improved-control-over-wsus-maintenance) <!--4110109-->  
- [Pre-cache driver packages and OS images](/sccm/core/get-started/2019/technical-preview-1904#bkmk_precache) <!--4224642-->  
- [Improvements to OS deployment](/sccm/core/get-started/2019/technical-preview-1904#bkmk_osd) <!--2839943,4447680-->  

### Technical Preview version 1903

- [Cloud services cost estimator](/sccm/core/get-started/2019/technical-preview-1903#bkmk_cmg) <!--3555774-->  
- [Use your distribution point as a local cache server for Delivery Optimization](/sccm/core/get-started/2019/technical-preview-1903#bkmk_doinc) <!--3555764-->  
- [Reclaim lock for editing task sequences](/sccm/core/get-started/2019/technical-preview-1903#bkmk_sedo) <!--3699337-->  
- [Drill through required updates](/sccm/core/get-started/2019/technical-preview-1903#bkmk_req-updates) <!--4224414-->  
- [Improvement to task sequence media creation](/sccm/core/get-started/2019/technical-preview-1903#bkmk_tsmedia) <!--4090666-->  


## Features in previous technical previews

The following features were released with previous versions of the Configuration Manager technical preview branch. These features remain available in later versions, but aren't yet available in the current branch.

<!-- This is the list of individual features that are still in TP (not in CB). 
**Note there is no third column in this table!**
Copy from the bottom of the list above any individual feature that is still in TP and add to the top of this list (then remove the third column)
With each CB release, review and remove from this list for anything that's now available in CB. 
-->

| Feature        | Technical preview version |  
|----------------|---------------------------|
| Download reports from the Community Hub<!--3555936--> | [Tech Preview 1812](capabilities-in-technical-preview-1812.md#bkmk_hub) |
| Community Hub <!--3556020, fka 1357766--> | [Tech Preview 1807](capabilities-in-technical-preview-1807.md#bkmk_hub) |
| Client-based PXE responder service <!--3556018, fka 1357148--> | [Tech Preview 1712](capabilities-in-technical-preview-1712.md#client-based-pxe-responder-service) |
| PXE network boot support for IPv6 <!--3601254, fka 1269793--> |[Tech Preview 1706](capabilities-in-technical-preview-1706.md#pxe-network-boot-support-for-ipv6)|
| Use Azure Active Directory <!--3607315, fka 1322145--> | [Tech Preview 1702](capabilities-in-technical-preview-1702.md#azurediscovery) |
| Improvements to Asset Intelligence <!--3601024, fka 1307390--> | [Tech Preview 1608](capabilities-in-technical-preview-1608.md#improvements-to-asset-intelligence) |
| End users can install apps from the Company Portal <!--3601249, fka 1037233--> | [Tech Preview 1605](capabilities-in-technical-preview-1605.md#BKMK_End) |


## See also  

For more information, see the following articles:  

- [Evaluate Configuration Manager in a lab](/sccm/core/get-started/evaluate-with-lab-environment)
- [What's new in Configuration Manager incremental versions](/sccm/core/plan-design/changes/whats-new-incremental-versions)  
- [Introduction to Configuration Manager](/sccm/core/understand/introduction)

> [!Tip]  
> For more information on current branch features that require consent to enable, see [pre-release features](/sccm/core/servers/manage/pre-release-features).  
>
> For more information on current branch features that you must enable first, see [Enable optional features from updates](/sccm/core/servers/manage/install-in-console-updates#bkmk_options).  
