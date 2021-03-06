---
title: SQL-Anweisungen verarbeiten | Microsoft Docs
ms.custom: ''
ms.date: 01/19/2017
ms.prod: sql
ms.prod_service: connectivity
ms.reviewer: ''
ms.suite: sql
ms.technology: connectivity
ms.tgt_pltfrm: ''
ms.topic: conceptual
helpviewer_keywords:
- ODBC cursor library [ODBC], statement processing
- SQL statements [ODBC], cursor library
- cursor library [ODBC], statement processing
ms.assetid: 54dad6a3-e86c-477b-ba7c-4e95e0385ec1
caps.latest.revision: 8
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 603cb680e2986d484074a43d14f56de210da0b4a
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="processing-sql-statements"></a>Verarbeiten von SQL-Anweisungen
> [!IMPORTANT]  
>  Diese Funktion wird in einer zukünftigen Version von Windows entfernt werden. Verwenden Sie diese Funktion beim Entwickeln neuer Anwendungen und Planen von Anwendungen zu ändern, die dieses Feature verwenden. Microsoft empfiehlt die Verwendung der Cursorfunktionalität der Treiber.  
  
 Der ODBC-Cursorbibliothek übergibt alle SQL-Anweisungen direkt an den Treiber mit Ausnahme der folgenden:  
  
-   Positioniert Update und delete-Anweisungen  
  
-   **SELECT FOR UPDATE** Anweisungen  
  
-   SQL-Anweisungsbatches  
  
 Zum Ausführen von positionierten Updates und delete-Anweisungen und zur Positionierung des Cursors in einer Zeile aufrufen **SQLGetData** für diese Zeile erstellt die Cursorbibliothek eine gesuchte-Anweisung, die die Zeile identifiziert.  
  
 Dieser Abschnitt enthält die folgenden Themen.  
  
-   [Processing Positioned Update and Delete Statements (Verarbeiten einer positionierten Aktualisierung und von DELETE-Anweisungen)](../../../odbc/reference/appendixes/processing-positioned-update-and-delete-statements.md)  
  
-   [Processing SELECT FOR UPDATE Statements (Verarbeiten der Anweisung SELECT FOR UPDATE)](../../../odbc/reference/appendixes/processing-select-for-update-statements.md)  
  
-   [Processing Batches of SQL Statements (Verarbeiten von Batches von SQL-Anweisungen)](../../../odbc/reference/appendixes/processing-batches-of-sql-statements.md)  
  
-   [Erstellen von komplexen Anweisungen](../../../odbc/reference/appendixes/constructing-searched-statements.md)
