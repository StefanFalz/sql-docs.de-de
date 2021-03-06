---
title: Herstellen einer Verbindung mit einer dBASE- oder einer anderen DBF-Datei | Microsoft-Dokumentation
ms.custom: ''
ms.date: 03/14/2017
ms.prod: sql
ms.prod_service: integration-services
ms.component: connection-manager
ms.reviewer: ''
ms.suite: sql
ms.technology:
- integration-services
ms.tgt_pltfrm: ''
ms.topic: conceptual
helpviewer_keywords:
- connecting to DBF files
- dBase files
- DBF files
ms.assetid: b0e8c831-9f96-475c-82a4-4f5b02692752
caps.latest.revision: 16
author: douglaslMS
ms.author: douglasl
manager: craigg
ms.openlocfilehash: 6fd155c0d1e196c31b340c6364ce66db4acefb49
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="connect-to-a-dbase-or-other-dbf-file"></a>Herstellen einer Verbindung mit einer dBASE- oder einer anderen DBF-Datei
  Sie können eine Verbindung mit einer dBASE- oder einer anderen DBF-Datenbankdatei in einem [!INCLUDE[ssISnoversion](../../includes/ssisnoversion-md.md)] -Paket herstellen, indem Sie einen OLE DB-Verbindungs-Manager verwenden und Microsoft OLE DB-Anbieter für Jet 4.0 auswählen.  
  
> [!NOTE]  
>  Das Importieren aus oder Exportieren in dBASE- oder andere DBF-Dateien wird vom SQL Server-Import/Export-Assistenten in [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] nicht unterstützt. Sie können die Daten aus DBF-Dateien mit Microsoft Access oder Microsoft Excel in eine Access-Datenbank bzw. in Excel-Kalkulationstabellen importieren und anschließend den SQL Server-Import/Export-Assistenten verwenden.  
  
### <a name="to-configure-a-connection-manager-to-connect-to-a-dbase-or-other-dbf-file"></a>So konfigurieren Sie einen Verbindungs-Manager für das Herstellen einer Verbindung mit einer dBASE- oder anderen DBF-Datei  
  
1.  Fügen Sie dem Paket einen neuen OLE DB-Verbindungs-Manager hinzu. Weitere Informationen finden Sie unter [Add, Delete, or Share a Connection Manager in a Package](http://msdn.microsoft.com/library/6f2ba4ea-10be-4c40-9e80-7efcf6ee9655).  
  
2.  Wählen Sie im Dialogfeld **Verbindungs-Manager** auf der Seite **Verbindung** als **Anbieter**OLE DB nativ\Microsoft Jet 4.0 OLE DB-Anbieter aus.  
  
3.  Bei der Verwendung von DBF-Dateien stellt der Ordner die Datenbank dar und die einzelnen DBF-Dateien stellen Tabellen dar. Daher muss im Textfeld **Name der Datenbankdatei** der Pfad zum Ordner angegeben sein, in dem sich die DBF-Datei befindet. Der Dateiname selbst darf im Pfad nicht enthalten sein. Sie können den Ordnerpfad eingeben, kopieren oder über die Schaltfläche **Durchsuchen** die betreffende DBF-Datei auswählen und anschließend den Dateinamen am Ende des Pfades entfernen.  
  
4.  Geben Sie im Dialogfeld **Verbindungs-Manager** auf der Seite **Alle** als Wert für die Erweiterten Eigenschaften entsprechend **dBASE III**, **dBASE IV**oder **dBASE 5.0**ein.  
  
5.  Klicken Sie auf **Verbindung testen** , um die Gültigkeit der eingegebenen Werte zu überprüfen. Es sollte die Meldung "Die Testverbindung war erfolgreich." angezeigt werden. Klicken Sie auf **OK** , um das Meldungsfeld zu schließen.  
  
6.  Klicken Sie auf **OK** , um die Konfiguration des Verbindungs-Managers zu speichern.  
  
7.  Wenn Sie den Verbindungs-Manager für den Datenfluss eines Pakets verwenden möchten, wählen Sie eine OLE DB-Quelle oder ein OLE DB-Ziel aus und konfigurieren Quelle bzw. Ziel so, dass der in den vorangegangenen Schritten erstellte Verbindungs-Manager verwendet wird.  
  
## <a name="see-also"></a>Weitere Informationen finden Sie unter  
 [OLE DB-Verbindungs-Manager](../../integration-services/connection-manager/ole-db-connection-manager.md)  
  
  
