---
UID: NF:ntifs.PsDereferenceImpersonationToken
title: PsDereferenceImpersonationToken function (ntifs.h)
description: The PsDereferenceImpersonationToken routine decrements the reference count of an impersonation token.
old-location: ifsk\psdereferenceimpersonationtoken.htm
tech.root: ifsk
ms.date: 04/16/2018
keywords: ["PsDereferenceImpersonationToken function"]
ms.keywords: PsDereferenceImpersonationToken, PsDereferenceImpersonationToken routine [Installable File System Drivers], ifsk.psdereferenceimpersonationtoken, ntifs/PsDereferenceImpersonationToken, psref_8d62cb23-83a3-45fd-8b35-f7e38dd1548d.xml
req.header: ntifs.h
req.include-header: Ntifs.h
req.target-type: Universal
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
req.lib: NtosKrnl.lib
req.dll: NtosKrnl.exe
req.irql: < DISPATCH_LEVEL
targetos: Windows
req.typenames: 
f1_keywords:
 - PsDereferenceImpersonationToken
 - ntifs/PsDereferenceImpersonationToken
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - NtosKrnl.exe
api_name:
 - PsDereferenceImpersonationToken
---

# PsDereferenceImpersonationToken function


## -description

The <b>PsDereferenceImpersonationToken</b> routine decrements the reference count of an impersonation token.

## -parameters

### -param ImpersonationToken [in]


Pointer to the impersonation token whose reference count is to be decremented. If this is a <b>NULL</b> pointer, <b>PsDereferenceImpersonationToken</b> does nothing.

## -remarks

If the token's reference count reaches zero, the token is deleted.

For more information about security and access control, see the documentation on these topics in the Microsoft Windows SDK.

## -see-also

<a href="/windows-hardware/drivers/ddi/ntifs/nf-ntifs-psimpersonateclient">PsImpersonateClient</a>



<a href="/windows-hardware/drivers/ddi/ntifs/nf-ntifs-psreferenceimpersonationtoken">PsReferenceImpersonationToken</a>
