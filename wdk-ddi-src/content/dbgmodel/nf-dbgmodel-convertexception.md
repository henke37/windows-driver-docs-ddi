---
UID: NF:dbgmodel.ConvertException
title: ConvertException function (dbgmodel.h)
description: Trap and convert all exceptions coming out of a functor to an appropriate HRESULT.
ms.date: 09/28/2018
keywords: ["ConvertException function"]
ms.keywords: ConvertException
req.header: dbgmodel.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.lib: 
req.dll: 
req.irql: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
targetos: Windows
tech.root: debugger
ms.custom: RS5
f1_keywords:
 - ConvertException
 - dbgmodel/ConvertException
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - dbgmodel.h
api_name:
 - ConvertException
---

# ConvertException function


## -description

Trap and convert all exceptions coming out of a functor to an appropriate HRESULT.

C++ Specific API Helper.

## -parameters

### -param fn

An HRESULT returning functor.  If the functor throws an exception, the exception will be caught and converted to an HRESULT.

## -returns

This function returns HRESULT.

## -remarks

## -see-also

