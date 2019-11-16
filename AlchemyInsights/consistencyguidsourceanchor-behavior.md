---
title: Consistentie/bronanker gedrag
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516971"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Consistentie/bronanker gedrag

Azure AD Connect (versie 1.1.524.0 en na) vereenvoudigt nu het gebruik van msDS-consistentie Cyguid als sourceAnchor kenmerk. Wanneer u deze functie gebruikt, configureert Azure AD Connect automatisch de synchronisatieregels om:
  
- Gebruik msDS-consistentie Cyguid als het kenmerk sourceAnchor voor gebruikersobjecten. ObjectGUID wordt gebruikt voor andere objecttypen.
    
- Voor een bepaalde on-premises AD-gebruikersobject waarvan het kenmerk msDS-consistentie Cyguid niet is ingevuld, schrijft Azure AD Connect de waarde objectGUID terug naar het kenmerk msDS-consistentie Cyguid in on-premises Active Directory. Nadat het kenmerk msDS-consistentie Cyguid is ingevuld, Azure AD Connect vervolgens exporteert het object naar Azure AD.
    
 **Opmerking:** Zodra een on-premises AD-object is geïmporteerd in azure AD Connect (dat is, geïmporteerd in de AD-connector ruimte en geprojecteerd in de Metaverse), u de waarde sourceAnchor niet meer wijzigen. Als u de waarde sourceAnchor voor een bepaalde on-premises AD-object, configureert u het kenmerk msDS-consistentie Cyguid voordat deze wordt geïmporteerd in azure AD Connect. 
  
Raadpleeg de volgende onderwerpen voor meer informatie over SourceAnchor en consistentie Cyguid: [Azure AD Connect: ontwerpconcepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

