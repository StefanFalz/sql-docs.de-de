---
title: Hinzufügen von Datensätzen | Microsoft Docs
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
- AddNew method [ADO]
- ADO, editing data
- editing data [ADO], AddNew method
- editing data [ADO], adding data
ms.assetid: dd34669e-6f06-403b-9241-1c85c82aecc2
caps.latest.revision: 10
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 8e870545c3ff62342ebf707619d0963d6421e6fa
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="adding-records-to-a-recordset"></a>Hinzufügen von Datensätzen zu einem Recordset
Verwenden der **AddNew** Methode zum Erstellen und initialisieren einen neuen Datensatz in einer vorhandenen **Recordset**. Können Sie die **unterstützt** Methode mit einer **CursorOptionEnum** Wert **AdAddNew** zu überprüfen, ob Sie Datensätze, mit dem aktuellen hinzufügen können **Recordset** Objekt.

 Nach dem Aufruf der **AddNew** -Methode, der neue Datensatz wird zum aktuellen Datensatz und bleibt nach dem Aufruf von aktuellen der **Update** Methode. Wenn die **Recordset** Objekt werden keine Lesezeichen unterstützt, Sie ist möglicherweise nicht auf den neuen Datensatz zugreifen, nachdem Sie zu einem anderen Datensatz wechseln. Aus diesem Grund abhängig vom Cursortyp, müssen möglicherweise zum Aufrufen der **Requery** Methode zum Erstellen von neuen Datensatzes zugegriffen werden kann.

 Beim Aufrufen **AddNew** beim Bearbeiten des aktuellen Datensatzes oder beim Hinzufügen eines neuen Datensatzes ADO Ruft die **Update** Methode zum Speichern ändert, und klicken Sie dann den neuen Eintrag erstellt.

 Dieser Abschnitt enthält die folgenden Themen.

-   [Hinzufügen von Datensätzen mit der AddNew-Methode](../../../ado/guide/data/adding-records-using-addnew.md)

-   [Hinzufügen von mehreren Feldern](../../../ado/guide/data/adding-multiple-fields.md)

-   [Bestimmen des Bearbeitungsmodus](../../../ado/guide/data/determining-edit-mode.md)

-   [Using AddNew in Immediate and Batch Modes (Verwenden von AddNew in Immediate- und Batch-Modi)](../../../ado/guide/data/using-addnew-in-immediate-and-batch-modes.md)
