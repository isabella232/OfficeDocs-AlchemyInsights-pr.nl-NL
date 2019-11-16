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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b9e25-102">Consistentie/bronanker gedrag</span><span class="sxs-lookup"><span data-stu-id="b9e25-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b9e25-103">Azure AD Connect (versie 1.1.524.0 en na) vereenvoudigt nu het gebruik van msDS-consistentie Cyguid als sourceAnchor kenmerk.</span><span class="sxs-lookup"><span data-stu-id="b9e25-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b9e25-104">Wanneer u deze functie gebruikt, configureert Azure AD Connect automatisch de synchronisatieregels om:</span><span class="sxs-lookup"><span data-stu-id="b9e25-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b9e25-105">Gebruik msDS-consistentie Cyguid als het kenmerk sourceAnchor voor gebruikersobjecten.</span><span class="sxs-lookup"><span data-stu-id="b9e25-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b9e25-106">ObjectGUID wordt gebruikt voor andere objecttypen.</span><span class="sxs-lookup"><span data-stu-id="b9e25-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b9e25-107">Voor een bepaalde on-premises AD-gebruikersobject waarvan het kenmerk msDS-consistentie Cyguid niet is ingevuld, schrijft Azure AD Connect de waarde objectGUID terug naar het kenmerk msDS-consistentie Cyguid in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b9e25-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b9e25-108">Nadat het kenmerk msDS-consistentie Cyguid is ingevuld, Azure AD Connect vervolgens exporteert het object naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b9e25-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b9e25-109">**Opmerking:** Zodra een on-premises AD-object is geïmporteerd in azure AD Connect (dat is, geïmporteerd in de AD-connector ruimte en geprojecteerd in de Metaverse), u de waarde sourceAnchor niet meer wijzigen.</span><span class="sxs-lookup"><span data-stu-id="b9e25-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b9e25-110">Als u de waarde sourceAnchor voor een bepaalde on-premises AD-object, configureert u het kenmerk msDS-consistentie Cyguid voordat deze wordt geïmporteerd in azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b9e25-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b9e25-111">Raadpleeg de volgende onderwerpen voor meer informatie over SourceAnchor en consistentie Cyguid: [Azure AD Connect: ontwerpconcepten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b9e25-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

