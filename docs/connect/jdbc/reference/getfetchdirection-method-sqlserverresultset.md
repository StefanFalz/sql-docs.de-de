---
title: GetFetchDirection-Methode (SQLServerResultSet) | Microsoft Docs
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
- SQLServerResultSet.getFetchDirection
apilocation:
- sqljdbc.jar
apitype: Assembly
ms.assetid: 5ab385c2-e18c-4b75-ac2d-2402af5c52a5
caps.latest.revision: 10
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 594d59adc33decf67118fd680d6aeaa32a38ebe7
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="getfetchdirection-method-sqlserverresultset"></a>GetFetchDirection-Methode (SQLServerResultSet)
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Ruft die abrufrichtung für dieses [SQLServerResultSet](../../../connect/jdbc/reference/sqlserverresultset-class.md) Objekt.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
public int getFetchDirection()  
```  
  
## <a name="return-value"></a>Rückgabewert  
 Ein **Int** , der die aktuellen abrufrichtung angibt.  
  
## <a name="exceptions"></a>Ausnahmen  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## <a name="remarks"></a>Hinweise  
 Diese GetFetchDirection-Methode wird von der GetFetchDirection-Methode in der java.sql.ResultSet-Schnittstelle angegeben.  
  
 Diese Methode gibt FETCH_FORWARD für Vorwärtscursor, die letzte Einstellung vorgenommen, die durch einen Aufruf der [SetFetchDirection](../../../connect/jdbc/reference/setfetchdirection-method-sqlserverresultset.md) Methode für andere Cursortypen und "fetch_unknown" können diese Cursortypen wird zurückgegeben werden, wenn der SetFetchDirection-Methode wurde nie aufgerufen.  
  
## <a name="see-also"></a>Siehe auch  
 [SQLServerResultSet-Elemente](../../../connect/jdbc/reference/sqlserverresultset-members.md)   
 [SQLServerResultSet-Klasse](../../../connect/jdbc/reference/sqlserverresultset-class.md)  
  
  
