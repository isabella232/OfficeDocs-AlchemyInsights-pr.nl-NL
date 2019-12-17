---
title: S/MIME in Outlook op het web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053220"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="4b672-102">Codeer e-mail berichten in Outlook</span><span class="sxs-lookup"><span data-stu-id="4b672-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="4b672-103">Office 365-bericht versleuteling is gebaseerd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="4b672-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="4b672-104">Als uw abonnement Azure Rights Management of Azure Information Protection bevat, **hoeft u geen acties uit te voeren om de Rights Management-service handmatig in te schakelen of te activeren** .</span><span class="sxs-lookup"><span data-stu-id="4b672-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="4b672-105">Op basis van feedback van klanten, zullen we niet langer inschakelen Exchange mail flow regels voor het automatisch coderen van uitgaande e-mail met een bepaald type gevoelige informatie in uw Tenant standaard.</span><span class="sxs-lookup"><span data-stu-id="4b672-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="4b672-106">In plaats daarvan geven we gedetailleerde instructies over hoe je dat zelf doen.</span><span class="sxs-lookup"><span data-stu-id="4b672-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="4b672-107">Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel voor het versleutelen van gevoelige informatie.</span><span class="sxs-lookup"><span data-stu-id="4b672-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="4b672-108">Als u Outlook op het web (voorheen **OWA**): wanneer u een e-mail bericht opstelt, klikt u op **beveiligen** in OWA.</span><span class="sxs-lookup"><span data-stu-id="4b672-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="4b672-109">Dit is van toepassing op de machtiging ' niet doorsturen '.</span><span class="sxs-lookup"><span data-stu-id="4b672-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="4b672-110">Klik op **machtiging wijzigen** en kies **coderen** om het bericht alleen te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="4b672-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="4b672-111">Als u **Outlook-client**gebruikt: als u een gecodeerd bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Opties** > **machtigingen**en selecteert u vervolgens de gewenste beveiligingsoptie.</span><span class="sxs-lookup"><span data-stu-id="4b672-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="4b672-112">Als u **alle e-mail** die is verzonden naar bepaalde geadresseerden of externe partnerorganisaties automatisch wilt coderen, moet u een regel voor het transport van e-mail berichten in het Beheercentrum van Exchange maken.</span><span class="sxs-lookup"><span data-stu-id="4b672-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="4b672-113">Gedetailleerde instructies zijn beschikbaar in [dit ondersteuningsartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="4b672-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

