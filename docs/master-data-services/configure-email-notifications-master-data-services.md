---
title: Konfigurieren von E-Mail-Benachrichtigungen (Master Data Services) | Microsoft-Dokumentation
ms.custom: ''
ms.date: 03/07/2017
ms.prod: sql
ms.prod_service: mds
ms.component: non-specific
ms.reviewer: ''
ms.suite: sql
ms.technology:
- master-data-services
ms.tgt_pltfrm: ''
ms.topic: conceptual
helpviewer_keywords:
- e-mail [Master Data Services], configuring
- notifications [Master Data Services], configuring notifications
ms.assetid: 4241a6ab-7465-471b-9890-57c6b572037e
caps.latest.revision: 7
author: leolimsft
ms.author: lle
manager: craigg
ms.openlocfilehash: 95696ddfa7941511b713eccffe635f9b59acc450
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="configure-email-notifications-master-data-services"></a>Konfigurieren von E-Mail-Benachrichtigungen (Master Data Services)

[!INCLUDE[appliesto-ss-xxxx-xxxx-xxx-md-winonly](../includes/appliesto-ss-xxxx-xxxx-xxx-md-winonly.md)]

  Konfigurieren Sie Benachrichtigungs-E-Mails, wenn E-Mail-Nachrichten von [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] automatisch gesendet werden sollen.  
  
### <a name="to-configure-notifications"></a>So konfigurieren Sie Benachrichtigungen  
  
1.  Wählen Sie in [!INCLUDE[ssMDScfgmgr](../includes/ssmdscfgmgr-md.md)]auf der Seite **Datenbank** die [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] -Datenbank aus.  
  
2.  Klicken Sie im Abschnitt **Systemeinstellungen** auf **Profil erstellen**.  
  
3.  Füllen Sie alle Pflichtfelder aus. Weitere Informationen finden Sie unter [Datenbank-E-Mail-Profil und -Konto erstellen &#40;Dialogfeld im Konfigurations-Manager für Master Data Services&#41;](../master-data-services/create-database-mail-profile-and-account-dialog-box.md).  
  
4.  Klicken Sie auf **OK**.  
  
    > [!NOTE]  
    >  Nachdem Sie Benachrichtigungen konfiguriert haben, können Sie keine Änderungen mithilfe von [!INCLUDE[ssMDScfgmgr](../includes/ssmdscfgmgr-md.md)] vornehmen. Sie müssen die Änderungen direkt in der [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] -Datenbank vornehmen. Weitere Informationen finden Sie unter [Database Mail Configuration Objects](../relational-databases/database-mail/database-mail-configuration-objects.md).  
  
## <a name="next-steps"></a>Next Steps  
  
-   [!INCLUDE[ssMDScfgmgr](../includes/ssmdscfgmgr-md.md)] verfügt über Einstellungen, die sich auf Benachrichtigungen auswirken. Sie können diese Einstellungen in [!INCLUDE[ssMDScfgmgr](../includes/ssmdscfgmgr-md.md)] oder direkt in der Tabelle Systemeinstellungen der [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] -Datenbank anpassen. Weitere Informationen finden Sie unter [Systemeinstellungen &#40;Master Data Services&#41;](../master-data-services/system-settings-master-data-services.md).  
  
## <a name="see-also"></a>Weitere Informationen finden Sie unter  
 [Benachrichtigungen &#40;Master Data Services&#41;](../master-data-services/notifications-master-data-services.md)   
 [Problembehandlung für E-Mail-Benachrichtigungen (Master Data Services)](http://social.technet.microsoft.com/wiki/contents/articles/troubleshooting-email-notifications-master-data-services.aspx)   
 [Konfigurieren von Geschäftsregeln für das Senden von Benachrichtigungen &#40;Master Data Services&#41;](../master-data-services/configure-business-rules-to-send-notifications-master-data-services.md)  
  
  
