---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813755"
---
# <a name="error-attributevaluemustbeunique"></a>Fout: AttributeValueMustBeUnique

De meest voorkomende reden voor de fout AttributeValueMustBeUnique is dat twee objecten met verschillende SourceAnchor (immutableId) dezelfde waarde hebben voor de proxyaddresses en/of UserPrincipalName-kenmerken. De fout AttributeValueMustBeUnique oplossen:
  
1. Identificeer de gedupliceerde proxyAddresses, userPrincipalName of andere kenmerkwaarde die de fout veroorzaakt. Bepaal ook welke twee (of meer) objecten betrokken zijn bij het conflict. Het rapport dat wordt gegenereerd door Azure AD Connect Health voor synchronisatie, kan u helpen de twee objecten te identificeren.
    
2. Bepaal welk object de gedupliceerde waarde moet blijven hebben en welk object niet.
    
3. Verwijder de gedupliceerde waarde uit het object dat DEZE WAARDE NIET mag hebben. Houd er rekening mee dat u de wijziging moet aan brengen in de adreslijst waar het object vandaan komt. In sommige gevallen moet u mogelijk een van de objecten in conflict verwijderen.
    
4. Als u de wijziging hebt aangebracht in de on-premises AD, laat Azure AD Connect de wijziging synchroniseren om de fout te herstellen.
    

