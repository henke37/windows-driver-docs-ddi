---
UID: NS:miniport._PCI_EXPRESS_SEC_AER_CAPABILITIES
title: "_PCI_EXPRESS_SEC_AER_CAPABILITIES"
author: windows-driver-content
description: The PCI_EXPRESS_SEC_AER_CAPABILITIES structure describes a PCI Express (PCIe) secondary error capabilities and control register of a PCIe advanced error reporting capability structure.
old-location: pci\pci_express_sec_aer_capabilities.htm
old-project: PCI
ms.assetid: fdfc0157-699e-4927-8186-b76b2e2bbda1
ms.author: windowsdriverdev
ms.date: 2/24/2018
ms.keywords: "*PPCI_EXPRESS_SEC_AER_CAPABILITIES, PCI.pci_express_sec_aer_capabilities, PCI_EXPRESS_SEC_AER_CAPABILITIES, PCI_EXPRESS_SEC_AER_CAPABILITIES union [Buses], PPCI_EXPRESS_SEC_AER_CAPABILITIES, PPCI_EXPRESS_SEC_AER_CAPABILITIES union pointer [Buses], _PCI_EXPRESS_SEC_AER_CAPABILITIES, pci_struct_22bcb7f0-e690-414b-ba51-37c8783a6fad.xml, wdm/PCI_EXPRESS_SEC_AER_CAPABILITIES, wdm/PPCI_EXPRESS_SEC_AER_CAPABILITIES"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: miniport.h
req.include-header: Ntddk.h, Wdm.h, Miniport.h
req.target-type: Windows
req.target-min-winverclnt: 
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
req.irql: Any level (see Remarks section)
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	wdm.h
api_name:
-	PCI_EXPRESS_SEC_AER_CAPABILITIES
product:
- Windows
targetos: Windows
req.typenames: PCI_EXPRESS_SEC_AER_CAPABILITIES, *PPCI_EXPRESS_SEC_AER_CAPABILITIES
---

# _PCI_EXPRESS_SEC_AER_CAPABILITIES structure


## -description


The PCI_EXPRESS_SEC_AER_CAPABILITIES structure describes a PCI Express (PCIe) secondary error capabilities and control register of a PCIe advanced error reporting capability structure.


## -syntax


````
typedef union _PCI_EXPRESS_SEC_AER_CAPABILITIES {
  struct {
    ULONG SecondaryUncorrectableFirstErrorPtr  :5;
    ULONG Reserved  :27;
  };
  ULONG  AsULONG;
} PCI_EXPRESS_SEC_AER_CAPABILITIES, *PPCI_EXPRESS_SEC_AER_CAPABILITIES;
````


## -struct-fields




### -field DUMMYSTRUCTNAME

 


### -field AsULONG

A ULONG representation of the contents of the PCI_EXPRESS_SEC_AER_CAPABILITIES structure.


#### - Reserved

Reserved for system use.


#### - SecondaryUncorrectableFirstErrorPtr

The bit position of the first error that was reported in the PCIe secondary uncorrectable error status register.


## -remarks



The PCI_EXPRESS_SEC_AER_CAPABILITIES structure is available in Windows Server 2008 and later versions of Windows.

A PCI_EXPRESS_SEC_AER_CAPABILITIES structure is contained in the <a href="https://msdn.microsoft.com/library/windows/hardware/ff537458">PCI_EXPRESS_BRIDGE_AER_CAPABILITY</a> structure.




## -see-also

<a href="https://msdn.microsoft.com/library/windows/hardware/ff537458">PCI_EXPRESS_BRIDGE_AER_CAPABILITY</a>



 

 

