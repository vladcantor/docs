---
title: "IMetaDataImport::ResetEnum Method | Microsoft Docs"
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
  - "IMetaDataImport.ResetEnum"
apilocation: 
  - "mscoree.dll"
apitype: "COM"
f1_keywords: 
  - "IMetaDataImport::ResetEnum"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ResetEnum method [.NET Framework metadata]"
  - "IMetaDataImport::ResetEnum method [.NET Framework metadata]"
ms.assetid: dda867b5-1050-49ba-b01c-fcc83b7a5617
caps.latest.revision: 11
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# IMetaDataImport::ResetEnum Method
Resets the specified enumerator to the specified position.  
  
## Syntax  
  
```  
HRESULT ResetEnum (  
   [in] HCORENUM    hEnum,   
   [in] ULONG       ulPos  
);  
```  
  
#### Parameters  
 `hEnum`  
 [in] The enumerator to reset.  
  
 `ulPos`  
 [in] The new position at which to place the enumerator.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** Cor.h  
  
 **Library:** Included as a resource in MsCorEE.dll  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## See Also  
 [IMetaDataImport Interface](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-interface.md)   
 [IMetaDataImport2 Interface](../../../../docs/framework/unmanaged-api/metadata/imetadataimport2-interface.md)