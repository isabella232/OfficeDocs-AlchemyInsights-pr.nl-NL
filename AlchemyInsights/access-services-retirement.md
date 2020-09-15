---
title: Toegang tot services buiten gebruik gesteld
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698677"
---
# <a name="access-services-retirement"></a>Toegang tot services buiten gebruik gesteld

Aangezien we voor het eerst aangekondigd zijn in MC97576, in maart 2017, en de laatste keer dat de toegangs services van het afgelopen jaar wordt buiten gebruik gesteld. De volgende fase van dit proces is de verwijdering van Access-webdatabases die SharePoint-lijsten gebruiken als onderliggende gegevensopslag.

**Wat betekent dit voor mij?**

Vanaf 2019 wordt het maken van nieuwe Access-databases in SharePoint Online beëindigd en wordt de service en alle resterende apps van april 2020 uitgeschakeld.

**Wat moet ik doen als voorbereiding op deze wijziging?**

U wordt aangeraden een overgangs plan te maken voor de Access-webdatabases van uw organisatie. Beheerders kunnen de [app scanner van SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gebruiken om een inventaris van de Access-apps te verkrijgen die sites gebruiken.

Er zijn verschillende manieren om gegevens van Access-webdatabases te migreren:

- Importeren in een lokale Access-database (. ACCDB) of een Excel-bestand.
- We raden u ook aan om Microsoft PowerApps als een alternatief platform te ontwikkelen voor het maken van zakelijke oplossingen zonder code voor Internet en mobiele apparaten.