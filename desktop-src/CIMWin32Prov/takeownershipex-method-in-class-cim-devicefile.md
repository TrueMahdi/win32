---
Description: 'Obtains ownership of the logical device file specified in the object path. This method is an extended version of the TakeOwnerShip method and is inherited from CIM\_LogicalFile.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: '084f755a-e837-4d21-8bd2-0f63f80302fc'
ms.prod: 'windows-server-dev'
ms.technology:
- cimwin32
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: 'TakeOwnerShipEx method of the CIM\_DeviceFile class'
---

# TakeOwnerShipEx method of the CIM\_DeviceFile class

The **TakeOwnerShipEx** method obtains ownership of the logical device file specified in the object path. This method is an extended version of the [**TakeOwnerShip**](takeownership-method-in-class-cim-devicefile.md) method and is inherited from [**CIM\_LogicalFile**](cim-logicalfile.md). If the logical file is a directory, then this method acts recursively, taking ownership of all of the files and sub-directories that the directory contains.

> \[!Important\]  
> The DMTF (Distributed Management Task Force) CIM (Common Information Model) classes are the parent classes upon which WMI classes are built. WMI currently supports only the [CIM 2.x version schemas](Http://Go.Microsoft.Com/FWLink/p/?LinkID=309367).

�

This topic uses Managed Object Format (MOF) syntax. For more information about using this method, see [Calling a Method](https://msdn.microsoft.com/library/aa384832).

## Syntax


```mof
uint32 TakeOwnerShipEx(
  [out]�string REF StopFileName,
  [in]��string ����StartFileName,
  [in]��boolean ���Recursive
);
```



## Parameters

<dl> <dt>

*StopFileName* \[out\]
</dt> <dd>

String that represents the name of the file (or directory) where the method failed. This parameter is **null** if the method succeeds.

</dd> <dt>

*StartFileName* \[in\]
</dt> <dd>

String that represents the child file (or directory) to use as a starting point for this method. Typically, the *StartFileName* parameter is the *StopFileName* parameter specifying the file or directory at which an error occurred from the previous method call. If this parameter is **null**, the operation is performed on the file or directory specified in the **ExecMethod** call.

</dd> <dt>

*Recursive* \[in\]
</dt> <dd>

If **TRUE**, the method is also applied recursively to files and directories within the directory specified by the [**CIM\_DeviceFile**](cim-devicefile.md) instance. For file instances, this parameter is ignored.

</dd> </dl>

## Return value

Returns a value of 0 (zero) on success, and any other number to indicate an error.

<dl> <dt>


</dt> <dd>

0

Success.

</dd> <dt>


</dt> <dd>

2

Access denied.

</dd> <dt>


</dt> <dd>

8

Unspecified failure.

</dd> <dt>


</dt> <dd>

9

Invalid object.

</dd> <dt>


</dt> <dd>

10

Object already exists.

</dd> <dt>


</dt> <dd>

11

File system not NTFS.

</dd> <dt>


</dt> <dd>

12

Platform not Windows.

</dd> <dt>


</dt> <dd>

13

Drive not the same.

</dd> <dt>


</dt> <dd>

14

Directory not empty.

</dd> <dt>


</dt> <dd>

15

Sharing violation.

</dd> <dt>


</dt> <dd>

16

Invalid start file.

</dd> <dt>


</dt> <dd>

17

Privilege not held.

</dd> <dt>


</dt> <dd>

21

Invalid parameter.

</dd> </dl>

## Remarks

This method is currently not implemented by WMI. To use this method, you must implement it in your own provider.

This documentation is derived from the CIM class descriptions published by the DMTF. Microsoft may have made changes to correct minor errors, conform to Microsoft SDK documentation standards, or provide more information.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server�2008<br/>                                                          |
| Namespace<br/>                | Root\\CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## See also

<dl> <dt>

[CIM\_DeviceFile](takeownershipex-method-in-class-cim-devicefile.md)
</dt> <dt>

[**CIM\_DeviceFile**](cim-devicefile.md)
</dt> </dl>

�

�



