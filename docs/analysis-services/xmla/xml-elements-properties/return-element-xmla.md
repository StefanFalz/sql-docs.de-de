---
title: return-Element (XMLA) | Microsoft Docs
ms.date: 05/08/2018
ms.prod: sql
ms.technology: analysis-services
ms.custom: xmla
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: e8746fb9f8b397ef50b1a5c66a2132e5f0cf5c87
ms.sourcegitcommit: 808d23a654ef03ea16db1aa23edab496b73e5072
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2018
ms.locfileid: "34576192"
---
# <a name="return-element-xmla"></a>return-Element (XMLA)
[!INCLUDE[ssas-appliesto-sqlas-aas](../../../includes/ssas-appliesto-sqlas-aas.md)]
  Enthält Informationen, indem Sie eine [DiscoverResponse](../../../analysis-services/xmla/xml-elements-objects-discoverresponse.md) -Element als Antwort auf eine [Discover](../../../analysis-services/xmla/xml-elements-methods-discover.md) Methodenaufruf oder ein [ExecuteResponse](../../../analysis-services/xmla/xml-elements-objects-executeresponse.md) -Element als Antwort auf eine [Execute](../../../analysis-services/xmla/xml-elements-methods-execute.md) -Methodenaufruf.  
  
## <a name="syntax"></a>Syntax  
  
```xml  
  
<DiscoverResponse> <!-- or ExecuteResponse -->  
   <return>  
      <root>...</root>  
      <!-- or -->  
      <results>...</results> <!-- ExecuteResponse only -->  
   </return>  
</DiscoverResponse>  
```  
  
## <a name="element-characteristics"></a>Elementmerkmale  
  
|Merkmal|Description|  
|--------------------|-----------------|  
|Datentyp und -länge|InclusionThresholdSetting|  
|Standardwert|InclusionThresholdSetting|  
|Cardinality|1-1: Erforderliches Element, das nur einmal auftritt.|  
  
## <a name="element-relationships"></a>Elementbeziehungen  
  
|Beziehung|Element|  
|------------------|-------------|  
|Übergeordnete Elemente|[DiscoverResponse](../../../analysis-services/xmla/xml-elements-objects-discoverresponse.md), [ExecuteResponse](../../../analysis-services/xmla/xml-elements-objects-executeresponse.md)|  
|Untergeordnete Elemente|Siehe Tabelle unten.|  
  
|Ancestor|Untergeordnete Elemente|  
|--------------|--------------------|  
|[DiscoverResponse](../../../analysis-services/xmla/xml-elements-objects-discoverresponse.md)|[Stamm](../../../analysis-services/xmla/xml-elements-properties/root-element-xmla.md)|  
|[ExecuteResponse](../../../analysis-services/xmla/xml-elements-objects-executeresponse.md)|[Stamm](../../../analysis-services/xmla/xml-elements-properties/root-element-xmla.md) oder [Ergebnisse](../../../analysis-services/xmla/xml-elements-properties/results-element-xmla.md)|  
  
## <a name="remarks"></a>Hinweise  
 Das **return** -Element enthält die Daten, die von der **Discover** - und der **Execute** -Methode zurückgegeben wurden. In der Regel enthält das **return** -Element ein einzelnes **root** -Element, das entweder die von einem erfolgreichen **Discover** - oder **Execute** -Methodenaufruf zurückgegebenen Daten oder eine von einem nicht erfolgreichen Methodenaufruf zurückgegebene XMLA-Ausnahme (XML for Analysis) enthält. Wenn die **Execute** -Methode einen **Batch** -Befehl enthält, der mehrere Vorgänge ausführt, enthält das **return** -Element ein **results** -Element, das wiederum ein **root** -Element für jeden erfolgreich oder nicht erfolgreich vom **Batch** -Befehl ausgeführten Befehl enthält.  
  
## <a name="see-also"></a>Siehe auch
 [Eigenschaften &#40;XMLA&#41;](../../../analysis-services/xmla/xml-elements-properties/xml-elements-properties.md)  
  
  
