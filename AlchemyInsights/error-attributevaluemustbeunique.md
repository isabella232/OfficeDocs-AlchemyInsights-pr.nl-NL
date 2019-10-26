---
title: Fout AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36526980"
---
# <a name="error-attributevaluemustbeunique"></a>Fout: AttributeValueMustBeUnique

De meest voorkomende reden voor de fout AttributeValueMustBeUnique is twee objecten met verschillende SourceAnchor (immutableId) dezelfde waarde voor de kenmerken ProxyAddresses en/of UserPrincipalName hebben. U de AttributeValueMustBeUnique-fout oplossen:
  
1. Identificeer de gedupliceerde proxyAddresses, userPrincipalName of een andere kenmerkwaarde die de fout veroorzaakt. Bepaal ook welke twee (of meer) objecten bij het conflict betrokken zijn. Het rapport dat wordt gegenereerd door Azure AD Connect Health voor synchronisatie kan u helpen de twee objecten te identificeren.
    
2. Bepaal welk object moet blijven de gedupliceerde waarde en welk object moet niet.
    
3. Verwijder de gedupliceerde waarde van het object dat deze waarde niet mag hebben. Houd er rekening mee dat u de wijziging moet aanbrengen in de map waar het object vandaan komt. In sommige gevallen moet u mogelijk een van de objecten in conflict verwijderen.
    
4. Als u de wijziging hebt aangebracht in de on-premises AD, laat Azure AD Connect synchroniseren van de wijziging voor de fout te krijgen opgelost.
    

