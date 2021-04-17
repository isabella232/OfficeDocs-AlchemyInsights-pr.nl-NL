---
title: Reservering annuleren
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819687"
---
# <a name="cancelling-reservation"></a>Reservering annuleren

- **Selfservice:** U kunt een gereserveerd exemplaar zelf annuleren of uitwisselen in de [Microsoft Azure-portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecteer de reservering en klik op terugbetaling of omruiling. Houd er rekening mee dat u eigenaarstoegang op de reserveringsorder moet hebben om deze te kunnen ruilen of terugbetalen. Als u alleen toegang hebt tot de reservering, kunt u geen restitutie of omruiling verlenen. Vraag de eigenaar van de Reserveringsorder u toegang te geven tot de Reserveringsorder
- **Omruilbeleid:** u kunt een reservering omruilen voor een andere reservering van hetzelfde type, er zijn **geen boetes** voor het omwisselen van reserveringen. De totale verplichting met een nieuwe reservering moet groter zijn dan de som van het restitutiebedrag van de uitgewisselde reservering en de toekomstige maandelijkse betalingen (indien van toepassing)
- **Restitutiebeleid:** de som van de restitutie en de geannuleerde toekomstige betalingen mag niet hoger zijn dan $ 50.000 in een doorlopend venster van 12 maanden. We **brengen momenteel geen boete in rekening** voor restituties, maar kunnen deze wel in rekening brengen voor toekomstige restituties  
    **Uitzonderingen:** Selfservice-omruil- en annuleringsmogelijkheid is niet beschikbaar voor klanten van Enterprise Agreement van de Amerikaanse overheid
- **API/PS/CLI**-ondersteuning is niet beschikbaar voor annulering en restituties [Selfservice-uitwisselingen en restituties voor Azure-reserveringen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selfservice-omruil- en annuleringsmogelijkheid is niet beschikbaar voor klanten van Enterprise Agreement van de Amerikaanse overheid. Andere soorten abonnementen van de Amerikaanse overheid, waaronder Pay-As-You-Go en Microsoft Cloud Solution Provider, worden ondersteund

Meer informatie: [hoe retour- en omruilingstransacties worden verwerkt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Meer informatie: [omruilings- en restitutiebeleid](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Overige vragen: [Gereserveerde documenten bezoeken](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Een bestaand gereserveerd exemplaar omruilen (selfservice)**

U kunt een reservering uitwisselen voor een andere reservering van hetzelfde type. U kunt ook een reservering terugbetalen, tot $ 50.000 USD per jaar, als u deze niet langer nodig heeft. Selfservice-omruil- en annuleringsmogelijkheid is niet beschikbaar voor klanten van Enterprise Agreement van de Amerikaanse overheid. Andere soorten abonnementen van de Amerikaanse overheid, waaronder Pay-As-You-Go en Microsoft Cloud Solution Provider,, worden ondersteund. U moet eigenaarstoegang hebben op de reserveringsopdracht om een bestaande reservering te ruilen of terug te betalen.

De volgende stappen volgen de procedure voor het voltooien van de transactie

1. Meld u aan bij uw [Microsoft Azure-portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecteer de reserveringen die u wilt terugbetalen en klik op **Ruilen**
2. Selecteer het VM-product dat u wilt kopen en typ een hoeveelheid. Zorg ervoor dat het nieuwe aankoopbedrag meer is dan het retourbedrag. [Bepaal de juiste grootte voordat u tot aankoop overgaat](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. De transactie controleren en voltooien

**Restitutie voor een gereserveerd exemplaar**

Om een reservering terug te betalen, gaat u naar **Reserveringsgegevens** en klikt u op **Restitutie**

**Terugbetaling naar rato:**

**Voorbeelden van pro rata en minimumvereisten voor terugbetaling en omruiling**  
Voorbeeld van een reservering vooraf:

- U koopt op 1 januari een RI met een looptijd van één jaar voor $ 120
- Op 7 april wilt u een restitutie geven of deze reservering uitwisselen
- Aangezien de reservering 97 dagen actief is, krijgt u (1-97/365) * $ 120 terug. (dat wil zeggen, $ 88,1). Er geldt momenteel geen boete voor restituties
- Als u ruilt, moet uw nieuwe aankoop groter zijn dan $ 88,1
- Er geldt momenteel geen boete voor restituties

**Voorbeeld van reservering van factureringsplan:**

- U koopt een RI met een looptijd van één jaar voor $ 10 per maand
- Op 7 april wilt u een restitutie geven of deze reservering uitwisselen
- Omdat de laatste betaling 7 dagen geleden plaatsvond, krijgt u (1-7/31) * $ 10 terug. (dat wil zeggen, $ 7,74).
- De toekomstige betalingen die worden geannuleerd zijn $ 80. Er geldt momenteel geen boete voor restituties
- Deze annulering betekent dat er $ 87,74 wordt afgetrokken van de teruggavelimiet van $ 50.000
- Als u ruilt, moet uw nieuwe aankoop groter zijn dan $ 87,74

**Aanbevolen documenten**

- [Hoe retour- en omruilingstransacties worden verwerkt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Omruilings- en restitutiebeleid](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)