---
title: Toewijzing van aan de gebruiker ingerichte kenmerk
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949698"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="ed909-102">Toewijzing van aan de gebruiker ingerichte kenmerk</span><span class="sxs-lookup"><span data-stu-id="ed909-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="ed909-103">Als u problemen met bekende kenmerktoewijzingen wilt oplossen, raadpleegt u [kenmerktoewijzingen](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="ed909-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="ed909-104">Microsoft Azure Active Directory (AD) biedt ondersteuning voor gebruikers die toegang bieden tot SaaS-toepassingen van derden, zoals Salesforce, G suite en andere.</span><span class="sxs-lookup"><span data-stu-id="ed909-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="ed909-105">Als u het inrichten van de gebruiker inschakelt voor een SaaS-toepassing van derden, beheert de Azure-Portal zijn kenmerkwaarden via kenmerktoewijzingen.</span><span class="sxs-lookup"><span data-stu-id="ed909-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="ed909-106">Als u wilt weten hoe u de standaardtoewijzingen van kenmerken aanpast, raadpleegt u [kenmerk gebruikers inrichten voor de Gebruikerstoewijzing van de SaaS-toepassingen in azure Active Directory aanpassen](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="ed909-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="ed909-107">Als u meer wilt weten over het inrichten van de SaaS-app van gebruikers, raadpleegt u [Wat is de geautomatiseerde SaaS-app voor gebruikers in azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ed909-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="ed909-108">Wanneer u kenmerktoewijzingen aanpast voor het inrichten van de gebruiker, kan het kenmerk dat u wilt toewijzen niet worden weergegeven in de bronkenmerk lijst.</span><span class="sxs-lookup"><span data-stu-id="ed909-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="ed909-109">Wanneer u [een kenmerk vanuit uw on-premises Active Directory naar Azure AD synchroniseert voor de levering aan een toepassings](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikel, leest u hoe u het ontbrekende kenmerk toevoegt door het te synchroniseren vanuit uw on-PREMISes advertentie in azure AD.</span><span class="sxs-lookup"><span data-stu-id="ed909-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
