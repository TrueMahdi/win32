﻿---
Description: 'The Item property retrieves an extension, by index, from the collection. This is the default property.'
ms.assetid: '0242dc14-abf2-49df-b75a-9005b2376cfc'
title: 'Extensions.Item property'
---

# Extensions.Item property

\[CAPICOM is a 32-bit only component that is available for use in the following operating systems: Windows Server 2008, Windows Vista, and Windows XP. Instead, use the [**X509ExtensionCollection Class**](T:System.Security.Cryptography.X509Certificates.X509ExtensionCollection) in the [**System.Security.Cryptography.X509Certificates**](frlrfSystemSecurityCryptographyX509Certificates) namespace.\]

The **Item** property retrieves an extension, by index, from the collection. This is the default property.

## Syntax


```VB
Extensions.Item( _
  ByVal Index _
) As Variant
```



## Property value

An [**Extension**](extension.md) object that represents the indexed certificate extension of the collection.

## Requirements



|                                  |                                                                                        |
|----------------------------------|----------------------------------------------------------------------------------------|
| End of client support<br/> | Windows Vista<br/>                                                               |
| End of server support<br/> | Windows Server 2008<br/>                                                         |
| Redistributable<br/>       | CAPICOM 2.0 or later on Windows Server 2003 and Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



## See also

<dl> <dt>

[**Extensions**](extensions.md)
</dt> </dl>

 

 



