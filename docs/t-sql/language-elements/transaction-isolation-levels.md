---
title: Transaktionsisolationsstufen | Microsoft-Dokumentation
ms.custom: ''
ms.date: 03/14/2017
ms.prod: sql
ms.prod_service: sql-database
ms.component: t-sql|language-elements
ms.reviewer: ''
ms.suite: sql
ms.technology: t-sql
ms.tgt_pltfrm: ''
ms.topic: language-reference
dev_langs:
- TSQL
helpviewer_keywords:
- locking [SQL Server], hints
- isolation levels [SQL Server], metadata access
- hints [SQL Server], locking
ms.assetid: 02bb71fa-1e92-4782-a9cf-6e256cc1f3ea
caps.latest.revision: 23
author: douglaslMS
ms.author: douglasl
manager: craigg
ms.openlocfilehash: 1b0322843a6fd6493f3a4a72af723bbacc9dcdcd
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="transaction-isolation-levels"></a>Transaktionsisolationsstufen
[!INCLUDE[tsql-appliesto-ss2012-xxxx-xxxx-xxx-md](../../includes/tsql-appliesto-ss2012-xxxx-xxxx-xxx-md.md)]

  In [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] werden Sperrhinweise in Abfragen, die über Katalogsichten, Kompatibilitätssichten, Informationsschemasichten oder Metadaten ausgebende integrierte Funktionen auf Metadaten zugreifen, nicht mit Sicherheit berücksichtigt.  
  
 Intern berücksichtigt [!INCLUDE[ssDEnoversion](../../includes/ssdenoversion-md.md)] beim Zugriff auf Metadaten nur die Isolationsstufe READ COMMITTED. Wenn eine Transaktion beispielsweise die Isolationsstufe SERIALIZABLE besitzt und innerhalb der Transaktion versucht wird, über Katalogsichten oder Metadaten ausgebende integrierte Funktionen auf Metadaten zuzugreifen, werden die entsprechenden Abfragen ausgeführt, bis sie als READ COMMITTED abgeschlossen sind. Bei der Momentaufnahmeisolation kann der Zugriff auf Metadaten jedoch aufgrund von gleichzeitigen DDL-Vorgängen einen Fehler erzeugen. Der Grund dafür ist, dass Metadaten nicht versionsspezifisch sind. Daher besteht das Risiko, dass bei der Momentaufnahmeisolation der Zugriff über folgende Sichten und Funktionen zu einem Fehler führt:  
  
-   Katalogsichten  
  
-   Kompatibilitätssichten  
  
-   Informationsschemasichten  
  
-   Metadaten ausgebende integrierte Funktionen  
  
-   Die **sp_help**-Gruppe gespeicherter Prozeduren  
  
-   [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Native Client-Katalogprozeduren  
  
-   Dynamische Verwaltungssichten (DMVs, Dynamic Management Views) und -funktionen  
  
 Weitere Informationen zu Isolationsstufen in SQL Server finden Sie unter [SET TRANSACTION ISOLATION LEVEL &#40;Transact-SQL&#41;](../../t-sql/statements/set-transaction-isolation-level-transact-sql.md).  
  
 Die folgende Tabelle fasst den Zugriff auf Metadaten bei verschiedenen Isolationsstufen zusammen.  
  
|Isolationsstufe|Supported|Berücksichtigt|  
|---------------------|---------------|-------------|  
|READ UNCOMMITTED|nein|Nicht mit Sicherheit berücksichtigt|  
|READ COMMITTED|ja|ja|  
|REPEATABLE READ|nein|nein|  
|MOMENTAUFNAHMEN ISOLATION|nein|nein|  
|SERIALIZABLE|nein|nein|  
  
  
