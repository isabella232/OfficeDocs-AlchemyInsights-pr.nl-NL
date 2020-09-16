---
title: ConsistencyGuid/sourceAnchor gedrag
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756278"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor gedrag

Azure AD Connect (versie 1.1.524.0 en After) vergemakkelijkt het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk. Wanneer u deze functie gebruikt, worden in azure AD Connect automatisch de synchronisatieregels geconfigureerd voor:
  
- Gebruik msDS-ConsistencyGuid als het sourceAnchor-kenmerk voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor een bepaald on-premises AD User object waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het kenmerk msDS-ConsistencyGuid in on-premises Active Directory. Nadat het kenmerk msDS-ConsistencyGuid is ingevuld, wordt het object in azure AD Connect vervolgens geëxporteerd naar Azure AD.
    
 **Opmerking:** Wanneer een on-premises AD-object wordt geïmporteerd in azure AD Connect (dat wil zeggen dat het wordt geïmporteerd in de AD connector-ruimte en de geprojecteerde tekst in de standaardtekst), kunt u de sourceAnchor waarde niet meer wijzigen. Als u de sourceAnchor waarde wilt opgeven voor een bepaald on-premises AD-object, configureert u het kenmerk msDS-ConsistencyGuid voordat het wordt geïmporteerd in azure AD Connect. 
  
Ga voor meer informatie over SourceAnchor en ConsistencyGuid naar de volgende informatie: [Azure AD Connect: ontwerp concepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

