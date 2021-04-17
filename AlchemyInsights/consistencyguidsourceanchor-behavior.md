---
title: ConsistencyGuid /sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816987"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor behavior

Azure AD Connect (versie 1.1.524.0 en daarna) faciliteert nu het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk. Wanneer u deze functie gebruikt, worden de synchronisatieregels automatisch geconfigureerd door Azure AD Connect:
  
- MsDS-ConsistencyGuid gebruiken als het sourceAnchor-kenmerk voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor elk on-premises AD-gebruikersobject waarvan het msDS-ConsistencyGuid-kenmerk niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het msDS-ConsistencyGuid-kenmerk in on-premises Active Directory. Nadat het msDS-ConsistencyGuid-kenmerk is ingevuld, exporteert Azure AD Connect het object vervolgens naar Azure AD.
    
 **Opmerking:** Wanneer een on-premises AD-object is geïmporteerd in Azure AD Connect (dat wil zeggen, geïmporteerd in de AD Connector-ruimte en geprojecteerd in de Metaverse), kunt u de bronwaardeAnchor niet meer wijzigen. Als u de bronwaardeAnchor wilt opgeven voor een bepaald on-premises AD-object, configureert u het msDS-ConsistencyGuid-kenmerk voordat het wordt geïmporteerd in Azure AD Connect. 
  
Voor meer informatie over SourceAnchor en ConsistencyGuid raadpleegt u het volgende: [Azure AD Connect: Ontwerpconcepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

