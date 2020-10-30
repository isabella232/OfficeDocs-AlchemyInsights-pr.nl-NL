---
title: Reservering annuleren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807362"
---
# <a name="cancelling-reservation"></a>Reservering annuleren

- **Self-service:** U kunt met behulp van [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)zelf een gereserveerd exemplaar annuleren of uitwisselen. Selecteer de reservering en klik op restitutie of Exchange. U moet beschikken over de eigenaren van de reserverings order voor Exchange of restitutie. U kunt met alleen de reservering verdergaan met restitutie of Exchange. Vraag de eigenaar van de reserverings order om u de reserverings order toegang te geven
- **Exchange-beleid:** U kunt een reservering uitwisselen voor een andere reservering van hetzelfde type – er zijn **geen sancties** voor de reserverings uitwisseling. De totale toezegging met de nieuwe reservering moet groter zijn dan de som van het restitutiebedrag van de geexchangeeerde reservering en de toekomstige maandelijkse aflossing (indien van toepassing).
- **Restitutiebeleid:** De som van de restitutie en de geannuleerde toekomstige betaling mag niet groter zijn dan $50.000 USD in een rolling venster van 12 maanden. Er worden op **dit moment geen boete** aan betaald, maar het bedrag voor toekomstige restituties werd opgeheven.  
    **Uitzonderingen:** Service voor selfservice uitwisseling en annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement
- **API/PS/cli-** ondersteuning is niet beschikbaar voor annulering en teruggave [van selfservice-uitwisseling en restitutie voor Azure reserveringen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selfservice Exchange en de mogelijkheid om te annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement. Andere typen US Government-abonnementen, waaronder pay-as-nl-go en CSP, worden ondersteund

Meer informatie: [hoe retour-en Exchange-transacties worden verwerkt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Meer informatie: [beleid voor koers uitwisseling en restitutie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Overige vragen: [naar documenten met gereserveerde exemplaren van documenten](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) gaan

**Een bestaand gereserveerd exemplaar (Self-Service) uitwisselen**

U kunt een reservering uitwisselen voor een andere reservering van hetzelfde type. Als u het niet meer nodig hebt, betaalt u ook een reservering van maximaal $50.000 USD per jaar. Selfservice Exchange en de mogelijkheid om te annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement. Andere typen US Government-abonnementen, waaronder pay-as-u-go en CSP, worden ondersteund. U moet beschikken over de eigenaren van de reserverings order voor het omwisselen van een bestaande reserve.

De volgende stappen helpen u bij de procedure voor het voltooien van de transactie

1. Meld u aan bij uw [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecteer de reserveringen die u wilt terugbetalen en klik op **Exchange** .
2. Selecteer het VM-product dat u wilt kopen en typ een hoeveelheid. Zorg ervoor dat het nieuwe totale aankoopbedrag groter is dan het retour totaal, [de juiste grootte bepalen voordat u koopt](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. De transactie controleren en voltooien

**Restitutie voor een gereserveerd exemplaar**

Als u een reservering wilt terugbetalen, gaat u naar **reserverings details** en klikt u op **restitutie**

**Met Pro geclassificeerde restitutie:**

**Voorbeelden van Pro-en minimumvereisten voor restitutie en uitwisseling**  
Voorbeeld van precover reservation:

- U koopt een term RI voor 1 jaar voor $120 op 1 januari
- Op 7 april wilt u deze reservering vervragen of verwisselen
- Aangezien de reservering voor 97 dagen live is, krijgt u (1-97/365) * $120 back. (bijvoorbeeld $88,1). Er is momenteel geen boete voor de vergoeding
- Als de uitwisseling is opgebruikt, moet uw nieuwe aankoop groter zijn dan $88,1
- Er is op dit moment geen boete voor restituties

**Voorbeeld van reservering van facturerings abonnement:**

- U koopt een term RI van één jaar voor $10 per maand
- Op 7 april wilt u deze reservering vervragen of verwisselen
- Aangezien de laatste betaling 7 dagen plaatsvond, krijgt u (1-7/31) * $10 terug. (bijvoorbeeld $7,74)
- De termijn voor toekomstige betalingen zijn $80. Er is momenteel geen boete voor de vergoeding
- Met deze annulering wordt $87,74 afgetrokken van u de $50.000-restitutie limiet
- Als de totale waarde van de aankoop groter is dan $87,74, moet de totale waarde van de nieuwe aankoop groter zijn dan.

**Aanbevolen documenten**

- [Hoe retour-en Exchange-transacties worden verwerkt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Beleid voor Exchange en restitutie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)