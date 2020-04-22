---
title: S/MIME in de webversie van Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764867"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="23f70-102">E-mailberichten versleutelen in Outlook</span><span class="sxs-lookup"><span data-stu-id="23f70-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="23f70-103">Microsoft 365-berichtversleuteling is gebouwd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="23f70-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="23f70-104">Als uw abonnement Azure Rights Management of Azure Information Protection bevat, hoeft u geen acties uit te voeren om de Rights Management Service **handmatig in te schakelen of te activeren.**</span><span class="sxs-lookup"><span data-stu-id="23f70-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="23f70-105">Op basis van feedback van klanten kunnen de Exchange-mailstroomregels niet langer automatisch uitgaande e-mail versleutelen die standaard bepaalde soorten gevoelige informatie in uw tenant bevat.</span><span class="sxs-lookup"><span data-stu-id="23f70-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="23f70-106">In plaats daarvan geven we gedetailleerde instructies over hoe jullie dat zelf kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="23f70-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="23f70-107">Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel om gevoelige informatie te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="23f70-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="23f70-108">Als u Outlook on the Web gebruikt (voorheen **OWA):** Klik bij het opstellen van een e-mailbericht op **Beveiligen** in OWA.</span><span class="sxs-lookup"><span data-stu-id="23f70-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="23f70-109">Dit geldt voor "Niet doorsturen" toestemming.</span><span class="sxs-lookup"><span data-stu-id="23f70-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="23f70-110">Klik **op Machtigingen wijzigen** en kies **Versleutelen** om het bericht alleen te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="23f70-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="23f70-111">Als u **Outlook-client gebruikt:** Als u outlook-client wilt gebruiken: als u een versleuteld bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Optiesmachtigingen** > **Permissions**en selecteert u de gewenste beveiligingsoptie.</span><span class="sxs-lookup"><span data-stu-id="23f70-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="23f70-112">Als u **alle e-mail die** naar bepaalde ontvangers of externe partnerorganisaties wordt verzonden, automatisch wilt versleutelen, moet u een regel voor het transport van e-mailstromen maken in het Exchange-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="23f70-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="23f70-113">Gedetailleerde instructies zijn opgenomen in [dit ondersteuningsartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="23f70-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

