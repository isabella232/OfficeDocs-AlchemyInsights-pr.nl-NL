---
title: Externe groepen uitschakelen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704123"
---
# <a name="how-to-disable-external-groups"></a>Externe groepen uitschakelen

Yammer externe berichtuitwisseling toepast Exchange-Transport regels (Etr's), een set proactieve besturingselementen om te voorkomen dat bedrijfsgegevens worden gedeeld. Om te voorkomen dat gebruikers externe groepen kunnen maken, moet u een Exchange-transportregel (ETR toe) configureren en Yammer configureren voor gebruik van de Exchange-transportregel om externe berichten te blokkeren.
  
Wanneer u een regel hebt gemaakt in het Exchange Online-Beheercentrum, voert u deze stappen uit om ETR toe in te stellen voor toepassing in Yammer:
  
- Meld u aan bij Yammer als een gecontroleerde beheerder, en in het **Yammer-Beheercentrum**gaat u naar C ** \> Beveiligingsinstellingen voor inhoud en beveiliging.**

- Selecteer onder **externe bericht**uitwisseling **de optie uw Exchange Online Exchange-Transport regels (Etr's) afdwingen in Yammer.**

- Selecteer **Save**.

Zie voor meer informatie [externe berichten uitschakelen in een Yammer-netwerk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  