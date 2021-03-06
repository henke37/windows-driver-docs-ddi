---
UID: NF:usbctypes.USBC_PD_POWER_DATA_OBJECT_GET_TYPE
title: USBC_PD_POWER_DATA_OBJECT_GET_TYPE function (usbctypes.h)
description: Retrieves the type of Power Data Object (PDO).
tech.root: usbref
ms.date: 09/30/2018
keywords: ["USBC_PD_POWER_DATA_OBJECT_GET_TYPE function"]
ms.keywords: USBC_PD_POWER_DATA_OBJECT_GET_TYPE
req.header: usbctypes.h
req.include-header: usbctypes.h
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 1.27
req.umdf-ver: N/A
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
ms.custom: RS5
f1_keywords:
 - USBC_PD_POWER_DATA_OBJECT_GET_TYPE
 - usbctypes/USBC_PD_POWER_DATA_OBJECT_GET_TYPE
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - usbctypes.h
api_name:
 - USBC_PD_POWER_DATA_OBJECT_GET_TYPE
---

# USBC_PD_POWER_DATA_OBJECT_GET_TYPE function


## -description

Retrieves the type of Power Data Object (PDO).

## -parameters

### -param Pdo

A pointer to a [**USBC_PD_POWER_DATA_OBJECT_TYPE**](ns-usbctypes-_usbc_pd_power_data_object.md) structure that contains the type of PDO.

## -returns

This function returns the type in **Common.Type** member of [**USBC_PD_POWER_DATA_OBJECT_TYPE**](ns-usbctypes-_usbc_pd_power_data_object.md).

## -remarks

## -see-also

[**USBC_PD_POWER_DATA_OBJECT_TYPE**](ns-usbctypes-_usbc_pd_power_data_object.md)

