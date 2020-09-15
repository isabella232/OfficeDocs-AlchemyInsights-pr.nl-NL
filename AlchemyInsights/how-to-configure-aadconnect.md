---
title: 646 AADConnect configureren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704484"
---
# <a name="configure-sync-features"></a><span data-ttu-id="b4fbe-102">Synchronisatiefuncties configureren</span><span class="sxs-lookup"><span data-stu-id="b4fbe-102">Configure sync features</span></span>

<span data-ttu-id="b4fbe-103">Azure AD Connect bevat diverse functies die standaard zijn ingeschakeld, of die u later kunt inschakelen.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="b4fbe-104">Voor bepaalde functies is extra configuratie in specifieke omgevingen vereist.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="b4fbe-105">Limieten voor [filteren](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) de objecten worden gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="b4fbe-106">Standaard worden alle gebruikers, contactpersonen, groepen en Windows 10-computeraccounts gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="b4fbe-107">U kunt objecten opnemen of uitsluiten op basis van domeinen, Ou's of andere kenmerken.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="b4fbe-108">[Synchronisatie van wachtwoord hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchroniseert de wachtwoord-hash van de on-premises Active Directory naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="b4fbe-109">Dit betekent dat het wachtwoord op één locatie kan worden gebruikt, maar het gebruik van hetzelfde wachtwoord in zowel on-premises als in Cloud omgevingen.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="b4fbe-110">Aangezien Active Directory de gezaghebbende bron is, kunt u uw eigen wachtwoordbeleid gebruiken.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="b4fbe-111">Met [selfservice voor wachtwoordherstel (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kunnen gebruikers hun eigen wachtwoorden opnieuw instellen in de Cloud, terwijl ze nog steeds uw on-premises wachtwoordbeleid toepassen.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="b4fbe-112">Met [apparaat voor herschrijfing](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kunt u geregistreerde apparaten in azure AD terugschrijven naar de on-premises Active Directory, zodat ze kunnen worden gebruikt voor voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="b4fbe-113">[Onopzettelijke verwijdering voorkomen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is standaard ingeschakeld om te voorkomen dat te veel gelijktijdige objecten worden verwijderd (meer dan 500 objecten per synchronisatie).</span><span class="sxs-lookup"><span data-stu-id="b4fbe-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="b4fbe-114">U kunt deze instelling wijzigen om te voldoen aan de behoeften van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="b4fbe-115">[Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is standaard ingeschakeld voor expres installaties en helpt u ervoor te zorgen dat uw versie van Azure AD Connect altijd up-to-date is.</span><span class="sxs-lookup"><span data-stu-id="b4fbe-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
