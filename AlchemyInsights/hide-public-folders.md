---
title: Openbare mappen verbergen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315339"
---
# <a name="hide-public-folders"></a>Openbare mappen verbergen

**De volledige structuur van openbare mappen verbergen:**

Gebruik de stappen in [dit artikel](https://aka.ms/ControlPF) om de volledige structuur van openbare mappen te verbergen voor selectieve of alle gebruikers.

**Een specifieke openbare map verbergen:**

1. Machtigingen toevoegen voor gebruikers die toegang moeten hebben tot de openbare map

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Verwijder de gebruiker **Standaard uit** de **machtigingenlijst:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
