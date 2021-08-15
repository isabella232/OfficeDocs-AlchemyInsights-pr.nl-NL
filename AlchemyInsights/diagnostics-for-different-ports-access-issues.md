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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030897"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostische gegevens voor toegangsproblemen met verschillende poorten

Voer de volgende stappen uit om de verschillende problemen met poorttoegang op te lossen:

1. Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again. 
2. Controleer de netwerkinstellingen van uw VM om te bepalen of netwerkbeveiligingsgroepen (NSG's) verkeer blokkeren. U kunt ook het hulpprogramma IP-stroomcontrole van Network [Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) gebruiken om te controleren of NSG's het verkeer blokkeren, User-Defined Routes (UR's) om uw verkeer weer on-premises ('Default Route' 0.0.0.0/0) of naar een netwerkapparaat te laten teruggeleiden.
Als u nog steeds problemen hebt na het proberen van de bovenstaande stappen, geeft u de VM-naam en de TCP-poort op waar u e-mail op wilt verzenden voor verdere diagnose.

**Aanbevolen documenten**

[Beperkingen en aanbevelingen voor het verzenden van uitgaande e-mail via poort 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)