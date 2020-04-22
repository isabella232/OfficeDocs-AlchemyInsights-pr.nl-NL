---
title: ConsistencyGuid / sourceAnchor gedrag
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705728"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor gedrag

Azure AD Connect (versie 1.1.524.0 en daarna) vergemakkelijkt nu het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk. Wanneer u deze functie gebruikt, configureert Azure AD Connect automatisch de synchronisatieregels om:
  
- MsDS-ConsistencyGuid gebruiken als het kenmerk sourceAnchor voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor een bepaald on-premises AD-gebruikersobject waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het kenmerk msDS-ConsistencyGuid in on-premises Active Directory. Nadat het kenmerk msDS-ConsistencyGuid is ingevuld, exporteert Azure AD Connect het object naar Azure AD.
    
 **Let op:** Zodra een on-premises AD-object is geïmporteerd in Azure AD Connect (dat wil zeggen geïmporteerd in de AD-connectorruimte en geprojecteerd in de metaverse), u de bronankerwaarde niet meer wijzigen. Als u de bronAnkerwaarde voor een bepaald on-premises AD-object wilt opgeven, configureert u het kenmerk msDS-ConsistencyGuid voordat het wordt geïmporteerd in Azure AD Connect. 
  
Zie voor meer informatie over SourceAnchor en ConsistencyGuid het volgende: [Azure AD Connect: Design concepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

