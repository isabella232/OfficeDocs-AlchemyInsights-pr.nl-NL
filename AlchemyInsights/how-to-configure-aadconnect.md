---
title: 646 AadConnect configureren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722528"
---
# <a name="configure-sync-features"></a><span data-ttu-id="b1ab0-102">Synchronisatiefuncties configureren</span><span class="sxs-lookup"><span data-stu-id="b1ab0-102">Configure sync features</span></span>

<span data-ttu-id="b1ab0-103">Azure AD Connect bevat verschillende functies die standaard zijn ingeschakeld of die u later inschakelen.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="b1ab0-104">Sommige functies vereisen extra configuratie in specifieke omgevingen.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="b1ab0-105">[Filterlimieten de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objecten worden gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="b1ab0-106">Standaard worden alle gebruikers, contactpersonen, groepen en Windows 10-computeraccounts gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="b1ab0-107">U objecten opnemen of uitsluiten op basis van domeinen, OU's of andere kenmerken.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="b1ab0-108">[Synchronisatie van wachtwoordhash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoordhash van de on-premises Active Directory naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="b1ab0-109">Dit maakt wachtwoordbeheer op één locatie mogelijk, maar het gebruik van hetzelfde wachtwoord in zowel on-premises als cloudomgevingen.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="b1ab0-110">Omdat Active Directory de gezaghebbende bron is, u uw eigen wachtwoordbeleid gebruiken.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="b1ab0-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) stelt gebruikers in staat om hun eigen wachtwoorden opnieuw in de cloud te resetten terwijl ze nog steeds uw on-premises wachtwoordbeleid toepassen.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="b1ab0-112">[Met apparaatterugschrijftijd](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunnen geregistreerde apparaten in Azure AD worden teruggeschreven naar de on-premises Active Directory, zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="b1ab0-113">[Voorkomen dat per ongeluk worden](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) verwijderd, is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige objectverwijderingen (meer dan 500 objecten per synchronisatie) worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="b1ab0-114">U deze instelling wijzigen om aan de behoeften van uw organisatie te voldoen.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="b1ab0-115">[Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor expresinstallaties en zorgt ervoor dat uw versie van Azure AD Connect altijd actueel is.</span><span class="sxs-lookup"><span data-stu-id="b1ab0-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
