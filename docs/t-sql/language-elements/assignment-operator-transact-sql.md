---
title: = (Zuweisungsoperator) (Transact-SQL) | Microsoft-Dokumentation
ms.custom: ''
ms.date: 03/14/2017
ms.prod: sql
ms.prod_service: database-engine, sql-database, sql-data-warehouse, pdw
ms.component: t-sql|language-elements
ms.reviewer: ''
ms.suite: sql
ms.technology: t-sql
ms.tgt_pltfrm: ''
ms.topic: language-reference
dev_langs:
- TSQL
helpviewer_keywords:
- operators [Transact-SQL], assignment
- assignment operators [Transact-SQL]
- headings [SQL Server columns]
- relationships [SQL Server], assignment operators
- column headings [SQL Server]
ms.assetid: c3040db6-21d6-40ac-a783-82c98ec006cc
caps.latest.revision: 29
author: douglaslMS
ms.author: douglasl
manager: craigg
monikerRange: '>= aps-pdw-2016 || = azuresqldb-current || = azure-sqldw-latest || >= sql-server-2016 || = sqlallproducts-allversions'
ms.openlocfilehash: 51e8c7fb8f85eabe4f4e8fd30da6c95bf548e60f
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="-assignment-operator-transact-sql"></a>= (Zuweisungsoperator) (Transact-SQL)
[!INCLUDE[tsql-appliesto-ss2012-all_md](../../includes/tsql-appliesto-ss2012-all-md.md)]

  Das Gleichheitszeichen (=) ist der einzige Zuweisungsoperator von [!INCLUDE[tsql](../../includes/tsql-md.md)]. Im folgenden Beispiel wird die `@MyCounter`-Variable erstellt. Anschließend legt der Zuweisungsoperator `@MyCounter` auf einen Wert fest, der von einem Ausdruck zurückgegeben wird.  
  
```  
DECLARE @MyCounter INT;  
SET @MyCounter = 1;  
```  
  
 Mit dem Zuweisungsoperator kann auch eine Beziehung zwischen einer Spaltenüberschrift und dem Ausdruck hergestellt werden, der die Werte für die Spalte definiert. Im folgenden Beispiel werden die Spaltenüberschriften `FirstColumnHeading` und `SecondColumnHeading` angezeigt. Die Zeichenfolge `xyz` wird unter der Spaltenüberschrift `FirstColumnHeading` für alle Zeilen angezeigt. Jede Produkt-ID aus der `Product`-Tabelle wird unter der Spaltenüberschrift `SecondColumnHeading` aufgelistet.  
  
```  
-- Uses AdventureWorks  
  
SELECT FirstColumnHeading = 'xyz',  
       SecondColumnHeading = ProductID  
FROM Production.Product;  
GO  
```  
  
## <a name="see-also"></a>Weitere Informationen finden Sie unter  
 [Operatoren &#40;Transact-SQL&#41;](../../t-sql/language-elements/operators-transact-sql.md)   
 [Verbundoperatoren &#40;Transact-SQL&#41;](../../t-sql/language-elements/compound-operators-transact-sql.md)   
 [Ausdrücke &#40;Transact-SQL&#41;](../../t-sql/language-elements/expressions-transact-sql.md)  
  
  
