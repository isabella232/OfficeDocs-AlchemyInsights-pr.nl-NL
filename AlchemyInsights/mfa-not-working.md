---
title: Problemen met MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755126"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="515c7-102">Problemen met Azure MFA</span><span class="sxs-lookup"><span data-stu-id="515c7-102">Issues with Azure MFA</span></span>
<span data-ttu-id="515c7-103">Er zijn enkele dingen die u kunt controleren als gebruikers zich niet kunnen aanmelden met multi-factor Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="515c7-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="515c7-104">De betrokken gebruiker wordt mogelijk geblokkeerd in azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="515c7-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="515c7-105">Als dat het geval is, worden verificatiepogingen voor die specifieke gebruiker automatisch geweigerd.</span><span class="sxs-lookup"><span data-stu-id="515c7-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="515c7-106">Voer de stappen in dit artikel uit om ze te deblokkeren.</span><span class="sxs-lookup"><span data-stu-id="515c7-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="515c7-107">Als het deblokkeren van de gebruiker niet is gelukt of als de gebruiker niet is geblokkeerd, kunt u proberen MFA opnieuw in te stellen voor de gebruiker, zodat ze opnieuw de registratieprocedure doorlopen.</span><span class="sxs-lookup"><span data-stu-id="515c7-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="515c7-108">Voer de stappen in dit artikel uit.</span><span class="sxs-lookup"><span data-stu-id="515c7-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="515c7-109">Als dit de eerste keer is dat u MFA inschakelt en uw gebruikers niet kunnen inloggen met niet-browsers, zoals Outlook, Skype, etc, of ADAL (Active Directory Authentication Library), is niet ingeschakeld voor uw O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="515c7-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="515c7-110">In dit geval dient u verbinding te maken met Exchange Online PowerShell en deze cmdlet uit te voeren:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="515c7-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>