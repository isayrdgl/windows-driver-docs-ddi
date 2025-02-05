---
UID: NE:ntddndis._NDIS_PM_WAKE_REASON_TYPE
title: _NDIS_PM_WAKE_REASON_TYPE (ntddndis.h)
description: The NDIS_PM_WAKE_REASON_TYPE enumeration identifies the type of wake-up event that was generated by the network adapter.
old-location: netvista\ndis_pm_wake_reason_type.htm
tech.root: netvista
ms.date: 12/02/2021
keywords: ["NDIS_PM_WAKE_REASON_TYPE enumeration"]
ms.keywords: "*PNDIS_PM_WAKE_REASON_TYPE, NDIS_PM_WAKE_REASON_TYPE, NDIS_PM_WAKE_REASON_TYPE enumeration [Network Drivers Starting with Windows Vista], NdisWakeReasonMediaConnect, NdisWakeReasonMediaDisconnect, NdisWakeReasonPacket, NdisWakeReasonUnspecified, NdisWakeReasonWlan4WayHandshakeRequest, NdisWakeReasonWlanAPAssociationLost, NdisWakeReasonWlanGTKHandshakeError, NdisWakeReasonWlanNLODiscovery, NdisWakeReasonWwanRegisterState, NdisWakeReasonWwanSMSReceive, NdisWakeReasonWwanUSSDReceive, PNDIS_PM_WAKE_REASON_TYPE, PNDIS_PM_WAKE_REASON_TYPE enumeration pointer [Network Drivers Starting with Windows Vista], _NDIS_PM_WAKE_REASON_TYPE, netvista.ndis_pm_wake_reason_type, ntddndis/NDIS_PM_WAKE_REASON_TYPE, ntddndis/NdisWakeReasonMediaConnect, ntddndis/NdisWakeReasonMediaDisconnect, ntddndis/NdisWakeReasonPacket, ntddndis/NdisWakeReasonUnspecified, ntddndis/NdisWakeReasonWlan4WayHandshakeRequest, ntddndis/NdisWakeReasonWlanAPAssociationLost, ntddndis/NdisWakeReasonWlanGTKHandshakeError, ntddndis/NdisWakeReasonWlanNLODiscovery, ntddndis/NdisWakeReasonWwanRegisterState, ntddndis/NdisWakeReasonWwanSMSReceive, ntddndis/NdisWakeReasonWwanUSSDReceive, ntddndis/PNDIS_PM_WAKE_REASON_TYPE"
req.header: ntddndis.h
req.include-header: Ntddndis.h
req.target-type: Windows
req.target-min-winverclnt: Supported in NDIS 6.30 and later.
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
req.typenames: NDIS_PM_WAKE_REASON_TYPE, *PNDIS_PM_WAKE_REASON_TYPE
f1_keywords:
 - _NDIS_PM_WAKE_REASON_TYPE
 - ntddndis/_NDIS_PM_WAKE_REASON_TYPE
 - PNDIS_PM_WAKE_REASON_TYPE
 - ntddndis/PNDIS_PM_WAKE_REASON_TYPE
 - NDIS_PM_WAKE_REASON_TYPE
 - ntddndis/NDIS_PM_WAKE_REASON_TYPE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ntddndis.h
api_name:
 - _NDIS_PM_WAKE_REASON_TYPE
 - PNDIS_PM_WAKE_REASON_TYPE
 - NDIS_PM_WAKE_REASON_TYPE
---

# _NDIS_PM_WAKE_REASON_TYPE enumeration


## -description

The <b>NDIS_PM_WAKE_REASON_TYPE</b> enumeration identifies the type of wake-up event that was generated by the network adapter.

## -enum-fields

### -field NdisWakeReasonUnspecified:0x0000

The type of wake-up event is not specified.

### -field NdisWakeReasonPacket:0x0001

The network adapter generated the wake-up event because it received a packet that matched a wake-on-LAN (WOL) pattern.

### -field NdisWakeReasonMediaDisconnect:0x0002

The network adapter generated the wake-up event because it disconnected from the network media.

### -field NdisWakeReasonMediaConnect:0x0003

The network adapter generated the wake-up event because it connected to the network media.

### -field NdisWakeReasonWlanNLODiscovery:0x1000

The 802.11 network adapter generated the wake-up event because it detected a service set identifier (SSID) that was specified through a network list offload (NLO). 

For more information about NLO, see <a href="/windows-hardware/drivers/network/wi-fi-network-list-offload">Wi-Fi Network List Offload</a>.

### -field NdisWakeReasonWlanAPAssociationLost:0x1001

The 802.11 network adapter generated the wake-up event because it became disassociated with the access point (AP).

### -field NdisWakeReasonWlanGTKHandshakeError:0x1002

The 802.11 network adapter generated the wake-up event because it encountered an error during the IEEE 802.11i RSN group transient key (GTK) handshake with the AP.

### -field NdisWakeReasonWlan4WayHandshakeRequest0x1003

The 802.11 network adapter generated the wake-up event because it received the first frame of the IEEE 802.11i RSN 4-way handshake with the AP. This handshake is performed when the adapter authenticates with the AP.

### -field NdisWakeReasonWwanRegisterState:0x2000

The mobile broadband (MB) network adapter generated the wake-up event because its registration state to the MB Service has changed.

### -field NdisWakeReasonWwanSMSReceive:0x2001

The mobile broadband (MB) network adapter generated the wake-up event because the MB Service has to be notified about the receipt of a Short Message Service (SMS) message. The adapter generates this wake-up event either after the completion of a previously-issued <a href="/windows-hardware/drivers/network/oid-wwan-sms-read">OID_WWAN_SMS_READ</a> query request, or the arrival of a new class-0 (flash/alert) message from the network provider as an event notification.

### -field NdisWakeReasonWwanUSSDReceive:0x2002

The mobile broadband (MB) network adapter generated the wake-up event because it received an Unstructured Supplementary Service Data (USSD) message.

### -field NdisWakeReasonWwanPacketState:0x2004

The mobile broadband (MB) network adapter generated the wake-up event because of a packet state change.

### -field NdisWakeReasonWwanUiccChange:0x2005

The mobile broadband (MB) network adapter generated the wake-up event because the SIM card state changed.

## -remarks

The  <b>WakeReason</b> member of the <a href="/windows-hardware/drivers/ddi/ntddndis/ns-ntddndis-_ndis_pm_wake_reason">NDIS_PM_WAKE_REASON</a> structure contains an <b>NDIS_PM_WAKE_REASON_TYPE</b> enumeration value.

## -see-also

<a href="/windows-hardware/drivers/ddi/ntddndis/ns-ntddndis-_ndis_pm_wake_reason">NDIS_PM_WAKE_REASON</a>

