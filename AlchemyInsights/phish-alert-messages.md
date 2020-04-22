---
title: 2491 Waarschuwingse-mailberichten van het beleid 'Phish Delivered due to tenant or user override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758903"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="b1288-102">E-mailberichten waarschuwen van het beleid 'Phish Delivered due to tenant or user override'</span><span class="sxs-lookup"><span data-stu-id="b1288-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="b1288-103">Er is een standaardwaarschuwingsbeleid met de naam 'Phish Delivered due to tenant or user override' uitgerold naar tenants met Office 365 ATP P1- en P2-licenties.</span><span class="sxs-lookup"><span data-stu-id="b1288-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="b1288-104">Als u deze waarschuwing hebt ontvangen, zijn de stappen die u moet onderzoeken:</span><span class="sxs-lookup"><span data-stu-id="b1288-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="b1288-105">Klik in het waarschuwingsbericht op **Waarschuwing weergeven** om naar de pagina **Waarschuwingen** in het beveiligings- & Compliance Center te gaan.</span><span class="sxs-lookup"><span data-stu-id="b1288-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="b1288-106">Selecteer de waarschuwing om de optie te zien om **de berichtenlijst** weer te geven of **Berichten weer geven in Explorer**.</span><span class="sxs-lookup"><span data-stu-id="b1288-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="b1288-107">Beide opties brengen u naar de details van het bericht, waaronder de Message ID.</span><span class="sxs-lookup"><span data-stu-id="b1288-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="b1288-108">Houd er rekening mee dat de koppeling Threat Explorer automatisch de berichten filtert die overeenkomen met de waarschuwingscriteria.</span><span class="sxs-lookup"><span data-stu-id="b1288-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="b1288-109">Mogelijk moet u het datumfilter in Threat Explorer aanpassen.</span><span class="sxs-lookup"><span data-stu-id="b1288-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="b1288-110">Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde overschrijving:</span><span class="sxs-lookup"><span data-stu-id="b1288-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="b1288-111">Een toegestane afzender of domein ingesteld door de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="b1288-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="b1288-112">Een toegestane afzender of domein die door de beheerder is ingesteld in een antispambeleid.</span><span class="sxs-lookup"><span data-stu-id="b1288-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="b1288-113">Een toegestaan IP-adres in een verbindingsfilterbeleid.</span><span class="sxs-lookup"><span data-stu-id="b1288-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="b1288-114">Een regel voor e-mailstroom (ook wel transportregel genoemd) die is geconfigureerd om berichten toe te laten.</span><span class="sxs-lookup"><span data-stu-id="b1288-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="b1288-115">Als u van mening bent dat het bericht onjuist is gemarkeerd als phish, gebruikt u de [invoegtoepassing Outlook-rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) om berichtvoorbeelden naar Microsoft in te dienen.</span><span class="sxs-lookup"><span data-stu-id="b1288-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
