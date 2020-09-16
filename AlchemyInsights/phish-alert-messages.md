---
title: 2491-waarschuwingen voor e-mailberichten van het beleid ' phishing verzonden vanwege Tenant of gebruiker override '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728606"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="24dc3-102">Waarschuwen voor e-mailberichten van het beleid ' phishing is bezorgd vanwege Tenant of gebruiker override '</span><span class="sxs-lookup"><span data-stu-id="24dc3-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="24dc3-103">Een standaard waarschuwings beleid met de naam ' phishing bezorgd vanwege Tenant of gebruiker override ' is uitgerold naar tenants met Office 365 ATP P1 en P2-licenties.</span><span class="sxs-lookup"><span data-stu-id="24dc3-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="24dc3-104">Als u deze melding ontvangt, volgt u deze stappen:</span><span class="sxs-lookup"><span data-stu-id="24dc3-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="24dc3-105">Klik in het waarschuwingsbericht op **melding weergeven** om naar de pagina **waarschuwingen** in het beveiligings & nalevings centrum te gaan.</span><span class="sxs-lookup"><span data-stu-id="24dc3-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="24dc3-106">Selecteer de melding om de optie voor het **weergeven** van berichten **in Verkenner**weer te geven.</span><span class="sxs-lookup"><span data-stu-id="24dc3-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="24dc3-107">Met deze opties kunt u de details van het bericht, inclusief de bericht-ID, volgen.</span><span class="sxs-lookup"><span data-stu-id="24dc3-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="24dc3-108">Houd er rekening mee dat de koppeling bedreigings Verkenner automatisch de berichten filtert die voldoen aan de waarschuwingscriteria.</span><span class="sxs-lookup"><span data-stu-id="24dc3-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="24dc3-109">Mogelijk moet u het datumfilter in de bedreigings Verkenner aanpassen.</span><span class="sxs-lookup"><span data-stu-id="24dc3-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="24dc3-110">Het malafide bericht is bezorgd vanwege een handmatig geconfigureerde Override:</span><span class="sxs-lookup"><span data-stu-id="24dc3-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="24dc3-111">Een toegestane afzender of domein dat is opgegeven door de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="24dc3-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="24dc3-112">Een toegestane afzender of domein dat door de beheerder is ingesteld op een antispambeleid.</span><span class="sxs-lookup"><span data-stu-id="24dc3-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="24dc3-113">Een toegestaan IP-adres in een beleid voor verbindings filters.</span><span class="sxs-lookup"><span data-stu-id="24dc3-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="24dc3-114">Een e-mail stroom regel (ook wel een transportregel genoemd) die is geconfigureerd voor het toestaan van berichten in.</span><span class="sxs-lookup"><span data-stu-id="24dc3-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="24dc3-115">Als u van mening bent dat het bericht onjuist is gemarkeerd als phishing, gebruikt u de [invoegtoepassing rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) in Outlook om bericht voorbeelden bij Microsoft in te dienen.</span><span class="sxs-lookup"><span data-stu-id="24dc3-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
