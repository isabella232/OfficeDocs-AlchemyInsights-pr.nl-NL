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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f0d5d-102">ConsistencyGuid / sourceAnchor gedrag</span><span class="sxs-lookup"><span data-stu-id="f0d5d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f0d5d-103">Azure AD Connect (versie 1.1.524.0 en daarna) vergemakkelijkt nu het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f0d5d-104">Wanneer u deze functie gebruikt, configureert Azure AD Connect automatisch de synchronisatieregels om:</span><span class="sxs-lookup"><span data-stu-id="f0d5d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f0d5d-105">MsDS-ConsistencyGuid gebruiken als het kenmerk sourceAnchor voor gebruikersobjecten.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f0d5d-106">ObjectGUID wordt gebruikt voor andere objecttypen.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f0d5d-107">Voor een bepaald on-premises AD-gebruikersobject waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het kenmerk msDS-ConsistencyGuid in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f0d5d-108">Nadat het kenmerk msDS-ConsistencyGuid is ingevuld, exporteert Azure AD Connect het object naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f0d5d-109">**Let op:** Zodra een on-premises AD-object is geïmporteerd in Azure AD Connect (dat wil zeggen geïmporteerd in de AD-connectorruimte en geprojecteerd in de metaverse), u de bronankerwaarde niet meer wijzigen.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f0d5d-110">Als u de bronAnkerwaarde voor een bepaald on-premises AD-object wilt opgeven, configureert u het kenmerk msDS-ConsistencyGuid voordat het wordt geïmporteerd in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f0d5d-111">Zie voor meer informatie over SourceAnchor en ConsistencyGuid het volgende: [Azure AD Connect: Design concepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f0d5d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

