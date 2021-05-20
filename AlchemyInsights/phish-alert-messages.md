---
title: 2491 E-mailberichten van het beleid 'Phish Delivered due to tenant or user override'
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544573"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="9cc33-102">E-mailberichten waarschuwen vanuit het beleid 'Phish Delivered due to tenant or user override'</span><span class="sxs-lookup"><span data-stu-id="9cc33-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="9cc33-103">Er is een standaardwaarschuwingsbeleid met de naam 'Phish Delivered due to tenant or user override' uitgerold naar tenants met Microsoft Defender voor Office 365 P1- en P2-licenties.</span><span class="sxs-lookup"><span data-stu-id="9cc33-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="9cc33-104">Als u deze waarschuwing hebt ontvangen, volgen de volgende stappen om dit te onderzoeken:</span><span class="sxs-lookup"><span data-stu-id="9cc33-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="9cc33-105">Klik in het waarschuwingsbericht op **Waarschuwing weergeven om** naar de pagina **Waarschuwingen** te gaan in & Compliancecentrum.</span><span class="sxs-lookup"><span data-stu-id="9cc33-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="9cc33-106">Selecteer de waarschuwing om de optie Berichtenlijst weergeven **of** **Berichten weergeven in Verkenner te zien.**</span><span class="sxs-lookup"><span data-stu-id="9cc33-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="9cc33-107">Beide opties brengen u naar de details van het bericht, inclusief de bericht-id.</span><span class="sxs-lookup"><span data-stu-id="9cc33-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="9cc33-108">Houd er rekening mee dat de koppeling Threat Explorer automatisch de berichten filtert die voldoen aan de waarschuwingscriteria.</span><span class="sxs-lookup"><span data-stu-id="9cc33-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="9cc33-109">Mogelijk moet u het datumfilter in Threat Explorer aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9cc33-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="9cc33-110">Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde override:</span><span class="sxs-lookup"><span data-stu-id="9cc33-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="9cc33-111">Een toegestane afzender of domein die door de gebruiker is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="9cc33-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="9cc33-112">Een toegestane afzender of domein die door de beheerder is ingesteld in een antispambeleid.</span><span class="sxs-lookup"><span data-stu-id="9cc33-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="9cc33-113">Een toegestaan IP-adres in een verbindingsfilterbeleid.</span><span class="sxs-lookup"><span data-stu-id="9cc33-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="9cc33-114">Een regel voor de e-mailstroom (ook wel een transportregel genoemd) die is geconfigureerd om berichten toe te staan.</span><span class="sxs-lookup"><span data-stu-id="9cc33-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="9cc33-115">Als u denkt dat het bericht ten onrechte is gemarkeerd als phish, gebruikt u de invoeg Outlook [Rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) om berichtvoorbeelden in te dienen bij Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9cc33-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
