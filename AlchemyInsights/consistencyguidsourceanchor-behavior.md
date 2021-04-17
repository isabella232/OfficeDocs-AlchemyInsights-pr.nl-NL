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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="c4457-102">ConsistencyGuid /sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="c4457-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="c4457-103">Azure AD Connect (versie 1.1.524.0 en daarna) faciliteert nu het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk.</span><span class="sxs-lookup"><span data-stu-id="c4457-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="c4457-104">Wanneer u deze functie gebruikt, worden de synchronisatieregels automatisch geconfigureerd door Azure AD Connect:</span><span class="sxs-lookup"><span data-stu-id="c4457-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="c4457-105">MsDS-ConsistencyGuid gebruiken als het sourceAnchor-kenmerk voor gebruikersobjecten.</span><span class="sxs-lookup"><span data-stu-id="c4457-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="c4457-106">ObjectGUID wordt gebruikt voor andere objecttypen.</span><span class="sxs-lookup"><span data-stu-id="c4457-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="c4457-107">Voor elk on-premises AD-gebruikersobject waarvan het msDS-ConsistencyGuid-kenmerk niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het msDS-ConsistencyGuid-kenmerk in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c4457-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="c4457-108">Nadat het msDS-ConsistencyGuid-kenmerk is ingevuld, exporteert Azure AD Connect het object vervolgens naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c4457-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="c4457-109">**Opmerking:** Wanneer een on-premises AD-object is geïmporteerd in Azure AD Connect (dat wil zeggen, geïmporteerd in de AD Connector-ruimte en geprojecteerd in de Metaverse), kunt u de bronwaardeAnchor niet meer wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c4457-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="c4457-110">Als u de bronwaardeAnchor wilt opgeven voor een bepaald on-premises AD-object, configureert u het msDS-ConsistencyGuid-kenmerk voordat het wordt geïmporteerd in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c4457-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="c4457-111">Voor meer informatie over SourceAnchor en ConsistencyGuid raadpleegt u het volgende: [Azure AD Connect: Ontwerpconcepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="c4457-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

