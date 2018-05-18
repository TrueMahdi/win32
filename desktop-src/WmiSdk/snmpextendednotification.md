---
Description: 'The SnmpExtendedNotification class is the base class for any class mapped from the NOTIFICATION-TYPE macro to a CIM class by the SNMP Provider.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: '207966c1-14cf-4a47-8176-0f58838cfa1e'
ms.prod: 'windows-server-dev'
ms.technology: 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: SnmpExtendedNotification class
---

# SnmpExtendedNotification class

The **SnmpExtendedNotification** class is the base class for any class mapped from the [NOTIFICATION-TYPE](notification-type-macro.md) macro to a CIM class by the [SNMP Provider](snmp-provider.md).

> [!Note]  
> For more information about installing the provider, see [Setting up the WMI SNMP Environment](setting-up-the-wmi-snmp-environment.md).

�

The following syntax is simplified from Managed Object Format (MOF) code and includes all of its inherited properties. Properties and methods are in alphabetic order, not MOF order.

## Syntax

``` syntax
class SnmpExtendedNotification : __ExtrinsicEvent
{
  uint8� SECURITY_DESCRIPTOR[];
  uint64 TIME_CREATED;
  string AgentAddress;
  string AgentTransport;
  string AgentTransportAddress;
  string Community;
  string Identification;
  string TimeStamp;
  string AgentTransportProtocol;
};
```

## Members

The **SnmpExtendedNotification** class has these types of members:

-   [Properties](#properties)

### Properties

The **SnmpExtendedNotification** class has these properties.

<dl> <dt>

**AgentAddress**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Network address of the entity that created the notification. This is the actual address of the device. When the management entity uses SNMP over UDP, the transport address refers to an IP address. When the management entity uses SNMP over IPX, the transport address is set to **NULL**. This property is valid for SNMPv1 only.

</dd> <dt>

**AgentTransport**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Transport protocol used by the sending entity. This property is valid for SNMPv1 and SNMPv2C.

</dd> <dt>

**AgentTransportAddress**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Network address of the entity that sent the notification. This is the address of the last entity that forwarded the notification. When the management entity uses SNMP over UDP, the transport address refers to an IP address. When the management entity uses SNMP over IPX, the transport address refers to an IPX address. This property is valid for SNMPv1 and SNMPv2C.

</dd> <dt>

**AgentTransportProtocol**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The transport protocol used by the sending entity.

</dd> <dt>

**Community**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Community name associated with an instance of the PDU. The community name authenticates the originator of the PDU. This property is valid for both SNMPv1 and SNMPv2C.

</dd> <dt>

**Identification**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **textual\_convention** ("OBJECTIDENTIFIER"), **encoding** ("OBJECTIDENTIFIER"), **object\_syntax** ("OBJECTIDENTIFIER"), **object\_identifier** ("1.3.6.1.6.3.1.1.4.1")
</dt> </dl>

Authoritative identification of this notification. Maps directly to the MIB entry SnmpTrapOID variable binding. This property is valid for SNMPv2C only.

</dd> <dt>

**SECURITY\_DESCRIPTOR**
</dt> <dd> <dl> <dt>

Data type: **uint8** array
</dt> <dt>

Access type: Read-only
</dt> </dl>

Descriptor used by the event provider to determine which users can receive the event. This property is inherited from [**\_\_Event**](--event.md). For more information about constants used to set this security descriptor, see [WMI Security Constants](wmi-security-constants.md).

</dd> <dt>

**TIME\_CREATED**
</dt> <dd> <dl> <dt>

Data type: **uint64**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Unique value that indicates the time at which the event was generated. This is a 64-bit value that represents the number of 100-nanosecond intervals after January 1, 1601. The information is in the Coordinated Universal Times (UTC) format. This property is inherited from [**\_\_Event**](--event.md).

For more information about using **uint64** values in scripts, see [Scripting in WMI](https://msdn.microsoft.com/library/aa389763).

</dd> <dt>

**TimeStamp**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **textual\_convention** ("TimeTicks"), **encoding** ("TimeTicks"), **object\_syntax** ("TimeTicks"), **object\_identifier** ("1.3.6.1.2.1.1.3")
</dt> </dl>

Time in hundredths of a second since the network management portion of the agent was last re-initialized. This maps to the MIB variable sysUptime.0, which is of type **INTEGER32**. This property maps to the CIM class property **TimeStamp**, which is of type **uint32**. This property is valid for SNMPv2C only.

</dd> </dl>

## Remarks

A [NOTIFICATION-TYPE](notification-type-macro.md) macro that contains references to an [OBJECT-TYPE](object-type-macro.md) macro named **TimeStamp** or **Identification** causes a mapping conflict. If this conflict occurs, the required properties take precedence and the conflicting references must be renamed.

A [NOTIFICATION-TYPE](notification-type-macro.md) macro that contains references to an [OBJECT-TYPE](object-type-macro.md) macro named **Community** causes a mapping conflict. If this conflict occurs, the required properties take precedence and the conflicting references must be renamed.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server�2008<br/>                                                          |
| Namespace<br/>                | Root\\snmp\\SMIR<br/>                                                             |
| MOF<br/>                      | <dl> <dt>SnmpSmiR.mof</dt> </dl> |



## See also

<dl> <dt>

[**\_\_ExtrinsicEvent**](--extrinsicevent.md)
</dt> <dt>

[NOTIFICATION-TYPE Macro](notification-type-macro.md)
</dt> </dl>

�

�



