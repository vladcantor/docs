---
title: "ICorProfilerCallback::ExceptionUnwindFunctionLeave Method | Microsoft Docs"
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
  - "ICorProfilerCallback.ExceptionUnwindFunctionLeave"
apilocation: 
  - "mscorwks.dll"
apitype: "COM"
f1_keywords: 
  - "ICorProfilerCallback::ExceptionUnwindFunctionLeave"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ICorProfilerCallback::ExceptionUnwindFunctionLeave method [.NET Framework profiling]"
  - "ExceptionUnwindFunctionLeave method [.NET Framework profiling]"
ms.assetid: ebaad1d5-ee0a-4cb0-96bc-8ba5d371b747
caps.latest.revision: 13
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# ICorProfilerCallback::ExceptionUnwindFunctionLeave Method
Notifies the profiler that the unwind phase of exception handling has finished unwinding a function.  
  
## Syntax  
  
```  
HRESULT ExceptionUnwindFunctionLeave();  
```  
  
## Remarks  
 When the `ExceptionUnwindFunctionLeave` method is called, the function instance and its stack data are removed from the stack.  
  
 The profiler should not block during this call because the stack may not be in a state that allows garbage collection, and therefore preemptive garbage collection cannot be enabled. If the profiler blocks here and a garbage collection is attempted, the runtime will block until this callback returns.  
  
 Also, during this call, the profiler must not call into managed code or in any way cause a managed-memory allocation.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorProf.idl, CorProf.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## See Also  
 [ICorProfilerCallback Interface](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-interface.md)   
 [ExceptionUnwindFunctionEnter Method](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-exceptionunwindfunctionenter-method.md)