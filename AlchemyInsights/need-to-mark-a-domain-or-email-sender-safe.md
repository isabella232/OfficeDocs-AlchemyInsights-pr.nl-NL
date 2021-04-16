---
title: Wilt u een domein of e-mail afzender veilig markeren?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792127"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="90e5a-102">Wilt u een domein of e-mail afzender veilig markeren?</span><span class="sxs-lookup"><span data-stu-id="90e5a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="90e5a-103">Het gebruik **van lijsten met veilige afzenders wordt** niet aanbevolen, omdat uw organisatie hiermee wordt geopend voor spam-, phish- en spoofing-aanvallen.</span><span class="sxs-lookup"><span data-stu-id="90e5a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="90e5a-104">Als er echter een zakelijke vereiste is, **raden** we u aan hiervoor **[E-mailstroomregels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="90e5a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="90e5a-105">Onze richtlijnen zorgen ervoor dat afzenderverificatie (controleert of verzendend domein niet wordt vervalst).</span><span class="sxs-lookup"><span data-stu-id="90e5a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="90e5a-106">**Opmerking:** Het is niet raadzaam om false positives te beheren met behulp van lijsten met veilige afzenders, omdat uitzonderingen op spamfilters uw organisatie kunnen openen voor beveiligingsaanvallen.</span><span class="sxs-lookup"><span data-stu-id="90e5a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="90e5a-107">Als uw gebruikers berichten ontvangen die onjuist zijn gemarkeerd als spam of ongewenste e-mail, kunt u berichten en bestanden **[rapporteren aan Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="90e5a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="90e5a-108">Veilige afzenders in Outlook, lijst met toegestane afzenders  of toegestane domeinlijst in antispambeleid moeten worden vermeden omdat afzenders alle spam-, spoof- en phish-beveiliging en afzenderverificatie (SPF, DKIM, DMARC) omzeilen.</span><span class="sxs-lookup"><span data-stu-id="90e5a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="90e5a-109">Deze methode wordt het beste alleen gebruikt voor tijdelijke tests.</span><span class="sxs-lookup"><span data-stu-id="90e5a-109">This method is best used for temporary testing only.</span></span>
