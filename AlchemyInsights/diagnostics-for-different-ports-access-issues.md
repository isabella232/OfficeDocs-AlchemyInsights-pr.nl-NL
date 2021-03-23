---
title: Diagnostische gegevens voor toegangsproblemen met verschillende poorten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035263"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="a0249-102">Diagnostische gegevens voor toegangsproblemen met verschillende poorten</span><span class="sxs-lookup"><span data-stu-id="a0249-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="a0249-103">Voer de volgende stappen uit om de verschillende problemen met poorttoegang op te lossen:</span><span class="sxs-lookup"><span data-stu-id="a0249-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="a0249-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span><span class="sxs-lookup"><span data-stu-id="a0249-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="a0249-105">Controleer de netwerkinstellingen van uw VM om te bepalen of netwerkbeveiligingsgroepen (NSG's) verkeer blokkeren.</span><span class="sxs-lookup"><span data-stu-id="a0249-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="a0249-106">U kunt ook het hulpprogramma IP-stroomcontrole van Network [Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) gebruiken om te controleren of NSG's het verkeer blokkeren, User-Defined Routes (UR's) om uw verkeer weer on-premises ('Default Route' 0.0.0.0/0) of naar een netwerkapparaat te laten teruggeleiden.</span><span class="sxs-lookup"><span data-stu-id="a0249-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="a0249-107">Als u nog steeds problemen hebt na het proberen van de bovenstaande stappen, geeft u de VM-naam en de TCP-poort op waar u e-mail op wilt verzenden voor verdere diagnose.</span><span class="sxs-lookup"><span data-stu-id="a0249-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="a0249-108">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="a0249-108">**Recommended Documents**</span></span>

[<span data-ttu-id="a0249-109">Beperkingen en aanbevelingen voor het verzenden van uitgaande e-mail via poort 25</span><span class="sxs-lookup"><span data-stu-id="a0249-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)