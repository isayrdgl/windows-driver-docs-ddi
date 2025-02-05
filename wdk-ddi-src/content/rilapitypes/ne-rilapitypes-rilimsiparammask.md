---
UID: NE:rilapitypes.RILIMSIPARAMMASK
title: RILIMSIPARAMMASK (rilapitypes.h)
description: "Microsoft reserves the RILIMSIPARAMMASK enumeration for internal use only. Don't use this enumeration in your code."
old-location: netvista\rilimsiparammask_2.htm
tech.root: netvista
ms.date: 02/26/2018
keywords: ["RILIMSIPARAMMASK enumeration"]
ms.keywords: RILIMSIPARAMMASK, RILIMSIPARAMMASK enumeration [Network Drivers Starting with Windows Vista], RIL_PARAM_IMSI_ALL, RIL_PARAM_IMSI_MCC, RIL_PARAM_IMSI_MNC, netvista.rilimsiparammask_2, rilapitypes/RILIMSIPARAMMASK, rilapitypes/RIL_PARAM_IMSI_ALL, rilapitypes/RIL_PARAM_IMSI_MCC, rilapitypes/RIL_PARAM_IMSI_MNC
req.header: rilapitypes.h
req.include-header: 
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
req.lib: NtosKrnl.exe
req.dll: 
req.irql: 
targetos: Windows
req.typenames: RILIMSIPARAMMASK
req.product: Windows 10 or later.
f1_keywords:
 - RILIMSIPARAMMASK
 - rilapitypes/RILIMSIPARAMMASK
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - rilapitypes.h
api_name:
 - RILIMSIPARAMMASK
---

# RILIMSIPARAMMASK enumeration (rilapitypes.h)


## -description

This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.

## -enum-fields

### -field RIL_PARAM_IMSI_IMSI

### -field RIL_PARAM_IMSI_MCC

### -field RIL_PARAM_IMSI_MNC

### -field RIL_PARAM_IMSI_ALL

## -syntax

```cpp
typedef enum _RILIMSIPARAMMASK {
  RIL_PARAM_IMSI_MCC,
  RIL_PARAM_IMSI_MNC,
  RIL_PARAM_IMSI_ALL
} RILIMSIPARAMMASK;
```

