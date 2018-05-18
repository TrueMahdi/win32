﻿---
Description: 'Represents the context for the activation of a UWP device app for printers.'
ms.assetid: 'DD0B5E6F-8E16-48E1-967B-D188535E1320'
title: IPrinterExtensionContext interface
---

# IPrinterExtensionContext interface

Represents the context for the activation of a UWP device app for printers.

## Members

The **IPrinterExtensionContext** interface inherits from the [**IDispatch**](ebbff4bc-36b2-4861-9efa-ffa45e013eb5) interface. **IPrinterExtensionContext** also has these types of members:

-   [Properties](#properties)

### Properties

The **IPrinterExtensionContext** interface has these properties.



| Property                                                                           | Access type          | Description                                                                            |
|:-----------------------------------------------------------------------------------|:---------------------|:---------------------------------------------------------------------------------------|
| [**DriverProperties**](iprinterextensioncontext-driverproperties.md)<br/>   | Read-only<br/> | Gets the driver property bag.<br/>                                               |
| [**PrinterQueue**](iprinterextensioncontext-printerqueue.md)<br/>           | Read-only<br/> | Gets the queue for the printer.<br/>                                             |
| [**PrintSchemaTicket**](iprinterextensioncontext-printschematicket.md)<br/> | Read-only<br/> | Gets the print ticket that is appropriate for the queue and the activation.<br/> |
| [**UserProperties**](iprinterextensioncontext-userproperties.md)<br/>       | Read-only<br/> | Gets the user property bag for this app.<br/>                                    |



 

## Requirements



|                                     |                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8<br/>                                                                          |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                                |
| Header<br/>                   | <dl> <dt>Printerextension.h</dt> </dl> |



## See also

<dl> <dt>

[**IPrinterExtensionContextCollection**](iprinterextensioncontextcollection.md)
</dt> <dt>

[**IPrinterExtensionContextCollection::Count**](iprinterextensioncontextcollection-count.md)
</dt> <dt>

[**IPrinterExtensionContextCollection::GetAt**](iprinterextensioncontextcollection-getat.md)
</dt> <dt>

[**IPrinterExtensionEvent::OnPrinterQueuesEnumerated**](iprinterextensionevent-onprinterqueuesenumerated.md)
</dt> <dt>

[V4 Printer Driver Property Bags](print.v4_driver_property_bags)
</dt> </dl>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bprint\print%5D:%20IPrinterExtensionContext%20interface%20%20RELEASE:%20%285/12/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




