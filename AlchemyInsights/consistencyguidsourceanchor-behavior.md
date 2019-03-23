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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753097"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d99f3-102">ConsistencyGuid / sourceAnchor gedrag</span><span class="sxs-lookup"><span data-stu-id="d99f3-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d99f3-103">Azure AD verbinden (versie 1.1.524.0 en na) nu vergemakkelijkt het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk.</span><span class="sxs-lookup"><span data-stu-id="d99f3-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d99f3-104">Wanneer u deze functie gebruikt, het Azure AD verbinden automatisch synchronisatieregels te configureren:</span><span class="sxs-lookup"><span data-stu-id="d99f3-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d99f3-105">MsDS-ConsistencyGuid gebruiken als het kenmerk sourceAnchor voor gebruikersobjecten.</span><span class="sxs-lookup"><span data-stu-id="d99f3-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d99f3-106">ObjectGUID wordt gebruikt voor andere objecttypen.</span><span class="sxs-lookup"><span data-stu-id="d99f3-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d99f3-107">Voor een gegeven op-premises AD gebruiker object waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, Azure AD verbinden schrijft de kenmerken objectGUID waarde terug naar het kenmerk msDS-ConsistencyGuid in Active Directory voor gebouwen.</span><span class="sxs-lookup"><span data-stu-id="d99f3-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d99f3-108">Nadat het kenmerk msDS-ConsistencyGuid is gevuld, Azure AD verbinden het object vervolgens geëxporteerd naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d99f3-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d99f3-109">**Opmerking:** Eenmaal een op-premises AD object wordt geïmporteerd in Azure AD Connect (die wordt geïmporteerd in de Connector AD ruimte en geprojecteerd in de Metaverse), u kunt de waarde sourceAnchor niet meer wijzigen.</span><span class="sxs-lookup"><span data-stu-id="d99f3-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d99f3-110">De sourceAnchor waarde voor een gegeven in de lokalen AD object, wordt het kenmerk msDS-ConsistencyGuid configureren voordat deze wordt geïmporteerd in Azure AD verbinden.</span><span class="sxs-lookup"><span data-stu-id="d99f3-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d99f3-111">Raadpleeg voor meer informatie over SourceAnchor en ConsistencyGuid, de volgende: [Azure AD verbinden: concepten ontwerpen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d99f3-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

