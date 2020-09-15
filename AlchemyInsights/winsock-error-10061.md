---
title: 1554 Winsock-fout 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698857"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c875a-102">Winsock-fout 10061</span><span class="sxs-lookup"><span data-stu-id="c875a-102">Winsock error 10061</span></span>

<span data-ttu-id="c875a-103">Deze foutcode betekent dat Microsoft geen TCP-socket (verbinding) met de target-host kon maken.</span><span class="sxs-lookup"><span data-stu-id="c875a-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c875a-104">De meest waarschijnlijke oorzaak van deze fout is een probleem met de firewallconfiguratie.</span><span class="sxs-lookup"><span data-stu-id="c875a-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c875a-105">Ga als volgt te werk om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="c875a-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c875a-106">De firewallconfiguratie controleren met de gegevens in [url's en IP-adresbereiken voor Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c875a-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c875a-107">Als de fout specifiek is voor Exchange Online Protection (EOP), moet u eerder op de hoogte zijn van een wijziging in de [IP-adressen voor Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c875a-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c875a-108">Controleer of uw internetprovider (ISP) de poort niet blokkeert.</span><span class="sxs-lookup"><span data-stu-id="c875a-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c875a-109">Controleer de instellingen voor de Smart host en de doelserver in de connectors.</span><span class="sxs-lookup"><span data-stu-id="c875a-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c875a-110">Houd er rekening mee dat Microsoft 365 *binnenkomende* verbindingen op deze manier niet blokkeert.</span><span class="sxs-lookup"><span data-stu-id="c875a-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
