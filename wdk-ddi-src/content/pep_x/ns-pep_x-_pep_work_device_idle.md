---
UID: NS:pep_x._PEP_WORK_DEVICE_IDLE
title: _PEP_WORK_DEVICE_IDLE (pep_x.h)
description: The PEP_WORK_DEVICE_IDLE structure indicates whether to ignore the idle time-out for the specified device.
old-location: kernel\pep_work_device_idle.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["PEP_WORK_DEVICE_IDLE structure"]
ms.keywords: "*PPEP_WORK_DEVICE_IDLE, PEP_WORK_DEVICE_IDLE, PEP_WORK_DEVICE_IDLE structure [Kernel-Mode Driver Architecture], PPEP_WORK_DEVICE_IDLE, PPEP_WORK_DEVICE_IDLE structure pointer [Kernel-Mode Driver Architecture], _PEP_WORK_DEVICE_IDLE, kernel.pep_work_device_idle, pep_x/PEP_WORK_DEVICE_IDLE, pep_x/PPEP_WORK_DEVICE_IDLE"
req.header: pep_x.h
req.include-header: Pepfx.h
req.target-type: Windows
req.target-min-winverclnt: Supported starting with Windows 10.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: PEP_WORK_DEVICE_IDLE, *PPEP_WORK_DEVICE_IDLE
f1_keywords:
 - _PEP_WORK_DEVICE_IDLE
 - pep_x/_PEP_WORK_DEVICE_IDLE
 - PPEP_WORK_DEVICE_IDLE
 - pep_x/PPEP_WORK_DEVICE_IDLE
 - PEP_WORK_DEVICE_IDLE
 - pep_x/PEP_WORK_DEVICE_IDLE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - pep_x.h
api_name:
 - PEP_WORK_DEVICE_IDLE
---

# _PEP_WORK_DEVICE_IDLE structure


## -description

The <b>PEP_WORK_DEVICE_IDLE</b> structure indicates whether to ignore the idle time-out for the specified device.

## -struct-fields

### -field DeviceHandle

A handle that represents the registration of the device with the Windows <a href="/windows-hardware/drivers/kernel/overview-of-the-power-management-framework">power management framework</a> (PoFx). A POHANDLE value that represents the registration of the device with PoFx. The platform extension plug-in (PEP) previously received this handle from PoFx during the <a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_register_crashdump_device">PEP_DPM_REGISTER_DEVICE</a> notification that informed the PEP that the device's driver stack registered the device with PoFx.

### -field IgnoreIdleTimeout

Whether to ignore the idle time-out. Set to TRUE to tell the operating system to ignore the idle time-out for this device. Set to FALSE to tell the operating system to call the device driver's <a href="/windows-hardware/drivers/ddi/wdm/nc-wdm-po_fx_device_power_not_required_callback">DevicePowerNotRequiredCallback</a> callback routine after the device remains idle for the designated time-out interval. For more information, see <a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-pofxsetdeviceidletimeout">PoFxSetDeviceIdleTimeout</a>.

## -remarks

The <b>DeviceIdle</b> member of the <a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_work_information">PEP_WORK_INFORMATION</a> structure is a <b>PEP_WORK_DEVICE_IDLE</b> structure.

## -see-also

<a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_register_crashdump_device">PEP_DPM_REGISTER_DEVICE</a>



<a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_work_information">PEP_WORK_INFORMATION</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-pofxsetdeviceidletimeout">PoFxSetDeviceIdleTimeout</a>
