---
title: Sys.dm_pdw_network_credentials (Transact-SQL) | Microsoft Docs
ms.custom: ''
ms.date: 03/07/2017
ms.prod: sql
ms.prod_service: pdw
ms.reviewer: ''
ms.suite: sql
ms.technology: system-objects
ms.tgt_pltfrm: ''
ms.topic: language-reference
dev_langs:
- TSQL
ms.assetid: d4fee3ad-6285-4ea5-8513-5e6eb617abb0
caps.latest.revision: 8
author: stevestein
ms.author: sstein
manager: craigg
monikerRange: '>= aps-pdw-2016 || = sqlallproducts-allversions'
ms.openlocfilehash: e7b4534410eabf1186b115c07fef8a8d79960938
ms.sourcegitcommit: 7019ac41524bdf783ea2c129c17b54581951b515
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/23/2018
---
# <a name="sysdmpdwnetworkcredentials-transact-sql"></a>Sys.dm_pdw_network_credentials (Transact-SQL)
[!INCLUDE[tsql-appliesto-xxxxxx-xxxx-xxxx-pdw-md](../../includes/tsql-appliesto-xxxxxx-xxxx-xxxx-pdw-md.md)]

  Gibt eine Liste aller Netzwerkanmeldeinformationen, in gespeichert der [!INCLUDE[ssPDW](../../includes/sspdw-md.md)] Appliance für alle Zielserver. Für den Knoten, und jeder Serverknoten sind die Ergebnisse aufgeführt.  
  
|Spaltenname|Datentyp|Description|  
|-----------------|---------------|-----------------|  
|pdw_node_id|**int**|Eindeutige numerische Id, die dem Knoten zugeordnet.|  
|target_server_name|**nvarchar(32)**|IP-Adresse des Zielservers, [!INCLUDE[ssPDW](../../includes/sspdw-md.md)] greifen mithilfe der Anmeldeinformationen für Benutzername und Kennwort.|  
|username|**nvarchar(32)**|Der Benutzername für die das Kennwort gespeichert wird.|  
|last_modified|**datetime**|DateTime-Wert des letzten Vorgangs, der die Anmeldeinformationen geändert.|  
  
## <a name="permissions"></a>Berechtigungen  
 Erfordert die VIEW SERVER STATE.  
  
## <a name="general-remarks"></a>Allgemeine Hinweise  
 Der Schlüssel für diese dynamische verwaltungssicht ist *Pdw_node_id* plus *Target_server_name*.  
  
## <a name="see-also"></a>Siehe auch  
 [SQL Datawarehouse und Parallel Data Warehouse-dynamische Verwaltungssichten &#40;Transact-SQL&#41;](../../relational-databases/system-dynamic-management-views/sql-and-parallel-data-warehouse-dynamic-management-views.md)  
  
  
