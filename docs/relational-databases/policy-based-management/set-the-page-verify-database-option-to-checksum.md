---
title: Festlegen der PAGE_VERIFY-Datenbankoption auf CHECKSUM | Microsoft-Dokumentation
ms.custom: ''
ms.date: 03/04/2017
ms.prod: sql
ms.prod_service: database-engine
ms.component: performance-monitor
ms.reviewer: ''
ms.suite: sql
ms.technology:
- database-engine
ms.tgt_pltfrm: ''
ms.topic: conceptual
helpviewer_keywords:
- Best Practices [Database Engine]
ms.assetid: 686b9a4a-ea61-4263-9ab8-f444a3077679
caps.latest.revision: 8
author: MikeRayMSFT
ms.author: mikeray
manager: craigg
ms.openlocfilehash: 2bb1bccbb0cebbd6b0373a633e88e871342a2e90
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="set-the-pageverify-database-option-to-checksum"></a>Festlegen der PAGE_VERIFY-Datenbankoption auf CHECKSUM
[!INCLUDE[appliesto-ss-xxxx-xxxx-xxx-md](../../includes/appliesto-ss-xxxx-xxxx-xxx-md.md)]
  Diese Regel überprüft, ob die PAGE_VERIFY-Datenbankoption auf CHECKSUM festgelegt ist. Wenn CHECKSUM für die PAGE_VERIFY-Datenbankoption angegeben wird, berechnet [!INCLUDE[ssDEnoversion](../../includes/ssdenoversion-md.md)] beim Schreiben der Seite auf den Datenträger eine Prüfsumme des Inhalts der gesamten Seite und speichert den Wert im Seitenkopf. Wenn die Seite vom Datenträger gelesen wird, wird die Prüfsumme erneut berechnet und mit dem im Seitenkopf gespeicherten Prüfsummenwert verglichen. Dadurch wird ein hohes Maß an Integrität der Datendateien bereitgestellt.  
  
## <a name="best-practices-recommendations"></a>Empfehlungen zu Best Practices  
 Legen Sie die PAGE_VERIFY-Datenbankoption auf CHECKSUM fest.  
  
## <a name="for-more-information"></a>Weitere Informationen  
 [ALTER DATABASE SET-Optionen &#40;Transact-SQL&#41;](../../t-sql/statements/alter-database-transact-sql-set-options.md)  
  
  
