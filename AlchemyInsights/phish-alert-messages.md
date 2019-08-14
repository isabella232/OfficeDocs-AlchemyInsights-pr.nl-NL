---
title: 2491 e-mailberichten van het beleid negeren phishing afgeleverd door de huurder of de gebruiker
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391212"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f5226-102">E-berichten van het beleid negeren phishing afgeleverd door de huurder of de gebruiker</span><span class="sxs-lookup"><span data-stu-id="f5226-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f5226-103">Waarschuwing het standaardbeleid met de naam 'Phishing geleverd door de huurder of de gebruiker overschrijven' is aan huurders met Office 365 ATP ΔP1 en ΔP2 licenties zijn uitgerold.</span><span class="sxs-lookup"><span data-stu-id="f5226-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="f5226-104">Als u deze waarschuwing hebt ontvangen, vindt hier u de stappen uit om te onderzoeken:</span><span class="sxs-lookup"><span data-stu-id="f5226-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f5226-105">Klik op **Waarschuwing weergeven** om te gaan naar de pagina **waarschuwingen** in de & Security Center van de naleving van het waarschuwingsbericht.</span><span class="sxs-lookup"><span data-stu-id="f5226-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f5226-106">Selecteer de waarschuwing voor een overzicht van de optie voor het **weergeven van het bericht** of de **berichten weergeven in de Explorer**.</span><span class="sxs-lookup"><span data-stu-id="f5226-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f5226-107">Met beide opties gaat u naar de details van het bericht, waaronder de bericht-ID.</span><span class="sxs-lookup"><span data-stu-id="f5226-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f5226-108">Houd er rekening mee dat de koppeling bedreiging Explorer de berichten die voldoen aan de waarschuwingscriteria automatisch opnemen.</span><span class="sxs-lookup"><span data-stu-id="f5226-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f5226-109">Mogelijk moet u het datumfilter in gevaar Explorer aanpassen.</span><span class="sxs-lookup"><span data-stu-id="f5226-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f5226-110">Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde overschrijven:</span><span class="sxs-lookup"><span data-stu-id="f5226-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f5226-111">Een toegestane afzender of domein dat is ingesteld door de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="f5226-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f5226-112">Een toegestane afzender of domein dat is ingesteld door de beheerder in een anti-spambeleid.</span><span class="sxs-lookup"><span data-stu-id="f5226-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f5226-113">Een IP-adres in een filter beleid.</span><span class="sxs-lookup"><span data-stu-id="f5226-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f5226-114">Een e-mail stroom regel (ook bekend als een regel vervoer) die zodanig geconfigureerd dat berichten in.</span><span class="sxs-lookup"><span data-stu-id="f5226-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f5226-115">Als u denkt dat het bericht werd ten onrechte gemarkeerd als phishing, gebruik de Outlook [rapportbericht-invoegtoepassing](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) monsters bericht naar Microsoft te verzenden.</span><span class="sxs-lookup"><span data-stu-id="f5226-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
