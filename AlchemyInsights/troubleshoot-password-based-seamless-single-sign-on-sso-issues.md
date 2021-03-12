---
title: Problemen met naadloze eenmalige aanmelding (SSO) met een wachtwoord oplossen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714710"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="ae7a1-102">Problemen met naadloze eenmalige aanmelding (SSO) met een wachtwoord oplossen</span><span class="sxs-lookup"><span data-stu-id="ae7a1-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="ae7a1-103">Zie Wachtwoordgebaseerde verificatie bij Azure Active [Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)voor meer informatie over de basisprincipes van wachtwoordgebaseerde SSO.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="ae7a1-104">**Wachtwoordgebaseerde eenmalige aanmelding configureren**</span><span class="sxs-lookup"><span data-stu-id="ae7a1-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="ae7a1-105">[Eenmalige aanmelding op basis](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) van een wachtwoord configureren: in dit artikel wordt meer informatie besproken over de optie voor eenmalige aanmelding op basis van een wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="ae7a1-106">Als voor de toepassing die u toevoegt een aangepaste configuratie is vereist en u een wachtwoordgebaseerde eenmalige aanmelding moet gebruiken, is dit artikel bedoeld voor u.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="ae7a1-107">[Wachtwoordgebaseerde een-op-een-aanmelding configureren voor on-prem-apps.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) Toepassingsproxy ondersteunt verschillende modi voor een een aanmelding.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="ae7a1-108">Aanmelden via een wachtwoord is bedoeld voor toepassingen die een combinatie van gebruikersnaam en wachtwoord gebruiken voor verificatie.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="ae7a1-109">Wanneer u wachtwoordregistratie voor uw toepassing configureert, moeten uw gebruikers zich eenmaal aanmelden bij de on-premises toepassing.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="ae7a1-110">Daarna worden de aanmeldingsgegevens op slaat Azure Active Directory op en wordt deze automatisch aan de toepassing verstrekt wanneer uw gebruikers deze extern openen.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="ae7a1-111">U moet uw app al hebben gepubliceerd en getest met toepassingsproxy.</span><span class="sxs-lookup"><span data-stu-id="ae7a1-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="ae7a1-112">Als dat niet zo is, volgt u de stappen in Toepassingen publiceren met behulp van Azure AD-toepassingsproxy en gaat u vervolgens verder met uw configuratie van wachtwoordgebaseerde SSO voor on-prem-apps. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)</span><span class="sxs-lookup"><span data-stu-id="ae7a1-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="ae7a1-113">Zie Problemen met eenmalige aanmelding op basis van een wachtwoord [oplossen in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) als u problemen met een wachtwoord voor eenmalige aanmelding wilt oplossen</span><span class="sxs-lookup"><span data-stu-id="ae7a1-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
