---
title: 646 het configureren van AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541580"
---
# <a name="configure-sync-features"></a><span data-ttu-id="88100-102">Synchronisatiefuncties configureren</span><span class="sxs-lookup"><span data-stu-id="88100-102">Configure sync features</span></span>

<span data-ttu-id="88100-103">Azure AD Connect bevat diverse functies die standaard zijn ingeschakeld, of dat u later kunt inschakelen.</span><span class="sxs-lookup"><span data-stu-id="88100-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="88100-104">Sommige functies vereisen aanvullende configuratie specifieke omgevingen.</span><span class="sxs-lookup"><span data-stu-id="88100-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="88100-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limieten voor de objecten worden gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="88100-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="88100-106">Standaard alle gebruikers, contactpersonen, groepen en Windows 10 worden computeraccounts gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="88100-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="88100-107">U kunt opnemen of uitsluiten objecten op basis van domeinen, organisatie-eenheden of andere kenmerken.</span><span class="sxs-lookup"><span data-stu-id="88100-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="88100-108">[Hash Wachtwoordsynchronisatie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoordhash naar Azure AD van Active Directory op gebouwen.</span><span class="sxs-lookup"><span data-stu-id="88100-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="88100-109">Daardoor kan het wachtwoord management op één locatie, maar gebruik van het wachtwoord in beide op gebouwen en cloud-omgevingen.</span><span class="sxs-lookup"><span data-stu-id="88100-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="88100-110">Omdat Active Directory de bindende bron is, kunt u uw eigen instellingen voor wachtwoordbeleid.</span><span class="sxs-lookup"><span data-stu-id="88100-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="88100-111">[Self-wachtwoord opnieuw instellen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kunnen gebruikers hun wachtwoorden in de cloud tijdens het toepassen van het wachtwoordbeleid op de gebouwen nog steeds opnieuw.</span><span class="sxs-lookup"><span data-stu-id="88100-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="88100-112">[Apparaat writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunnen geregistreerde apparaten in Azure AD terug naar Active Directory op de ruimten worden geschreven zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="88100-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="88100-113">[Voorkomen dat per ongeluk wordt verwijderd](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige object verwijderen (meer dan 500 objecten per synchronisatie).</span><span class="sxs-lookup"><span data-stu-id="88100-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="88100-114">U kunt deze instelling om te voldoen aan de behoeften van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="88100-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="88100-115">[Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor snelle installatie en zorgt ervoor dat uw versie van Azure AD verbinden altijd actueel is.</span><span class="sxs-lookup"><span data-stu-id="88100-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
