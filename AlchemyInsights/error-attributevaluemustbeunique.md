---
title: Fout AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709146"
---
# <a name="error-attributevaluemustbeunique"></a>Fout: AttributeValueMustBeUnique

De meest voorkomende reden voor de fout in AttributeValueMustBeUnique is twee objecten met een ander SourceAnchor (immutableId) dezelfde waarde heeft voor de kenmerken ProxyAddresses en/of UserPrincipalName. Oplossing van de AttributeValueMustBeUnique-fout:
  
1. Identificeer de gedupliceerde proxyAddresses, userPrincipalName of een andere kenmerkwaarde die de fout veroorzaakt. U kunt ook identificeren welke twee (of meer) objecten bij het conflict betrokken zijn. Het rapport dat door Azure AD Connect Health voor synchronisatie is gegenereerd, kan u helpen bij het identificeren van de twee objecten.
    
2. Bepaal welke object de gedupliceerde waarde moet hebben en welk object dit niet mag doen.
    
3. Verwijdert de gedupliceerde waarde van het object dat deze waarde niet mag bevatten. Let op: u moet de wijziging aanbrengen in de map waarin het object is gebrond. In sommige gevallen moet u mogelijk een van de objecten in conflict verwijderen.
    
4. Als u de wijziging in de on-premises advertentie hebt aangebracht, kunt u de wijziging in azure AD Connect synchroniseren zodat de fout wordt hersteld.
    

