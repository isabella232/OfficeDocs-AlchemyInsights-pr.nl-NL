---
title: Fout AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499629"
---
# <a name="error-attributevaluemustbeunique"></a>Fout: AttributeValueMustBeUnique

De meest voorkomende reden voor de fout AttributeValueMustBeUnique is twee objecten met verschillende SourceAnchor (immutableId) dezelfde waarde hebben voor de kenmerken ProxyAddresses en/of UserPrincipalName. De AttributeValueMustBeUnique om fout te herstellen:
  
1. Identificeer de gedupliceerde proxyAddresses, userPrincipalName of andere kenmerkwaarde die de fout veroorzaakt. Ook kunt u aangeven welke twee (of meer) objecten in het conflict zijn betrokken. Het rapport gegenereerd door Azure AD verbinding maken met de gezondheid voor synchronisatie kunt u de twee objecten identificeren.
    
2. Bepalen welk object moet blijven de gedupliceerde waarde hebben en welk object moet niet.
    
3. Verwijder de dubbele waarde van het object dat moet geen waarde. Houd er rekening mee dat u ervoor moet de wijziging in de map waarin het object is opgehaald. In sommige gevallen moet u een van de objecten in een conflict verwijderen.
    
4. Als u de wijziging hebt aangebracht in de op AD, laat Azure AD verbinden synchroniseren de wijziging voor de fout hersteld.
    

