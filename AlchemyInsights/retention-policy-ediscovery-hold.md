---
title: 2609-retentie-of-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994056"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Kan geen items verwijderen in SharePoint Online of OneDrive voor bedrijven

U of uw gebruikers mogelijk niet verwijderen van items in SharePoint Online of OneDrive voor bedrijven omdat een bewaarbeleid, bewaar label of eDiscovery-wachtruimte wordt toegepast op een SharePoint van OneDrive-site of een specifiek item. Dit omvat het niet kunnen verwijderen van een document, een documentversie, een map, een documentbibliotheek, een lijst, een app, een site of een siteverzameling. Hier volgen enkele voorbeelden van de foutberichten die u ontvangen als u probeert een item te verwijderen dat wordt bewaard:

- "Deze site kan niet worden verwijderd omdat deze is opgenomen in een eDiscovery-opslag of bewaarbeleid"
- "Deze site heeft een nalevingsbeleid ingesteld op het blokkeren van verwijdering"
- "Een nalevingsbeleid blokkeert momenteel deze site verwijdering"
- ' Deze siteverzameling kan niet worden verwijderd omdat deze sites bevat die deel uitmaken van een eDiscovery-beleid voor vasthouden of bewaren '
- "U moet alle items in deze map verwijderen voordat u de map verwijdert"
- ' Versies van dit item kunnen niet worden verwijderd omdat het in de Houd-of bewaarbeleid staat '
- "Item kan niet worden verwijderd tijdens de Hold"
- "Het label dat op dit item wordt toegepast, voorkomt dat het wordt bewerkt of verwijderd"
- "Lijst kan niet worden verwijderd tijdens het vasthouden of bewaarbeleid"
- "De lijst kan niet worden verwijderd als deze is geblokkeerd of als er een bewaarbeleid wordt toegepast"

Als u items in een van deze scenario's wilt verwijderen, moet het bewaarbeleid, het retentie label of de eDiscovery-opslagruimte worden verwijderd (of moet een site worden uitgesloten van een bewaarbeleid). U moet de respectieve Hold die dit probleem veroorzaakt uitschakelen of uitsluiten. Nadat een bewaarbeleid of wachtstand is verwijderd, kan het maximaal 24 uur duren voordat de wijziging van kracht wordt. 

Zie een van de volgende onderwerpen voor informatie over de verschillende retentie-en Hold-functies die kunnen worden toegepast op SharePoint-sites en OneDrive-accounts.

- [Overzicht van bewaarbeleid](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Overzicht van inhoudings etiketten](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Bewaarplichten beheren in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery houdt](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Beleid voor beëindiging en verwijdering van verouderde sites](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
