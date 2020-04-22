---
title: FoutattribuutwaardeMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703169"
---
# <a name="error-attributevaluemustbeunique"></a>Fout: AttributeValueMustBeUnique

De meest voorkomende reden voor de fout AttributeValueMustBeUnieke is twee objecten met verschillende SourceAnchor (immutableId) hebben dezelfde waarde voor de kenmerken ProxyAddresses en/of UserPrincipalName. Ga als volgende over de fout AttributeValueMustBeUnique te fixeren:
  
1. Identificeer de gedupliceerde proxyAdressen, userPrincipalName of andere kenmerkwaarde die de fout veroorzaakt. Bepaal ook welke twee (of meer) objecten betrokken zijn bij het conflict. Met het rapport dat is gegenereerd door Azure AD Connect Health for sync, u de twee objecten identificeren.
    
2. Bepaal welk object de gedupliceerde waarde moet blijven hebben en welk object dat niet mag.
    
3. Verwijder de gedupliceerde waarde uit het object dat niet die waarde zou moeten hebben. Houd er rekening mee dat u de wijziging moet aanbrengen in de map waar het object vandaan komt. In sommige gevallen moet u mogelijk een van de objecten in conflict verwijderen.
    
4. Als u de wijziging hebt aangebracht in het ad op locatie, laat U Azure AD Connect de wijziging synchroniseren om de fout te laten oplossen.
    

