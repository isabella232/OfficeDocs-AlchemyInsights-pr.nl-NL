---
title: Replicaset
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713746"
---
# <a name="replica-set"></a>Replicaset

AADDS wordt ook wel het beheerde domein genoemd. Het zijn eigenlijk twee domeincontrollers die door de back-end worden uitgevoerd en onderhouden. De twee dc's bevatten één dc-hoofd en één replicatie-DC. Back-ups in AADDS (beheerd domein) zijn een geautomatiseerd proces dat wordt beheerd door het Azure-platform. In het geval van een probleem met uw beheerde domein, kan Azure-ondersteuning u helpen bij het terugzetten van de back-up.

U maakt elke replicaset in een virtueel netwerk. Elk virtueel netwerk moet worden doorge peerd naar elk ander virtueel netwerk dat de replicaset van een beheerd domein host. Met deze configuratie wordt een mesh-netwerktopologie gemaakt die adreslijstreplicatie ondersteunt. Een virtueel netwerk kan meerdere replicasets ondersteunen, mits elke replicaset zich in een ander virtueel subnet plaatst.

Zie Concepten replicasets voor meer informatie over [de replicaset.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
