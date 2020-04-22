---
title: Problemen met e-mailbezorging oplossen in openbare mappen met e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716347"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="6dac0-102">Problemen met e-mailbezorging oplossen in openbare mappen met e-mail</span><span class="sxs-lookup"><span data-stu-id="6dac0-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="6dac0-103">Als externe afzenders geen berichten naar uw openbare mappen met e-mail kunnen verzenden en de afzenders de fout ontvangen: **kan niet worden gevonden (550 5.4.1),** controleert u of het e-maildomein voor de openbare map is geconfigureerd als een intern relaydomein in plaats van een gezaghebbend domein:</span><span class="sxs-lookup"><span data-stu-id="6dac0-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="6dac0-104">Open het [Exchange-beheercentrum (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="6dac0-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="6dac0-105">Ga naar **Geaccepteerde domeinen** **e-mail,** \> selecteer het geaccepteerde domein en klik op **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="6dac0-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="6dac0-106">Als het domeintype op de pagina eigenschappen wordt geopend, **wijzigt**u de waarde in **Intern relay** en klikt u op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="6dac0-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="6dac0-107">Als externe afzenders de fout ontvangen **die u niet hebt (550 5.7.13),** voert u de volgende opdracht uit in Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) om de machtigingen voor anonieme gebruikers in de openbare map te bekijken:</span><span class="sxs-lookup"><span data-stu-id="6dac0-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="6dac0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Bijvoorbeeld. `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`</span><span class="sxs-lookup"><span data-stu-id="6dac0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="6dac0-109">Als u externe gebruikers wilt toestaan e-mail naar deze openbare map te verzenden, voegt u het toegangsrecht voor Items maken toe aan de gebruiker Anoniem.</span><span class="sxs-lookup"><span data-stu-id="6dac0-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="6dac0-110">Bijvoorbeeld `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="6dac0-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
