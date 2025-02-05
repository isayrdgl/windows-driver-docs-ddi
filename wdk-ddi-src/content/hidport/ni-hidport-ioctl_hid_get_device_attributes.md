---
UID: NI:hidport.IOCTL_HID_GET_DEVICE_ATTRIBUTES
title: IOCTL_HID_GET_DEVICE_ATTRIBUTES (hidport.h)
description: The IOCTL_HID_GET_DEVICE_ATTRIBUTES request obtains a HIDClass device's attributes in a HID_DEVICE_ATTRIBUTES structure.
old-location: hid\ioctl_hid_get_device_attributes.htm
tech.root: hid
ms.date: 04/30/2018
keywords: ["IOCTL_HID_GET_DEVICE_ATTRIBUTES IOCTL"]
ms.keywords: IOCTL_HID_GET_DEVICE_ATTRIBUTES, IOCTL_HID_GET_DEVICE_ATTRIBUTES control, IOCTL_HID_GET_DEVICE_ATTRIBUTES control code [Human Input Devices], hid.ioctl_hid_get_device_attributes, hidioreq_417c2e10-9ca8-4a9f-8a30-1ff401b65b13.xml, hidport/IOCTL_HID_GET_DEVICE_ATTRIBUTES
req.header: hidport.h
req.include-header: Hidport.h
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
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - IOCTL_HID_GET_DEVICE_ATTRIBUTES
 - hidport/IOCTL_HID_GET_DEVICE_ATTRIBUTES
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - hidport.h
api_name:
 - IOCTL_HID_GET_DEVICE_ATTRIBUTES
---

# IOCTL_HID_GET_DEVICE_ATTRIBUTES IOCTL


## -description

The IOCTL_HID_GET_DEVICE_ATTRIBUTES request obtains a HIDClass device's attributes in a <a href="/windows-hardware/drivers/ddi/hidport/ns-hidport-_hid_device_attributes">HID_DEVICE_ATTRIBUTES</a> structure.

For general information about HIDClass devices, see <a href="/windows-hardware/drivers/hid/hid-collections">HID Collections</a>.

## -ioctlparameters

### -input-buffer

<b>Parameters.DeviceIoControl.OutputBufferLength</b> contains the length, in bytes, of the HID class driver's buffer located at <b>Irp->UserBuffer</b>.

### -input-buffer-length

The size, in bytes, of the buffer must be greater than or equal to the size, in bytes, of a HID_DEVICE_ATTRIBUTES structure.

### -output-buffer

The HID minidriver returns the device attributes in a HID_DEVICE_ATTRIBUTES structure at <b>Irp->UserBuffer</b>.

### -output-buffer-length

The size of a HID_DEVICE_ATTRIBUTES structure.

### -in-out-buffer

### -inout-buffer-length

### -status-block

The HID minidriver sets the following fields of <b>Irp->IoStatus</b>:

<ul>
<li>
<b>Information</b> is set to the number of bytes transferred from the device.

</li>
<li>
<b>Status</b> is set to STATUS_SUCCESS if the transfer completed without error. Otherwise, it is set to an appropriate NTSTATUS error code.

</li>
</ul>

## -see-also

<a href="/windows-hardware/drivers/ddi/hidport/ns-hidport-_hid_device_attributes">HID_DEVICE_ATTRIBUTES</a>



<a href="/windows-hardware/drivers/ddi/hidport/ni-hidport-ioctl_hid_get_device_descriptor">IOCTL_HID_GET_DEVICE_DESCRIPTOR</a>
