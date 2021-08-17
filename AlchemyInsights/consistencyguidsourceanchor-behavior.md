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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044335"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor behavior

Azure AD Verbinding maken (versie 1.1.524.0 en daarna) maakt het gebruik van msDS-ConsistencyGuid als bronanchor-kenmerk mogelijk. Wanneer u deze functie gebruikt, worden Verbinding maken de synchronisatieregels automatisch geconfigureerd op:
  
- MsDS-ConsistencyGuid gebruiken als het sourceAnchor-kenmerk voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor elk on-premises AD-gebruikersobject waarvan het msDS-ConsistencyGuid-kenmerk niet is ingevuld, schrijft Azure AD Verbinding maken de objectGUID-waarde terug naar het msDS-ConsistencyGuid-kenmerk in on-premises Active Directory. Nadat het msDS-consistencyGuid-kenmerk is ingevuld, exporteert Azure AD Verbinding maken vervolgens het object naar Azure AD.
    
 **Opmerking:** Wanneer een on-premises AD-object is geïmporteerd in Azure AD Verbinding maken (dat wil zeggen, geïmporteerd in de AD Connector-ruimte en geprojecteerd in de Metaverse), kunt u de bronwaardeAnchor niet meer wijzigen. Als u de bronwaardeAnchor wilt opgeven voor een bepaald on-premises AD-object, configureert u het msDS-ConsistencyGuid-kenmerk voordat het wordt geïmporteerd in Azure AD-Verbinding maken. 
  
Voor meer informatie over SourceAnchor en ConsistencyGuid raadpleegt u het volgende: [Azure AD Verbinding maken: Ontwerpconcepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

