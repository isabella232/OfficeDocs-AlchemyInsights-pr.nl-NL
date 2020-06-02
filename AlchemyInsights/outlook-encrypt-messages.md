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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511503"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2de0b-102">E-mailberichten versleutelen in Outlook</span><span class="sxs-lookup"><span data-stu-id="2de0b-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2de0b-103">Microsoft 365 Message Encryption is gebouwd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="2de0b-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2de0b-104">Als uw abonnement Azure Rights Management of Azure Information Protection bevat, hoeft u geen acties te ondernemen om de Rights Management Service **handmatig in te schakelen of te activeren.**</span><span class="sxs-lookup"><span data-stu-id="2de0b-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2de0b-105">Op basis van feedback van klanten kunnen we exchange-e-mailstroomregels niet langer in staat stellen om uitgaande e-mail met bepaalde soorten gevoelige informatie in uw tenant standaard automatisch te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="2de0b-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2de0b-106">In plaats daarvan geven we gedetailleerde instructies over hoe jullie dit zelf kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="2de0b-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2de0b-107">Zie [dit artikel voor](https://aka.ms/OmeEtr)meer informatie over het maken van een transportregel om gevoelige informatie te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="2de0b-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2de0b-108">Als u Outlook on the Web gebruikt (voorheen **OWA):** Wanneer u een e-mailbericht opstelt, klikt u op **Beveiligen** in OWA.</span><span class="sxs-lookup"><span data-stu-id="2de0b-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2de0b-109">Dit is van toepassing "Niet doorsturen" toestemming.</span><span class="sxs-lookup"><span data-stu-id="2de0b-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2de0b-110">Klik **op Machtiging wijzigen** en kies **Versleutelen** om alleen het bericht te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="2de0b-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2de0b-111">Als u Outlook-client gebruikt: Als u **Outlook-client**gebruikt: Als u outlook 2013 of 2016 of Outlook 2016 voor Mac wilt verzenden: selecteert u **Options**  >  **Optiesmachtigingen**en selecteert u de beveiligingsoptie die u nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="2de0b-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2de0b-112">Als u **alle e-mail die** naar bepaalde ontvangers of externe partnerorganisaties wordt verzonden, automatisch wilt versleutelen, moet u een regel voor e-mailstroomtransport maken in het Exchange-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="2de0b-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2de0b-113">Gedetailleerde instructies worden gegeven in [dit ondersteuningsartikel.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="2de0b-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

