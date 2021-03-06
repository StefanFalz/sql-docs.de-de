---
title: Syscollector_execution_stats (Transact-SQL) | Microsoft Docs
ms.custom: ''
ms.date: 06/10/2016
ms.prod: sql
ms.prod_service: database-engine
ms.component: system-catalog-views
ms.reviewer: ''
ms.suite: sql
ms.technology: system-objects
ms.tgt_pltfrm: ''
ms.topic: language-reference
f1_keywords:
- syscollector_execution_stats
- syscollector_execution_stats_TSQL
dev_langs:
- TSQL
helpviewer_keywords:
- syscollector_execution_stats view
- data collector view
ms.assetid: 23e35ac5-fbbf-4922-970c-f4fac44c1263
caps.latest.revision: 17
author: stevestein
ms.author: sstein
manager: craigg
ms.openlocfilehash: 74fef0f1da7d6ec8d1a66525e3b985c61fe52991
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="syscollectorexecutionstats-transact-sql"></a>syscollector_execution_stats (Transact-SQL)
[!INCLUDE[tsql-appliesto-ss2008-xxxx-xxxx-xxx-md](../../includes/tsql-appliesto-ss2008-xxxx-xxxx-xxx-md.md)]

  Stellt Informationen zur Taskausführung für einen Sammlungssatz oder ein Paket bereit.  
  
|Spaltenname|Datentyp|Description|  
|-----------------|---------------|-----------------|  
|**log_id**|**bigint**|Identifiziert jede Sammlungssatzausführung. Wird verwendet, um diese Sicht mit anderen ausführlichen Protokollen zu verknüpfen. Lässt keine NULL-Werte zu.|  
|**task_name**|**nvarchar(128)**|Der Name des Sammlungssatz- oder Pakettasks, auf den sich diese Informationen beziehen. Lässt keine NULL-Werte zu.|  
|**execution_row_count_in**|**int**|Anzahl der Zeilen, die zu Beginn des Datenflusses verarbeitet wurden. Lässt NULL-Werte zu.|  
|**execution_row_count_out**|**int**|Anzahl der Zeilen, die am Ende des Datenflusses verarbeitet wurden. Lässt NULL-Werte zu.|  
|**execution_row_count_errors**|**int**|Anzahl der Zeilen, bei denen während des Datenflusses ein Fehler aufgetreten ist. Lässt NULL-Werte zu.|  
|**execution_time_ms**|**int**|Die für den Abschluss des Tasks erforderliche Zeit in Millisekunden. Lässt NULL-Werte zu.|  
|**log_time**|**datetime**|Der Zeitpunkt, zu dem diese Informationen protokolliert wurden. Lässt keine NULL-Werte zu.|  
  
## <a name="permissions"></a>Berechtigungen  
 Erfordert die SELECT-Berechtigung für **dc_operator**.  
  
## <a name="see-also"></a>Siehe auch  
 [Gespeicherte Prozeduren für den Datensammler &#40;Transact-SQL&#41;](../../relational-databases/system-stored-procedures/data-collector-stored-procedures-transact-sql.md)   
 [Sichten des Datensammlers &#40;Transact-SQL&#41;](../../relational-databases/system-catalog-views/data-collector-views-transact-sql.md)   
 [Datensammlung](../../relational-databases/data-collection/data-collection.md)  
  
  
