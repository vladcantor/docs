---
title: "Application Compatibility in the .NET Framework 4.5.1 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "application compatibility,.NET Framework 4.5.1"
  - "application compatibility,.NET Framework"
ms.assetid: 2b07b729-e2bf-4925-8b83-9c9ee6c48612
caps.latest.revision: 9
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# Application Compatibility in the .NET Framework 4.5.1
This topic provides links to information about application compatibility issues between the .NET Framework 4.5 and 4.5.1. The issues are divided into two categories:  
  
 [Runtime changes](../../../docs/framework/migration-guide/runtime-changes-in-the-net-framework-4-5-1.md)  
 Runtime changes affect all apps that are running under the [!INCLUDE[net_v451](../../../includes/net-v451-md.md)] and that use a particular feature.  
  
 [Retargeting changes](../../../docs/framework/migration-guide/retargeting-changes-in-the-net-framework-4-5-1.md)  
 Retargeting changes affect apps that are recompiled to target the [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]. They include:  
  
-   Changes in the design-time environment. For example, build tools may emit warnings when previously they did not.  
  
-   Changes in the runtime environment. These affect only apps that specifically target the [!INCLUDE[net_v451](../../../includes/net-v451-md.md)]. Apps that target previous versions of the .NET Framework behave as they did when running under those versions.  
  
 In the topics that describe runtime changes and retargeting changes, we have classified individual items by their expected impact, as follows:  
  
 Major  
 This is a significant change that affects a large number of apps or that requires substantial modification of code.  
  
 Minor  
 This is a change that affects a small number of apps or that requires minor modification of code.  
  
 Edge case  
 This is a change that affects apps under very specific scenarios that are not common.  
  
 Transparent  
 This is a change that has no noticeable effect on the app's developer or user. The app should not require modification because of this change.  
  
## See Also  
 [Versions and Dependencies](../../../docs/framework/migration-guide/versions-and-dependencies.md)   
 [Application Compatibility](../../../docs/framework/migration-guide/application-compatibility.md)   
 [Application Compatibility in 4.5](../../../docs/framework/migration-guide/application-compatibility-in-the-net-framework-4-5.md)   
 [Application Compatibility in 4.5.2](../../../docs/framework/migration-guide/application-compatibility-in-the-net-framework-4-5-2.md)