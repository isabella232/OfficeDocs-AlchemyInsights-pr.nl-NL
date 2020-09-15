---
title: Problemen met e-mail bezorging bij openbare mappen met e-mail oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677923"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="735d1-102">Problemen met e-mail bezorging bij openbare mappen met e-mail oplossen</span><span class="sxs-lookup"><span data-stu-id="735d1-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="735d1-103">Als externe afzenders geen berichten kunnen verzenden naar uw openbare mappen met e-mail en de afzenders ontvangen de fout: is **niet gevonden (550 5.4.1)**, controleert u of het e-mail domein voor de openbare map is geconfigureerd als een intern doorstuur domein in plaats van een gezaghebbend domein:</span><span class="sxs-lookup"><span data-stu-id="735d1-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="735d1-104">Open het [Exchange-Beheercentrum](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="735d1-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="735d1-105">Ga naar geaccepteerde **e-mail stroom** \> **domeinen**, selecteer het geaccepteerde domein en klik vervolgens op **bewerken**.</span><span class="sxs-lookup"><span data-stu-id="735d1-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="735d1-106">Als het domeintype is ingesteld op **gezaghebbend**, wijzigt u op de pagina met **Eigenschappen op de gewenste waarde en klikt** u vervolgens op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="735d1-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="735d1-107">Als externe afzenders de foutmelding krijgt **dat u geen machtiging hebt (550 5.7.13)**, voert u de volgende opdracht uit in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) om de machtigingen voor anonieme gebruikers in de openbare map weer te geven:</span><span class="sxs-lookup"><span data-stu-id="735d1-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="735d1-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Voor `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` Beeld:</span><span class="sxs-lookup"><span data-stu-id="735d1-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="735d1-109">Als u wilt toestaan dat externe gebruikers e-mail verzenden naar deze openbare map, voegt u de CreateItem-toegang rechtstreeks toe aan de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="735d1-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="735d1-110">Bijvoorbeeld `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="735d1-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
