---
title: "How to: Access the Predefined UTC and Local Time Zone Objects | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-bcl"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "time zones [.NET Framework], local"
  - "predefined time zones"
  - "UTC times, predefined"
  - "local time zone access"
  - "time zones [.NET Framework], retrieving"
  - "time zones [.NET Framework], UTC"
ms.assetid: 961fb70b-83f0-4dab-a042-cb5fcd817cf5
caps.latest.revision: 9
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# How to: Access the Predefined UTC and Local Time Zone Objects
The <xref:System.TimeZoneInfo> class provides two properties, <xref:System.TimeZoneInfo.Utc%2A> and <xref:System.TimeZoneInfo.Local%2A>, that give your code access to predefined time zone objects. This topic discusses how to access the <xref:System.TimeZoneInfo> objects returned by those properties.  
  
### To access the Coordinated Universal Time (UTC) TimeZoneInfo object  
  
1.  Use the `static` (`Shared` in Visual Basic) <xref:System.TimeZoneInfo.Utc%2A?displayProperty=fullName> property to access Coordinated Universal Time.  
  
2.  Rather than assigning the <xref:System.TimeZoneInfo> object returned by the property to an object variable, continue to access Coordinated Universal Time through the <xref:System.TimeZoneInfo.Utc%2A?displayProperty=fullName> property.  
  
### To access the local time zone  
  
1.  Use the `static` (`Shared` in Visual Basic) <xref:System.TimeZoneInfo.Local%2A?displayProperty=fullName> property to access the local system time zone.  
  
2.  Rather than assigning the <xref:System.TimeZoneInfo> object returned by the property to an object variable, continue to access the local time zone through the <xref:System.TimeZoneInfo.Local%2A?displayProperty=fullName> property.  
  
## Example  
 The following code uses the <xref:System.TimeZoneInfo.Local%2A?displayProperty=fullName> and <xref:System.TimeZoneInfo.Utc%2A?displayProperty=fullName> properties to convert a time from the U.S. and Canadian Eastern Standard time zone, as well as to display the time zone name to the console.  
  
 [!code-csharp[System.TimeZone2.Concepts#13](../../../samples/snippets/csharp/VS_Snippets_CLR_System/system.TimeZone2.Concepts/CS/TimeZone2Concepts.cs#13)]
 [!code-vb[System.TimeZone2.Concepts#13](../../../samples/snippets/visualbasic/VS_Snippets_CLR_System/system.TimeZone2.Concepts/VB/TimeZone2Concepts.vb#13)]  
  
 You should always access the local time zone through the <xref:System.TimeZoneInfo.Local%2A?displayProperty=fullName> property rather than assigning the local time zone to a <xref:System.TimeZoneInfo> object variable. Similarly, you should always access Coordinated Universal Time through the <xref:System.TimeZoneInfo.Utc%2A?displayProperty=fullName> property rather than assigning the UTC zone to a <xref:System.TimeZoneInfo> object variable.  This prevents the <xref:System.TimeZoneInfo> object variable from being invalidated by a call to the <xref:System.TimeZoneInfo.ClearCachedData%2A?displayProperty=fullName> method.  
  
## Compiling the Code  
 This example requires:  
  
-   That a reference to System.Core.dll be added to the project.  
  
-   That the <xref:System> namespace be imported with the `using` statement (required in C# code).  
  
## See Also  
 [Dates, Times, and Time Zones](../../../docs/standard/datetime/index.md)   
 [Finding the Time Zones Defined on a Local System](../../../docs/standard/datetime/finding-the-time-zones-on-local-system.md)   
 [How to: Instantiate a TimeZoneInfo Object](../../../docs/standard/datetime/instantiate-time-zone-info.md)