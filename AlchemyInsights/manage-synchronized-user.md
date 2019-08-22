---
title: Gesynchroniseerde gebruiker beheren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541981"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="05f69-102">Niet primair e-mailadres instellen of wijzigen van gebruikerskenmerken</span><span class="sxs-lookup"><span data-stu-id="05f69-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="05f69-103">Als directory-synchronisatie is ingeschakeld voor uw omgeving, kunnen niet enkele kenmerken van de gebruiker of het object worden gewijzigd met behulp van het Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="05f69-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="05f69-104">Volledig beheer van gesynchroniseerde gebruikers en alle bijbehorende kenmerken, uw lokale active directory-gebruikers en groepen management console gebruiken (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="05f69-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="05f69-105">Ook kunt u afzonderlijke gebruikers of kenmerken voor gesynchroniseerde gebruikers met powershell, zoals weergegeven in de volgende veelvoorkomende voorbeelden:</span><span class="sxs-lookup"><span data-stu-id="05f69-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="05f69-106">Set MsolUser UserPrincipalName - user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="05f69-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="05f69-107">Set MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com' - DisplayName "Het testgebruiker" - Achternaam 'Gebruiker'-titel "Manager"-afdeling "HR"</span><span class="sxs-lookup"><span data-stu-id="05f69-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="05f69-108">Verwijderen MsolUser - UserPrincipalName 'user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="05f69-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>