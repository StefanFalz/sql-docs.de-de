---
title: Komponenten des OLE DB-Treiber für SQLServer | Microsoft Docs
description: Komponenten des OLE DB-Treiber für SQLServer
ms.custom: ''
ms.date: 03/26/2018
ms.prod: sql
ms.prod_service: database-engine, sql-database, sql-data-warehouse, pdw
ms.component: oledb|applications
ms.reviewer: ''
ms.suite: sql
ms.technology: connectivity
ms.tgt_pltfrm: ''
ms.topic: reference
helpviewer_keywords:
- data access [OLE DB Driver for SQL Server], components
- components [OLE DB Driver for SQL Server]
- MSOLEDBSQL, about OLE DB Driver for SQL Server
author: pmasl
ms.author: Pedro.Lopes
manager: craigg
ms.openlocfilehash: 2548d1c3830611f9b9fddb556d8711ca7039b9ed
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="components-of-ole-db-driver-for-sql-server"></a>Komponenten des OLE DB-Treiber für SQLServer
[!INCLUDE[appliesto-ss-asdb-asdw-pdw-md](../../../includes/appliesto-ss-asdb-asdw-pdw-md.md)]

[!INCLUDE[Driver_OLEDB_Download](../../../includes/driver_oledb_download.md)]

  OLE DB-Treiber für SQL Server enthält die folgenden Komponenten:  

|Komponente|Description|  
|---------------|-----------------|  
|msoledbsql.dll|Die Dynamic Link Library (DLL)-Datei, die alle von der OLE DB-Treiber für SQL Server-Funktionen enthält.|  
|msoledbsqlr.rll|Die begleitende Ressourcendatei für den OLE DB-Treiber für SQL Server-Bibliothek.|   
|msoledbsql.h|Der OLE DB-Treiber für SQL Server-Headerdatei, die alle erforderlichen neuen Definitionen enthält erforderlich, um OLE DB-Treiber für SQL Server verwenden. Diese Headerdatei ersetzt die sqloledb.h-Headerdatei.<br /><br /> Hinweis: Sie können msoledbsql.h und sqloledb.h im selben Programm verweisen solange sqloledb.h zuerst definiert wird.|  
|msoledbsql.lib|Die Bibliotheksdatei benötigt für den direkten Aufruf der [OpenSqlFilestream](../../../relational-databases/blob/access-filestream-data-with-opensqlfilestream.md) -Funktion, die Teil der OLE DB-Treiber für SQL Server ist.<br /><br /> Hinweis: Wenn Sie die Datei msoledbsql.lib in Ihrem Programmcode verweisen, müssen Sie sicherstellen, dass die Datei msoledbsql.dll ist in Ihrem Systempfad sowie im Systempfad der Benutzer, die Stellen der Anwendung verwenden.|  

## <a name="see-also"></a>Siehe auch  
 [Erstellen von Anwendungen mit dem OLE DB-Treiber für SQL Server](../../oledb/applications/building-applications-with-oledb-driver-for-sql-server.md)  
