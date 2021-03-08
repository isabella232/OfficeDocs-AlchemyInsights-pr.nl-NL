---
title: Office 365-e-mailberichten die naar bepaalde domeinen worden verzonden, automatisch versleutelen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524877"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Office 365-e-mailberichten die naar bepaalde domeinen worden verzonden, automatisch versleutelen

1. Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **e-mailstroom > regels.** 
2. Klik op **het pictogram Nieuw (+)** en klik vervolgens op Office 365-berichtversleuteling toepassen en bescherming tegen rechten **op berichten.**
3. Voer **in** Naam een naam in voor de regel, zoals Berichten versleutelen die *naar* de contoso.com.
4. Kies **bij Deze regel toepassen als** de ontvanger > domein **is.** 
5. Voer de naam van het domein in, zoals **contoso.com.**
6. Klik op **het pictogram Toevoegen (+)** en klik op **OK.**
7. Klik naast het **veld Ga als volgt** te werk op Selecteer een **optie.** 
8. Selecteer **versleutelen** in de vervolgkeuzelijst van de RMS-sjabloon **en** klik op **OK.** (Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat. Maar u kunt het toevoegen!)
9. Kies desgewenst een selectie (in een lijst met optionele selecties die u op dit punt kunt maken, waarvan er een groot aantal kan worden overgelaten met de standaardinstelling voor eenvoud).
10. Klik op **Opslaan**.

> [!IMPORTANT]
> U kunt altijd teruggaan en deze regel later bewerken.

Zie Regels voor de e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) voor meer informatie over het maken van regels voor versleuteling.