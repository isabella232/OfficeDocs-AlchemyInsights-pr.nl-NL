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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="e997d-102">ConsistencyGuid/sourceAnchor gedrag</span><span class="sxs-lookup"><span data-stu-id="e997d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="e997d-103">Azure AD Connect (versie 1.1.524.0 en After) vergemakkelijkt het gebruik van msDS-ConsistencyGuid als sourceAnchor-kenmerk.</span><span class="sxs-lookup"><span data-stu-id="e997d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="e997d-104">Wanneer u deze functie gebruikt, worden in azure AD Connect automatisch de synchronisatieregels geconfigureerd voor:</span><span class="sxs-lookup"><span data-stu-id="e997d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="e997d-105">Gebruik msDS-ConsistencyGuid als het sourceAnchor-kenmerk voor gebruikersobjecten.</span><span class="sxs-lookup"><span data-stu-id="e997d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="e997d-106">ObjectGUID wordt gebruikt voor andere objecttypen.</span><span class="sxs-lookup"><span data-stu-id="e997d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="e997d-107">Voor een bepaald on-premises AD User object waarvan het kenmerk msDS-ConsistencyGuid niet is ingevuld, schrijft Azure AD Connect de objectGUID-waarde terug naar het kenmerk msDS-ConsistencyGuid in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e997d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="e997d-108">Nadat het kenmerk msDS-ConsistencyGuid is ingevuld, wordt het object in azure AD Connect vervolgens geëxporteerd naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e997d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="e997d-109">**Opmerking:** Wanneer een on-premises AD-object wordt geïmporteerd in azure AD Connect (dat wil zeggen dat het wordt geïmporteerd in de AD connector-ruimte en de geprojecteerde tekst in de standaardtekst), kunt u de sourceAnchor waarde niet meer wijzigen.</span><span class="sxs-lookup"><span data-stu-id="e997d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="e997d-110">Als u de sourceAnchor waarde wilt opgeven voor een bepaald on-premises AD-object, configureert u het kenmerk msDS-ConsistencyGuid voordat het wordt geïmporteerd in azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e997d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="e997d-111">Ga voor meer informatie over SourceAnchor en ConsistencyGuid naar de volgende informatie: [Azure AD Connect: ontwerp concepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="e997d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

