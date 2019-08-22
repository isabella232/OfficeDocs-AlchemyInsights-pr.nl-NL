---
title: E-mail levering problemen oplossen naar e-mailadres van openbare mappen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525094"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="b088e-102">E-mail levering problemen oplossen naar e-mailadres van openbare mappen</span><span class="sxs-lookup"><span data-stu-id="b088e-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="b088e-103">Externe afzenders geen berichten verzenden naar uw e-mailadres openbare mappen als de afzenders, wordt het foutbericht: **(550 5.4.1) niet is gevonden**, controleert u of het e-maildomein voor de openbare map is geconfigureerd als een intern relay-domein in plaats van een gezaghebbende domein:</span><span class="sxs-lookup"><span data-stu-id="b088e-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="b088e-104">Open het [beheercentrum van Exchange (SBV)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b088e-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="b088e-105">Ga naar de **e-mailstroom** \> **geaccepteerde domeinen**, selecteert u het geaccepteerde domein en klik vervolgens op **bewerken**.</span><span class="sxs-lookup"><span data-stu-id="b088e-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="b088e-106">In de eigenschappen pagina die wordt geopend als het domeintype **bindend**, wijzig de waarde in **interne relay** en klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="b088e-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="b088e-107">Als externe afzenders ontvangt de fout- **u hebt geen machtiging (550 5.7.13)**, moet u de volgende opdracht uitvoeren in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) om te zien welke machtigingen voor anonieme gebruikers in de openbare map:</span><span class="sxs-lookup"><span data-stu-id="b088e-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="b088e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Bijvoorbeeld `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="b088e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="b088e-109">Zodat externe gebruikers e-mail verzenden naar deze openbare map toevoegen de CreateItems toegang aan de gebruiker anoniem.</span><span class="sxs-lookup"><span data-stu-id="b088e-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="b088e-110">Bijvoorbeeld `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="b088e-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
