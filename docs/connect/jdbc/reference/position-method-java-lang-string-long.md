---
title: Position-Methode (java.lang.String, long) | Microsoft Docs
ms.custom: ''
ms.date: 01/19/2017
ms.prod: sql
ms.prod_service: connectivity
ms.reviewer: ''
ms.suite: sql
ms.technology: connectivity
ms.tgt_pltfrm: ''
ms.topic: conceptual
apiname:
- SQLServerClob.position (java.lang.String, long)
apilocation:
- sqljdbc.jar
apitype: Assembly
ms.assetid: 86fad8ed-375a-42e1-b40e-1fa085957a2c
caps.latest.revision: 9
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: dcc1c9342691a0f6f844d60654aabc9a6ef998da
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="position-method-javalangstring-long"></a>position-Methode (java.lang.String, long)
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Gibt die Zeichenposition der angegebenen Teilzeichenfolge im CLOB auf Grundlage der angegebenen Startposition zurück.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
public long position(java.lang.String searchstr,  
                     long start)  
```  
  
#### <a name="parameters"></a>Parameter  
 *searchstr*  
  
 Die Teilzeichenfolge, nach dem gesucht werden soll.  
  
 *start*  
  
 Die Position, an der mit der Suche begonnen wird. Die erste Position ist "1".  
  
## <a name="return-value"></a>Rückgabewert  
 Die Position, an der sich die Teilzeichenfolge befindet, oder "-1", wenn sie nicht vorhanden ist. Die erste Position ist "1".  
  
## <a name="exceptions"></a>Ausnahmen  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## <a name="remarks"></a>Hinweise  
 Diese Position-Methode wird von der Position-Methode in der java.sql.Clob-Schnittstelle angegeben.  
  
## <a name="see-also"></a>Siehe auch  
 [Position-Methode &#40;SQLServerClob&#41;](../../../connect/jdbc/reference/position-method-sqlserverclob.md)   
 [SQLServerClob-Methoden](../../../connect/jdbc/reference/sqlserverclob-methods.md)   
 [SQLServerClob-Elemente](../../../connect/jdbc/reference/sqlserverclob-members.md)   
 [SQLServerClob-Klasse](../../../connect/jdbc/reference/sqlserverclob-class.md)  
  
  
