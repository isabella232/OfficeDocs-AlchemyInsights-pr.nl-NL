---
title: S/MIME in de webversie van Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772257"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="0e7c8-102">E-mailberichten in Outlook versleutelen</span><span class="sxs-lookup"><span data-stu-id="0e7c8-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="0e7c8-103">Microsoft 365-bericht versleuteling is gebaseerd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="0e7c8-104">Als uw abonnement Azure Rights Management of Azure Information Protection bevat, **hoeft u geen acties te ondernemen om de Rights Management-service handmatig in te schakelen of te activeren** .</span><span class="sxs-lookup"><span data-stu-id="0e7c8-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="0e7c8-105">Op basis van feedback van klanten hebben we geen Exchange-e-mail stroom regels meer voor het automatisch versleutelen van uitgaande e-mail met bepaalde typen gevoelige informatie in uw Tenant.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="0e7c8-106">In plaats daarvan bieden we uitgebreide instructies voor hoe u dit kunt doen met beoordelen.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="0e7c8-107">Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel voor het versleutelen van gevoelige informatie.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="0e7c8-108">Als u de webversie van Outlook (voorheen **OWA**) gebruikt, hoeft u niets **te** doen om een e-mailbericht op te stellen in OWA.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="0e7c8-109">Dit is van toepassing op de machtiging niet doorsturen.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="0e7c8-110">Klik op **machtiging wijzigen** en kies **versleutelen** als u het bericht alleen wilt versleutelen.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="0e7c8-111">Als u de **Outlook-client**gebruikt: als u een versleuteld bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Opties**  >  **Permissions**en selecteert u de gewenste beschermings optie.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="0e7c8-112">Als u **alle e-mail** berichten die naar bepaalde geadresseerden of externe partnerorganisaties zijn verzonden automatisch wilt versleutelen, moet u een transportregel voor de e-mail stroom maken in het Exchange-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="0e7c8-113">In [Dit ondersteunings artikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)vindt u gedetailleerde instructies.</span><span class="sxs-lookup"><span data-stu-id="0e7c8-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

