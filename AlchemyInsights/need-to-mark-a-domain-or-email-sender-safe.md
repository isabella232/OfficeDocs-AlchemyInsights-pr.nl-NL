---
title: Wilt u een domein of e-mail afzender als veilig markeren?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803240"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f197a-102">Wilt u een domein of e-mail afzender als veilig markeren?</span><span class="sxs-lookup"><span data-stu-id="f197a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f197a-103">Het gebruik van **lijsten met veilige afzenders wordt niet aanbevolen** , omdat het uw organisatie opent tegen spam, phishing en spoofing.</span><span class="sxs-lookup"><span data-stu-id="f197a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f197a-104">Als er echter wel een zakelijke behoefte is, is het **raadzaam** om hiervoor een **[e-mail stroom regels](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f197a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f197a-105">Onze richtlijnen zorgen voor verificatie van de afzender (verifiëren of verzenden van een domein geen Spoofing wordt).</span><span class="sxs-lookup"><span data-stu-id="f197a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f197a-106">**Opmerking**: het wordt afgeraden dat u onware positieven beheert met behulp van lijsten met veilige afzenders, omdat uitzonderingen op spam filteren uw organisatie kan openen tegen beveiligingsaanvallen.</span><span class="sxs-lookup"><span data-stu-id="f197a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f197a-107">Meld **[berichten en bestanden naar Microsoft](https://protection.office.com/reportsubmission)** als uw gebruikers (en) berichten die niet correct zijn gemarkeerd als spam of ongewenste e-mail, willen ontvangen.</span><span class="sxs-lookup"><span data-stu-id="f197a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f197a-108">Veilige afzenders in Outlook, lijst met toegestane afzenders of de lijst met toegestane domeinen in het antispambeleid **moet worden vermeden** omdat afzenders alle spam, spoofing en phishing-bescherming (SPF, dkim, DMARC).</span><span class="sxs-lookup"><span data-stu-id="f197a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f197a-109">Deze methode is het meest geschikt voor tijdelijke tests.</span><span class="sxs-lookup"><span data-stu-id="f197a-109">This method is best used for temporary testing only.</span></span>
