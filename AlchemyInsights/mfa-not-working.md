---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810479"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="94e9f-102">Problemen met Azure MFA</span><span class="sxs-lookup"><span data-stu-id="94e9f-102">Issues with Azure MFA</span></span>
<span data-ttu-id="94e9f-103">Er zijn een paar dingen om te controleren of gebruikers zich niet kunnen aanmelden met meervoudige verificatie (MFA)</span><span class="sxs-lookup"><span data-stu-id="94e9f-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="94e9f-104">De betreffende gebruiker kan worden geblokkeerd in Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="94e9f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="94e9f-105">Als dat het geval is, worden verificatiepogingen voor die specifieke gebruiker automatisch geweigerd.</span><span class="sxs-lookup"><span data-stu-id="94e9f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="94e9f-106">Volg de stappen in dit artikel om de blokkering te deblokkeren.</span><span class="sxs-lookup"><span data-stu-id="94e9f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="94e9f-107">Als het deblokkeren van de gebruiker niet heeft geholpen of de gebruiker niet is geblokkeerd, kunt u proberen MFA opnieuw in te stellen voor de gebruiker en wordt het registratieproces opnieuw doorlopen.</span><span class="sxs-lookup"><span data-stu-id="94e9f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="94e9f-108">Volg de stappen in dit artikel.</span><span class="sxs-lookup"><span data-stu-id="94e9f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="94e9f-109">Als dit de eerste keer is dat u MFA inschakelen en uw gebruikers zich niet kunnen aanmelden bij niet-browsers,zoals Outlook, Skype, enzovoort, is ADAL (Active Directory Authentication Library) mogelijk niet ingeschakeld op uw O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="94e9f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="94e9f-110">In dit geval moet u verbinding maken met Exchange Online Powershell en deze cmdlet uitvoeren:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="94e9f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>