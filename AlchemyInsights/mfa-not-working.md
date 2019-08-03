---
title: Problemen met de MVR gesloten
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250160"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="0eb6c-102">Problemen met de MVR gesloten</span><span class="sxs-lookup"><span data-stu-id="0eb6c-102">Issues with MFA</span></span>
<span data-ttu-id="0eb6c-103">Er zijn een paar dingen om te controleren als gebruikers kunnen zich niet aanmelden met behulp van meerledige verificatie (MVR gesloten)</span><span class="sxs-lookup"><span data-stu-id="0eb6c-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="0eb6c-104">De gebruiker kan worden geblokkeerd in Azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="0eb6c-105">Als dit het geval is, probeert verificatie voor die specifieke gebruiker automatisch worden geweigerd.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="0eb6c-106">Volg de stappen in dit artikel om de blokkering op te heffen.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="0eb6c-107">Als de gebruiker deblokkeren hebt gehad of niet door de gebruiker is geblokkeerd opnieuw instellen van de MVR gesloten voor de gebruiker kunt u proberen en ze weer inschrijven bij het opnieuw.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="0eb6c-108">Volg de stappen in dit artikel.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="0eb6c-109">Als dit de eerste keer dat u ingeschakelde MVR gesloten en uw gebruikers zich niet aanmelden bij niet-browsers van clients zoals Outlook, Skype, enz, is misschien ADAL (Active Directory-verificatie Library) niet ingeschakeld op uw abonnement O365.</span><span class="sxs-lookup"><span data-stu-id="0eb6c-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="0eb6c-110">In dit geval moet u verbinding maken met Exchange Online Powershell en voer deze cmdlet:  *Set OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="0eb6c-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>