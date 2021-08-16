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
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015615"
---
# <a name="how-to-disable-external-groups"></a>Externe groepen uitschakelen

Yammer externe berichtuitwisseling is Exchange transportregels (ETR's), een reeks proactieve besturingselementen om te voorkomen dat bedrijfsgegevens worden gedeeld. Als u wilt voorkomen dat gebruikers externe groepen maken, moet u een Exchange-transportregel (ETR) configureren en vervolgens Yammer configureren om de regel Exchange Transport te gebruiken om externe berichten te blokkeren.
  
Nadat u een regel hebt gemaakt in Exchange Online beheercentrum, volgt u de volgende stappen om ETR in te stellen voor toepassing in Yammer:
  
- Meld u aan Yammer als geverifieerde beheerder en ga in het **Yammer-beheercentrum** naar **C-inhoud en \> beveiligingsbeveiliging Instellingen.**

- Selecteer **onder Externe berichtuitwisseling** de optie **Uw Exchange Online Exchange transportregels (ETR's) afdwingen in Yammer.**

- Selecteer **Opslaan**.

Zie Externe berichten in een netwerk uitschakelen voor [Yammer meer informatie.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  