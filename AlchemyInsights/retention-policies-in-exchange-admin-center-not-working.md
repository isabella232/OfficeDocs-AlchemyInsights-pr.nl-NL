---
title: Bewaarbeleid in Exchange-beheercentrum werkt niet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952223"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Bewaarbeleid in exchange-beheercentrum

Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de knop Terug < boven aan deze pagina en voert u vervolgens het e-mailadres in van de gebruiker die problemen heeft met bewaarbeleid.

Als u problemen hebt met bewaarbeleid in het Exchange-beheercentrum dat niet van toepassing is op postvakken of items die niet naar het archiefpostvak worden verplaatst, controleert u het volgende:

**Hoofdoorzaken:**

- **Beheerde mapassistent** heeft het postvak van de gebruiker niet verwerkt. Met de assistent voor beheerde mappen wordt geprobeerd om elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken.

  **Oplossing:** Voer de assistent beheerde map uit.

- **RetentionHold** is **ingeschakeld** in het postvak. Als het postvak is geplaatst op een Bewaarbewaring, wordt het bewaarbeleid voor het postvak in die periode niet verwerkt.

  **Oplossing:** Controleer de status van bewaringsinstelling en werk zo nodig bij. Zie Bewaring van [postvak voor meer informatie.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Opmerking:** Als een postvak kleiner is dan 10 MB, wordt het postvak niet automatisch verwerkt door de Assistent voor beheerde mappen.
 
Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:

- [Bewaarlabels en bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Een bewaarbeleid toepassen op postvakken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) of [bewaarlabels toevoegen of verwijderen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Het type bewaring voor een postvak identificeren](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
