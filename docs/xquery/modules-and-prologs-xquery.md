---
title: Module und Prologe (XQuery) | Microsoft Docs
ms.custom: ''
ms.date: 03/06/2017
ms.prod: sql
ms.prod_service: sql
ms.component: xquery
ms.reviewer: ''
ms.suite: sql
ms.technology:
- database-engine
ms.tgt_pltfrm: ''
ms.topic: language-reference
applies_to:
- SQL Server
dev_langs:
- XML
helpviewer_keywords:
- XQuery, prolog
- prolog
ms.assetid: 0f17b4a4-6234-41d4-a996-6db4e27bff7e
caps.latest.revision: 13
author: rothja
ms.author: jroth
manager: craigg
ms.openlocfilehash: 08d19f2a24c243647b4004a557fd25bf96d2dd62
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="modules-and-prologs-xquery"></a>Module und Prologe (XQuery)
[!INCLUDE[tsql-appliesto-ss2012-xxxx-xxxx-xxx-md](../includes/tsql-appliesto-ss2012-xxxx-xxxx-xxx-md.md)]

  [XQuery-Prolog](../xquery/modules-and-prologs-xquery-prolog.md) ist eine Reihe von Namespacedeklarationen. Wenn Sie den Namespace im Prolog verwenden, können Sie ein Präfix für die Namespaceeinbindung angeben und das Präfix im Abfragehauptteil verwenden.  
  
## <a name="implementation-limitations"></a>Implementierungseinschränkungen  
 Die folgenden XQuery-Spezifikationen werden in dieser Implementierung nicht unterstützt:  
  
-   Moduldeklaration (`version`)  
  
-   Moduldeklaration (`module namespace`)  
  
-   Xmpspacedeclaration (`xmlspace`)  
  
-   Standardsortierungsdeklaration (`declare default collation`)  
  
-   Basis-URI-Deklaration (`declare base-uri`)  
  
-   Konstruktionsdeklaration (`declare construction`)  
  
-   Standardreihenfolgendeklaration (`declare ordering`)  
  
-   Schemaimport (`import schema namespace`)  
  
-   Modulimport (`import module`)  
  
-   Variable Deklaration im Prolog (`declare variable`)  
  
-   Funktionsdeklaration (`declare function`)  
  
## <a name="in-this-section"></a>In diesem Abschnitt  
 [XQuery-Prolog](../xquery/modules-and-prologs-xquery-prolog.md)  
 Beschreibt XQuery-Prolog.  
  
## <a name="see-also"></a>Siehe auch  
 [XQuery-Sprachreferenz &#40;SQL Server&#41;](../xquery/xquery-language-reference-sql-server.md)  
  
  
