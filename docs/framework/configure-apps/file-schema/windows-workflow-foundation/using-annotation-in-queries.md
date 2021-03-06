---
title: "Using Annotation in Queries | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "reference"
ms.assetid: 50855b30-d5fe-49a9-89d3-3f1bfd670958
caps.latest.revision: 3
author: "Erikre"
ms.author: "erikre"
manager: "erikre"
---
# Using Annotation in Queries
Annotations allow you to arbitrarily tag tracking records with a value that can be configured after build time. For example, you might want several tracking records across several workflows to be tagged with “Mail Server” == “Mail Server1”. This makes it easy to find all records with this tag when querying tracking records later.  
  
## Adding Annotations  
 An annotation can be added to a tracking query as shown in the following example.  
  
```  
<activityStateQuery activityName="SendEmailActivity">  
  <states>  
    <state name="Closed"/>  
  </states>  
  <annotations>  
    <annotation name="MailServer" value="Mail Server1"/>  
  </annotations>  
</activityStateQuery>  
  
```  
  
> [!NOTE]
>  These tracking query elements can be used to create a tracking profile. A tracking profile can be created either in configuration or using code.  
  
## See Also  
 <xref:System.ServiceModel.Activities.Tracking.Configuration.ProfileWorkflowElement>   
 <xref:System.Activities.Tracking.TrackingProfile>   
 [\<participants>](../../../../../docs/framework/configure-apps/file-schema/windows-workflow-foundation/participants.md)   
 [Workflow Tracking and Tracing](../../../../../docs/framework/windows-workflow-foundation/workflow-tracking-and-tracing.md)   
 [Tracking Profiles](../../../../../docs/framework/windows-workflow-foundation/tracking-profiles.md)