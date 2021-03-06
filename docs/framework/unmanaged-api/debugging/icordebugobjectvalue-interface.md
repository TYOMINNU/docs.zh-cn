---
title: "ICorDebugObjectValue 接口 1"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugObjectValue
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugObjectValue
helpviewer_keywords: ICorDebugObjectValue interface [.NET Framework debugging]
ms.assetid: 937de6a0-6fbf-4ddc-80ea-a6217b73e62b
topic_type: apiref
caps.latest.revision: "14"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.workload: dotnet
ms.openlocfilehash: 6dfde9f212936b1a0d0f5a6e76eafd4a2e62356c
ms.sourcegitcommit: 16186c34a957fdd52e5db7294f291f7530ac9d24
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="icordebugobjectvalue-interface1"></a>ICorDebugObjectValue 接口 1
"ICorDebugValue"表示一个值，包含对象的子类。  
  
## <a name="methods"></a>方法  
  
|方法|描述|  
|------------|-----------------|  
|[GetClass 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-getclass-method.md)|公共语言运行时 (CLR) 中获取的接口指针<xref:System.Type>对象的此`ICorDebugObjectValue`引用。|  
|[GetContext 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-getcontext-method.md)|未实现。|  
|[GetFieldValue 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-getfieldvalue-method.md)|获取到的接口指针[ICorDebugValue](../../../../docs/framework/unmanaged-api/debugging/icordebugvalue-interface.md) ，表示指定类的指定字段的值。|  
|[GetManagedCopy 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-getmanagedcopy-method.md)|已过时。 请勿调用此方法。|  
|[GetVirtualMethod 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-getvirtualmethod-method.md)|未实现。|  
|[IsValueClass 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-isvalueclass-method.md)|获取一个值，该值指示此引用的对象是否`ICorDebugObjectValue`是值类型。|  
|[SetFromManagedCopy 方法](../../../../docs/framework/unmanaged-api/debugging/icordebugobjectvalue-setfrommanagedcopy-method.md)|已过时。 请勿调用此方法。|  
  
## <a name="remarks"></a>备注  
 `ICorDebugObjectValue`一直有效，直到正在调试的进程将继续运行。  
  
> [!NOTE]
>  此接口不支持跨计算机或跨进程远程调用。  
  
## <a name="requirements"></a>惠?  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CorDebug.idl、 CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [调试接口](../../../../docs/framework/unmanaged-api/debugging/debugging-interfaces.md)  
 
