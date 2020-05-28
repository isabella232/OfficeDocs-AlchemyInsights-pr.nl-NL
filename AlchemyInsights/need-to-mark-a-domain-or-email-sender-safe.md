---
title: Wilt u een domein of e-mailafzender veilig markeren?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281143"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f3626-102">Wilt u een domein of e-mailafzender veilig markeren?</span><span class="sxs-lookup"><span data-stu-id="f3626-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f3626-103">Het gebruik van lijsten met **veilige afzenders wordt niet aanbevolen** omdat het uw organisatie openstelt voor spam-, phish- en spoofing-aanvallen.</span><span class="sxs-lookup"><span data-stu-id="f3626-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f3626-104">Als er echter een zakelijke vereiste is, raden we **u aan** **[hiervoor e-mailstroomregels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f3626-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f3626-105">Onze richtlijnen zorgen ervoor dat afzenderverificatie (controleert of het verzenden van domein niet wordt vervalst).</span><span class="sxs-lookup"><span data-stu-id="f3626-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f3626-106">**Opmerking:** We raden u aan valse positieven te beheren door veilige afzenderlijsten te gebruiken, omdat uitzonderingen op spamfiltering uw organisatie kunnen openen voor beveiligingsaanvallen.</span><span class="sxs-lookup"><span data-stu-id="f3626-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f3626-107">Als uw gebruiker(s) berichten ontvangt die onjuist zijn gemarkeerd als spam of ongewenste e-mail, u **[berichten en bestanden rapporteren aan Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="f3626-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f3626-108">Veilige afzenders in Outlook, Toegestane afzenderlijst of toegestane domeinlijst in antispambeleid **moeten worden vermeden** omdat afzenders alle spam-, spoof- en phish-beveiliging en afzenderverificatie (SPF, DKIM, DMARC) omzeilen.</span><span class="sxs-lookup"><span data-stu-id="f3626-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f3626-109">Deze methode wordt het best alleen gebruikt voor tijdelijke tests.</span><span class="sxs-lookup"><span data-stu-id="f3626-109">This method is best used for temporary testing only.</span></span>
