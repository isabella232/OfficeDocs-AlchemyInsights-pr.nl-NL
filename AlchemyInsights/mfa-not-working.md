---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545156"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="9be5f-102">Problemen met MFA</span><span class="sxs-lookup"><span data-stu-id="9be5f-102">Issues with MFA</span></span>
<span data-ttu-id="9be5f-103">Er zijn een aantal dingen om te controleren of gebruikers kunnen niet inloggen met multi-factor Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="9be5f-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="9be5f-104">De betrokken gebruiker kan worden geblokkeerd in azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="9be5f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="9be5f-105">Als dat het geval is, wordt verificatiepogingen voor die specifieke gebruiker automatisch geweigerd.</span><span class="sxs-lookup"><span data-stu-id="9be5f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="9be5f-106">Volg de stappen in dit artikel om deze te deblokkeren.</span><span class="sxs-lookup"><span data-stu-id="9be5f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="9be5f-107">Als het deblokkeren van de gebruiker niet Help of de gebruiker niet is geblokkeerd, u proberen om MFA voor de gebruiker opnieuw in te stellen en zij zullen het proces voor inschrijven opnieuw doorlopen.</span><span class="sxs-lookup"><span data-stu-id="9be5f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="9be5f-108">Volg de stappen in dit artikel.</span><span class="sxs-lookup"><span data-stu-id="9be5f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="9be5f-109">Als dit de eerste keer dat u MFA hebt ingeschakeld en uw gebruikers niet kunnen aanmelden bij niet-browsers clients zoals Outlook, Skype, enzovoort, is misschien ADAL (Active Directory Authentication Library) niet ingeschakeld op uw O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="9be5f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="9be5f-110">In dit geval moet u verbinding maken met Exchange Online PowerShell en deze cmdlet uitvoeren:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="9be5f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>