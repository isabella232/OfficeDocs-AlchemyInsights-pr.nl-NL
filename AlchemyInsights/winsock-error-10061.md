---
title: 1554 Winsock fout 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766164"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="a704a-102">Winsock fout 10061</span><span class="sxs-lookup"><span data-stu-id="a704a-102">Winsock error 10061</span></span>

<span data-ttu-id="a704a-103">Deze foutcode betekent dat Microsoft geen TCP-socket (verbinding) met de doelhost kan maken.</span><span class="sxs-lookup"><span data-stu-id="a704a-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="a704a-104">De meest waarschijnlijke oorzaak van deze fout is een probleem met uw firewallconfiguratie.</span><span class="sxs-lookup"><span data-stu-id="a704a-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="a704a-105">Als u het probleem wilt oplossen, controleert u de volgende instellingen:</span><span class="sxs-lookup"><span data-stu-id="a704a-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="a704a-106">Uw firewallconfiguratie verifiëren met de gegevens in [Microsoft 365-URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="a704a-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="a704a-107">Als de fout specifiek is voor Exchange Online Protection (EOP), moet u eerder op de hoogte zijn gesteld van een wijziging van de [IP-adressen van Exchange Online Protection.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="a704a-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="a704a-108">Controleer of uw internetserviceprovider (ISP) de poort niet blokkeert.</span><span class="sxs-lookup"><span data-stu-id="a704a-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="a704a-109">Controleer de instellingen voor slimme host en doelserver in uw connectors.</span><span class="sxs-lookup"><span data-stu-id="a704a-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="a704a-110">Houd er rekening mee dat Microsoft 365 *inkomende* verbindingen op deze manier niet blokkeert.</span><span class="sxs-lookup"><span data-stu-id="a704a-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
