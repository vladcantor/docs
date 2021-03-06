---
title: "COR_PRF_FUNCTION Structure | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "COR_PRF_FUNCTION"
apilocation: 
  - "mscorwks.dll"
apitype: "COM"
f1_keywords: 
  - "COR_PRF_FUNCTION"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "COR_PRF_FUNCTION structure [.NET Framework profiling]"
ms.assetid: 8bb5acf5-cf4b-4ccb-93f1-46db1f3f8bf3
caps.latest.revision: 6
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# COR_PRF_FUNCTION Structure
Provides a unique representation of a function by combining its ID with the ID of its recompiled version.  
  
## Syntax  
  
```  
typedef struct _COR_PRF_FUNCTION {    FunctionID functionId;    ReJITID    reJitId;} COR_PRF_FUNCTION;  
```  
  
## Members  
  
|Member|Description|  
|------------|-----------------|  
|`functionId`|The ID of the function.|  
|`reJitId`|The ID of the recompiled function. A value of 0 (zero) represents the original version of the function.|  
  
## Remarks  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorProf.idl  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]  
  
## See Also  
 [Profiling Structures](../../../../docs/framework/unmanaged-api/profiling/profiling-structures.md)