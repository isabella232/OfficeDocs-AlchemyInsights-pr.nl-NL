---
title: Configuratie van app-proxy
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884947"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="f8d5f-102">Configuratie van app-proxy</span><span class="sxs-lookup"><span data-stu-id="f8d5f-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="f8d5f-103">Als u wilt weten hoe u een toepassingsproxy toepassing kunt configureren in azure AD zodat u uw on-premises toepassingen kunt weergeven in de Cloud, leest u [hoe u een toepassing van de toepassing proxy kunt configureren](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="f8d5f-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="f8d5f-104">Eenmalige aanmelding (SSO) Hiermee kunnen uw gebruikers toegang krijgen tot een toepassing zonder verificatie meerdere keren.</span><span class="sxs-lookup"><span data-stu-id="f8d5f-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="f8d5f-105">U kunt de authenticatie van de toepassing in de Cloud afronden op Azure Active Directory, zodat de service of connector de gebruiker kan imiteren om eventuele extra authenticatie van de toepassing te voltooien.</span><span class="sxs-lookup"><span data-stu-id="f8d5f-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="f8d5f-106">Voor meer informatie raadpleegt u [eenmalige aanmelding configureren voor een toepassing van de toepassings proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="f8d5f-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="f8d5f-107">Gebruik [dit artikel](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) om veelvoorkomende problemen met personen te verhelpen bij het maken van een nieuwe toepassing voor toepassingsproxy.</span><span class="sxs-lookup"><span data-stu-id="f8d5f-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="f8d5f-108">Als u problemen ondervindt bij het instellen van een back-end-authenticatie voor uw toepassing, moet u mogelijk problemen met de [Kerberos-beperkte delegering voor de toepassings proxy oplossen](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) of de richtlijnen volgen voor het [configureren van de toepassing met PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) voor het oplossen van het probleem.</span><span class="sxs-lookup"><span data-stu-id="f8d5f-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
