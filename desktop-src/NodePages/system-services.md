﻿---
Description: 'This section contains the reference for the system APIs and services offered by Windows for desktop apps.'
ms.assetid: '3a3dc403-8bad-4464-9dda-361daaf8f8d3'
title: System Services
---

# System Services

This section contains the reference for the system APIs and services offered by Windows for desktop apps. These include the traditionally available services for:

-   The Component Object Model (COM).
-   File compression.
-   Dynamic-link libraries.
-   Memory management.
-   Power management.
-   The creation and coordination of multiple threads of execution..
-   The development of service applications.
-   Windows messaging.
-   Obtaining Windows system information.
-   The Help API.

## In this section



| Topic                                                                                                    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|----------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [COM](com.md)<br/>                                                                                | COM is a platform-independent, distributed, object-oriented system for creating binary software components that can interact. COM is the foundation technology for Microsoft's OLE (compound documents) and ActiveX (Internet-enabled components) technologies.<br/>                                                                                                                                                                                                                                                                                                                                                                       |
| [COM+](cos.component_services_portal)<br/>                                                         | COM+ is an evolution of Microsoft Component Object Model (COM) and Microsoft Transaction Server (MTS). COM+ builds on and extends applications written using COM, MTS, and other COM-based technologies. COM+ handles many of the resource management tasks that you previously had to program yourself, such as thread allocation and security. COM+ also makes your applications more scalable by providing thread pooling, object pooling, and just-in-time object activation. COM+ also helps protect the integrity of your data by providing transaction support, even if a transaction spans multiple databases over a network.<br/> |
| [Compression API](cmpapi._compression_portal)<br/>                                                 | The Compression API exposes the Windows MSZIP, XPRESS, XPRESS\_HUFF, and LZMS compression algorithms. This enables developers of Windows applications to manage versions, service, and extend the exposed compression algorithms.<br/>                                                                                                                                                                                                                                                                                                                                                                                                     |
| [Distributed Transaction Coordinator](8c08ffc0-5695-4b1b-a320-eaf5731524d2)<br/>                   | Guide and reference documentation for system administrators and developers using the Distributed Transaction Coordinator (DTC).<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Microsoft.Dtc.PowerShell.Diagnostics](FCC7016C-9340-4DC5-BA82-5697ECE49094)<br/>                  | Provides information about the PowerShell cmdlets provided with Microsoft Distributed Transaction Coordinator (MSDTC) for diagnostics.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [Microsoft.MsDtcManagement.Commands](FCEF063C-1082-47B2-BCAA-8B6E120BF0EF)<br/>                    | Provides information about the PowerShell cmdlets provided with Microsoft Distributed Transaction Coordinator (MSDTC) for management.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [Dynamic Link Libraries](base.dynamic_link_libraries)<br/>                                         | How to create and manage DLLs.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [Help API](helpapi.helpapi_portal)<br/>                                                            | The Help API allows the opening of help catalogs and the retrieval of help content items.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [Interprocess Communications](base.interprocess_communications)<br/>                               | How to use mailslots and pipes.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Kernel Transaction Manager](fs.kernel_transaction_manager_portal)<br/>                            | How to use transacted file and registry operations, or define transactions for other resources.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Memory Management](base.memory_management)<br/>                                                   | Core memory management services.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [MultiPoint Services](multipoint.windows_multipoint_server_portal)<br/>                            | Server role that allows multiple users to simultaneously use the same computer, such as in a classroom environment.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [Operation Recorder](oprec._operation_portal)<br/>                                                 | Operation Recorder enables applications to speed up operations that repeatedly access the same file data by exposing the Windows prefetching mechanism as a public interface.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [Power Management](base.power_management_portal)<br/>                                              | Core power management services.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Processes and Threads](base.processes_and_threads)<br/>                                           | How to create and manage processes and threads.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [Remote Desktop Services](termserv.terminal_services_portal)<br/>                                  | How to programmatically interact with Remote Desktop Services.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| [Services](base.services)<br/>                                                                     | How to create and manage services.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [Synchronization](base.synchronization)<br/>                                                       | How to coordinate multiple threads of execution.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [Windows Desktop Sharing](rdp.rdp_portal)<br/>                                                     | Windows Desktop Sharing is a multiple-party screen-sharing technology. Key scenarios include remote assistance, real-time collaboration and conferencing, and video communication.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [Windows Notification Framework](windowssetupandmigration.windows_setup_and_migration_portal)<br/> | Documents the functions (and function callback prototypes) used to detect and possibly repair an application after a setup or migration has occurred.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [Windows Subsystem for Linux](wsl.windows_subsystem_for_linux_portal)<br/>                         | Reference information for the Windows Subsystem for Linux (WSL) programming interfaces. <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [Windows System Information](base.windows_system_information)<br/>                                 | How to programmatically access the registry and key system configuration and version information.<br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |



 

 

 



