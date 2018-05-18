---
title: IsDbReachable method of the Win32\_SessionBrokerServiceProperties class
description: Checks if the database is reachable.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 'c9774d6d-1b78-4ec1-bae2-80d41d4c9b06'
ms.prod: 'windows-server-dev'
ms.technology: 'remote-desktop-services'
ms.tgt_platform: multiple
keywords: ["IsDbReachable method Remote Desktop Services", "IsDbReachable method Remote Desktop Services , Win32_SessionBrokerServiceProperties class", "Win32_SessionBrokerServiceProperties class Remote Desktop Services , IsDbReachable method"]
topic_type:
- apiref
api_name:
- Win32_SessionBrokerServiceProperties.IsDbReachable
api_location:
- TssdWmi.dll
api_type:
- COM
---

# IsDbReachable method of the Win32\_SessionBrokerServiceProperties class

Checks if the database is reachable.

## Syntax


```mof
uint32 IsDbReachable(
  [in]�string connStringToDb,
  [in]�string connSecondaryStringToDb,
  [in]�string activeBrokerName
);
```



## Parameters

<dl> <dt>

*connStringToDb* \[in\]
</dt> <dd>

The connection string to the database.

</dd> <dt>

*connSecondaryStringToDb* \[in\]
</dt> <dd>

Secondary connection string to the central database.

**Windows Server�2012�R2 and Windows Server�2012:** This parameter is not available before Windows Server�2016.

</dd> <dt>

*activeBrokerName* \[in\]
</dt> <dd>

Active broker name.

**Windows Server�2012�R2 and Windows Server�2012:** This parameter is not available before Windows Server�2016.

</dd> </dl>

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                              |
| Minimum supported server<br/> | Windows Server�2012<br/>                                                         |
| Namespace<br/>                | Root\\CIMv2\\TerminalServices<br/>                                               |
| MOF<br/>                      | <dl> <dt>TssdWmi.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TssdWmi.dll</dt> </dl> |



## See also

<dl> <dt>

[**Win32\_SessionBrokerServiceProperties**](win32-sessionbrokerserviceproperties.md)
</dt> </dl>

�

�




