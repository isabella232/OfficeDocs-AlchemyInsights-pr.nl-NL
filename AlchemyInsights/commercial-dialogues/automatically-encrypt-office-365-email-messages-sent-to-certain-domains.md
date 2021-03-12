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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744550"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Office 365-e-mailberichten die naar bepaalde domeinen worden verzonden, automatisch versleutelen

1. Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **de optie e-mailstroom > regels.** 
2. Klik op **het pictogram Nieuw (+)** en klik vervolgens op **Office 365-berichtversleuteling en rechtenbescherming toepassen op berichten.**
3. Voer **in Naam** een naam in voor de regel, zoals Berichten versleutelen die naar *contoso.com.*
4. Kies **in Deze regel toepassen als**, de optie De ontvanger > domein **is**. 
5. Voer de naam van het domein in, zoals **contoso.com.**
6. Klik op **het pictogram Toevoegen (+)** en klik vervolgens op **OK.**
7. Klik naast **het veld Het volgende** doen op Selecteer **een**. 
8. Selecteer in **de vervolgkeuzelijst RMS-sjabloon** de optie **Versleutelen** en klik vervolgens op **OK.** (Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat. Maar u kunt het toevoegen!)
9. Kies een optionele selectie (in een lijst met optionele selecties die u op dit moment kunt maken, waarvan er veel kunnen worden overgelaten met de standaardinstelling voor eenvoud).
10. Klik op **Opslaan**.

> [!IMPORTANT]
> U kunt deze regel later altijd weer bewerken.

Zie Regels voor e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) voor meer informatie over het maken van regels voor versleuteling.