---
UID: NE:checksumtypes._NET_PACKET_RX_CHECKSUM_EVALUATION
title: NET_PACKET_RX_CHECKSUM_EVALUATION (checksumtypes.h)
description: The NET_PACKET_RX_CHECKSUM_EVALUATION enumeration specifies checksum evaluation flags for a NET_PACKET_CHECKSUM structure during packet reception.
tech.root: netvista
ms.date: 03/30/2022
keywords: ["NET_PACKET_RX_CHECKSUM_EVALUATION enumeration"]
ms.keywords: NET_PACKET_RX_CHECKSUM_EVALUATION, NET_PACKET_RX_CHECKSUM_EVALUATION,
req.header: checksumtypes.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.max-support: 
req.typenames: NET_PACKET_RX_CHECKSUM_EVALUATION
targetos: Windows
ms.custom: Vb
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - checksumtypes.h
api_name:
 - _NET_PACKET_RX_CHECKSUM_EVALUATION
 - NET_PACKET_RX_CHECKSUM_EVALUATION
product:
 - Windows
f1_keywords:
 - _NET_PACKET_RX_CHECKSUM_EVALUATION
 - checksumtypes/_NET_PACKET_RX_CHECKSUM_EVALUATION
 - NET_PACKET_RX_CHECKSUM_EVALUATION
 - checksumtypes/NET_PACKET_RX_CHECKSUM_EVALUATION
---

# NET_PACKET_RX_CHECKSUM_EVALUATION enumeration


## -description

The **NET_PACKET_RX_CHECKSUM_EVALUATION** enumeration specifies checksum evaluation flags for a [**NET_PACKET_CHECKSUM**](../checksumtypes/ns-checksumtypes-_net_packet_checksum.md) structure during packet reception.

## -enum-fields

### -field NetPacketRxChecksumEvaluationNotChecked:0 

The default value for this enumeration. Indicates that the checksum will be validated in software further up in the networking stack.

### -field NetPacketRxChecksumEvaluationValid:1 

Indicates the hardware determined that the checksum value is correct.

### -field NetPacketRxChecksumEvaluationInvalid:2 

Indicates the hardware determined that the checksum value is incorrect.

## -remarks

## -see-also

[**NET_PACKET_CHECKSUM**](../checksumtypes/ns-checksumtypes-_net_packet_checksum.md)

