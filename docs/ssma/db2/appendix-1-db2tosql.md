---
title: Anhang - 1 (DB2ToSQL) | Microsoft Docs
ms.prod: sql
ms.prod_service: sql-tools
ms.component: ssma-db2
ms.custom: ''
ms.date: 01/19/2017
ms.reviewer: ''
ms.suite: sql
ms.technology: ssma
ms.tgt_pltfrm: ''
ms.topic: conceptual
applies_to:
- Azure SQL Database
- SQL Server
ms.assetid: c6a30367-d56f-4fcc-8920-c6a6b0335a67
caps.latest.revision: 6
author: Shamikg
ms.author: Shamikg
manager: craigg
ms.openlocfilehash: 69752dfd2ced7946b2fb6470bc3780df286cc3f8
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="appendix---1-db2tosql"></a>Anhang - 1 (DB2ToSQL)
Kurze Übersicht über die Befehlszeilenoptionen SSMA-Konsole:  
  
|Sl. Nein.|Schalter|Erforderlich?|Switch-Argument|Zulässige Werte|  
|-----------|----------|-------------|-------------------|--------------------|  
|1|-s/script|ja|scriptfile|XML-Dateiname ist ungültig.<br /><br />-Konsole Definition Skriptdatei an.|  
|2|-V-variable|nein|variablevaluefile|XML-Dateiname ist ungültig.<br /><br />Wenn Variablen in einer Skriptdatei verwendet werden, muss diese Datei angegeben werden.|  
|3|-c/serverconnection|nein|serverconnectionfile|XML-Dateiname ist ungültig.<br /><br />Diese Datei enthält Informationen zur Serververbindung.|  
|4|X-/ Xmloutput|nein|xmloutputfile|Diese Option gibt die Konsolenausgabe in das XML-Format an. Wenn diese Option nicht angegeben ist, wird die standardmäßigen Ausgabe im Textformat.<br /><br />Wenn Xmloutputfile nicht angegeben ist, wird die XML-Ausgabe an "stdout" umgeleitet.<br /><br />Xmloutputfile ist der Name der Datei, die in die Konsolenausgabe in das XML-Format geschrieben wird.|  
|5|-l/log|nein|logfile|Der Dateiname ist ungültig.|  
|6|-e/projectenvironment|nein|projectenvironmentfolder|Gültigen Ordnernamen an, die Dateien der SSMA-Projekt enthält.|  
|7|-p/securepassword|nein|-a/hinzufügen {< Server_id > [,... n] &#124; alle} – C&#124;Serverconnection < Server-Verbindungsdatei > [-V&#124;Variable < Variable-Wert-Datei >] [-o/overwrite]<br /><br />oder<br /><br />-a/hinzufügen {< Server_id > [,... n] &#124; alle} – s&#124;Skript < Skriptdatei > [-V&#124;Variable < Variable-Wert-Datei >] [-o/overwrite]<br /><br />– R Reparaturprogramm {< Server_id > [,... n] &#124; alle}<br /><br />-l/list<br /><br />– e/Export {< Server-Id > [,... n] &#124; alle} < verschlüsselt-Kennwort - Datei ><br /><br />– i / importieren {< Server-Id > [,... n] &#124; alle} < verschlüsselt-Kennwort-Datei >|Wenn angegeben, muss diese Option nicht mit anderen Optionen kombiniert werden.<br /><br />Server-Id: eine eindeutige ID für einen Server {String} bereitgestellt<br /><br />Server-Verbindungsdatei: Server-Definitionsdatei (Serverconnectionfile oder Scriptfile).<br /><br />Variable-Wert-Datei: Es ist eine Variablendefinition-Datei und in Server-Verbindungsdatei verwendet.<br /><br />verschlüsselt ein Kennwort – Datei: eine Datei mit Servern Kennwörter verschlüsselt mit einer Passphrase Benutzer angegeben ist.|  
|8|-?|nein|Nicht zutreffend|Nicht zutreffend|  
  
## <a name="see-also"></a>Siehe auch  
[Executing the SSMA Console (Ausführen der SSMA-Konsole)](http://msdn.microsoft.com/en-us/ce63f633-067d-4f04-b8e9-e1abd7ec740b)  
  
