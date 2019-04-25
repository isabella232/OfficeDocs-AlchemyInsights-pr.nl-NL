---
title: ConsistencyGuid / sourceAnchor gedrag
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408103"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor gedrag

Azure AD verbinden (versie 1.1.524.0 en na) nu vergemakkelijkt het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk. Wanneer u deze functie gebruikt, het Azure AD verbinden automatisch synchronisatieregels te configureren:
  
- MsDS-ConsistencyGuid gebruiken als het kenmerk sourceAnchor voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor een gegeven op-premises AD gebruiker object waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, Azure AD verbinden schrijft de kenmerken objectGUID waarde terug naar het kenmerk msDS-ConsistencyGuid in Active Directory voor gebouwen. Nadat het kenmerk msDS-ConsistencyGuid is gevuld, Azure AD verbinden het object vervolgens geëxporteerd naar Azure AD.
    
 **Opmerking:** Eenmaal een op-premises AD object wordt geïmporteerd in Azure AD Connect (die wordt geïmporteerd in de Connector AD ruimte en geprojecteerd in de Metaverse), u kunt de waarde sourceAnchor niet meer wijzigen. De sourceAnchor waarde voor een gegeven in de lokalen AD object, wordt het kenmerk msDS-ConsistencyGuid configureren voordat deze wordt geïmporteerd in Azure AD verbinden. 
  
Raadpleeg voor meer informatie over SourceAnchor en ConsistencyGuid, de volgende: [Azure AD verbinden: concepten ontwerpen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

