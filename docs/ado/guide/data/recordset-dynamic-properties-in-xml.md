---
title: Recordset dynamischen Eigenschaften in XML | Microsoft Docs
ms.prod: sql
ms.prod_service: connectivity
ms.component: ado
ms.technology: connectivity
ms.custom: ''
ms.date: 01/19/2017
ms.reviewer: ''
ms.suite: sql
ms.tgt_pltfrm: ''
ms.topic: conceptual
helpviewer_keywords:
- Recordset dynamic properties in XML [ADO]
ms.assetid: 52f8e379-812a-4db8-9210-94458926301c
caps.latest.revision: 3
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 56ce4985fddc55b6f3e3d204623c950a13953a86
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="recordset-dynamic-properties-in-xml"></a>Recordset dynamischen Eigenschaften in XML
Die folgenden Recordset anbieterspezifische Eigenschaften (aus der Client-Cursormoduls) werden derzeit in der XML-Format gespeichert:  
  
-   Aktualisieren Sie die erneute Synchronisierung  
  
-   Eindeutige Tabelle  
  
-   Eindeutiges Schema  
  
-   Eindeutige Katalog  
  
-   Resync-Befehl  
  
-   IRowsetChange  
  
-   IRowsetUpdate  
  
-   CommandTimeout  
  
-   BatchSize  
  
-   UpdateCriteria  
  
-   Umstrukturieren von Namen  
  
-   AutoRecalc  
  
 Diese Eigenschaften werden als Attribute der Elementdefinition für das Recordset persistent gespeichert wird, im Schemaabschnitt gespeichert. Diese Attribute sind in der Rowset-Schemanamespace definiert und müssen haben das Präfix "Rs:".  
  
## <a name="see-also"></a>Siehe auch  
 [Beibehalten von Datensätzen im XML-Format](../../../ado/guide/data/persisting-records-in-xml-format.md)
