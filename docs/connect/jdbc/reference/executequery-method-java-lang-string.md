---
title: ExecuteQuery-Methode (java.lang.String) | Microsoft Docs
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
- SQLServerPreparedStatement.executeQuery (java.lang.String)
apilocation:
- sqljdbc.jar
apitype: Assembly
ms.assetid: 610205c2-6bcd-426c-ad6f-9682551efdec
caps.latest.revision: 11
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 5c336fa7b11186dfbc94f35daef99853175ffc86
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="executequery-method-javalangstring"></a>executeQuery-Methode (java.lang.String)
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Führt die angegebene SQL-Anweisung und gibt ein einzelnes [SQLServerResultSet](../../../connect/jdbc/reference/sqlserverresultset-class.md) Objekt.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
public final java.sql.ResultSet executeQuery(java.lang.String sql)  
```  
  
#### <a name="parameters"></a>Parameter  
 *sql*  
  
 Ein **Zeichenfolge** , die eine SQL-Anweisung enthält.  
  
## <a name="return-value"></a>Rückgabewert  
 Ein SQLServerResultSet-Objekt.  
  
## <a name="exceptions"></a>Ausnahmen  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## <a name="remarks"></a>Hinweise  
 Diese ExecuteQuery-Methode wird von der ExecuteQuery-Methode in der java.sql.Statement-Schnittstelle angegeben.  
  
 Diese Methode überschreibt die [ExecuteQuery](../../../connect/jdbc/reference/executequery-method-sqlserverstatement.md) -Methode, die in gefunden wurde die [SQLServerStatement](../../../connect/jdbc/reference/sqlserverstatement-class.md) Klasse.  
  
 Beim Aufrufen dieser Methode führt eine Ausnahme ausgelöst, da die SQL-Anweisung für die SQLServerPreparedStatement-Objekt angegeben wird, wenn das Objekt erstellt wird.  
  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md) wird ausgelöst, wenn die angegebene SQL-Anweisung etwas anderes als ein einzelnes erzeugt [SQLServerResultSet](../../../connect/jdbc/reference/sqlserverresultset-class.md) Objekt.  
  
## <a name="see-also"></a>Siehe auch  
 [ExecuteQuery-Methode &#40;sqlserverpreparedstatement-Klasse&#41;](../../../connect/jdbc/reference/executequery-method-sqlserverpreparedstatement.md)   
 [SQLServerPreparedStatement-Elemente](../../../connect/jdbc/reference/sqlserverpreparedstatement-members.md)   
 [SQLServerPreparedStatement-Klasse](../../../connect/jdbc/reference/sqlserverpreparedstatement-class.md)  
  
  
