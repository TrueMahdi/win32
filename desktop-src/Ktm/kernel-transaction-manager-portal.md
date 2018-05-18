---
Description: 'Implement Transactional NTFS (TxF) and Transactional Registry (TxR). TxF allows transacted file system operations within NTFS. TxR allows transacted registry operations. Coordinate file system and registry operations with a transaction.'
ms.assetid: '2f601994-db1e-4aac-8db1-9a36c702664b'
title: Kernel Transaction Manager
---

# Kernel Transaction Manager

## Purpose

The Kernel Transaction Manager (KTM) enables the development of applications that use transactions. The transaction engine itself is within the kernel, but transactions can be developed for kernel- or user-mode transactions, and within a single host or among distributed hosts.

The KTM is used to implement Transactional NTFS (TxF) and Transactional Registry (TxR). TxF allows transacted file system operations within the NTFS file system. TxR allows transacted registry operations. KTM enables client applications to coordinate file system and registry operations with a transaction.

To develop an application that coordinates transactions with resources other than TxF or TxR, you must first develop a Win32 transaction-aware service, also called a resource manager.

Managed and COM+ applications should use their native transaction managers.

## Where applicable

KTM can be used with applications and resource managers hosted on Windows�Vista or Windows Server�2008.

## Developer audience

The KTM API is designed for use by C and C++ programmers.

## Run-time requirements

KTM is supported starting with Windows�Vista.

## In this section



| Topic                                     | Description                                                                                                       |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| [About](about-ktm.md)<br/>         | General information about transactions and the capabilities provided by KTM.<br/>                           |
| [Reference](ktm-reference.md)<br/> | Documentation for the functions, data structures, enumerations, and other programming elements of KTM.<br/> |



�

## Related topics

<dl> <dt>

[Common Log File System](https://msdn.microsoft.com/library/windows/desktop/bb986747)
</dt> <dt>

[Transactional NTFS (TxF)](https://msdn.microsoft.com/library/windows/desktop/bb968806)
</dt> <dt>

[Distributed Transaction Coordinator](http://go.microsoft.com/fwlink/p/?linkid=139572)
</dt> </dl>

�

�



