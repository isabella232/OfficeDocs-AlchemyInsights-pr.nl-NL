---
title: Veranderen van Microsoft-naamservers terug naar het beheren van uw eigen DNS-records
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506383"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Veranderen van Microsoft-naamservers terug naar het beheren van uw eigen DNS-records

U hebt eerder uw NS-records gewijzigd om te wijzen naar Microsoft (ns1.bdm.microsoftonline.com), maar u hebt nu besloten om uw eigen DNS-records te beheren:

Wijzig op de website van uw domeinregistrar de naamserver terug naar uw registrar of vorige instelling. Als u niet bekend bent met DNS, neemt u contact op met de ondersteuning van de domeinregistrar. Houd er rekening mee dat het tot 48 uur kan duren voordat naamserverwijzigingen worden doorgevoerd. 

1. Ga in Microsoft 365-beheerportal **naar Instellingen** Domeinen, schakel het selectievakje naast het domein in en  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)selecteer **DNS beheren.** 

2. Selecteer in de wizard **Uw eigen DNS-records toevoegen** en voltooi de wizard. Hierdoor verandert de manier waarop uw DNS wordt beheerd en kunt u vervolgens de aangepaste DNS-records toevoegen die nodig zijn om uw geselecteerde services te ondersteunen.

Als u uw naamserverrecords hebt gewijzigd in Microsoft en een website hebt, kunt u ook DNS-records voor de website toevoegen in plaats van de naamservers terug te wijzigen. Zie DNS-records bijwerken om uw website bij uw huidige [hostingprovider te houden](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)voor meer informatie.


