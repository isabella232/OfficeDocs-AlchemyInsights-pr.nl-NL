---
title: Facturering voor aankoop van gereserveerd exemplaar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820317"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturering voor aankoop van gereserveerd exemplaar

De aankoop van het gereserveerde exemplaar wordt in rekening gebracht op de betalingswijze die is gekoppeld aan het abonnement dat u op het moment van aankoop selecteert. Het abonnementstype moet een ondernemingsovereenkomst zijn (aanbiedingsnummer: MS-AZR-0017P), Pay-As-You-Go (aanbiedingsnummer: MS-AZR-0003P), Microsoft Customer Agreement of CSP.

- Voor een ondernemingsabonnement worden de kosten afgetrokken van het saldo van de inschrijving of als overwaarde in rekening gebracht
- Voor betalen per gebruik-abonnement worden de kosten gefactureerd op de betalingswijze van de creditcard of factuur van het abonnement

**Reservering annuleren**

- **Selfservice:** U kunt een gereserveerd exemplaar zelf annuleren of uitwisselen met [Behulp van Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecteer de reservering en klik op restitutie of omruiling. Houd er rekening mee dat u toegang moet hebben tot de eigenaar van de reserveringsorder om deze om te wisselen of terug te betalen. Als u alleen toegang hebt tot de reservering, kunt u niet doorgaan met restitutie of omruiling. Vraag de eigenaar van de reserveringsorder om u de eigenaar toegang te geven tot de reserveringsorder
- **Exchange-beleid:** U kunt een reservering inruilen voor een andere reservering van hetzelfde type: er zijn **geen boetes voor reserveringsuitwisseling.** De totale verbintenis met nieuwe reservering moet groter zijn dan de som van het terugbetalingsbedrag van de geruilde reservering en de toekomstige maandelijkse betalingen (indien van toepassing)
- **Restitutiebeleid:** De som van de terugbetaling en de geannuleerde toekomstige betalingen mogen niet hoger zijn dan $ 50.000 USD in een rollend venster van 12 maanden. We brengen **momenteel geen boete in rekening voor** restituties, maar kunnen deze in rekening brengen bij toekomstige restituties

**Uitzonderingen:** Selfservice-mogelijkheid voor exchange en annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid voor enterprise agreement

- **API / PS / CLI-ondersteuning** is niet beschikbaar voor annulering en terugbetalingen [selfservice-exchanges en restituties voor Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selfservice-exchange- en annuleermogelijkheden zijn niet beschikbaar voor klanten van de Enterprise Agreement van de Amerikaanse overheid. Andere abonnementstypen van de Amerikaanse overheid, waaronder Pay-As-You-Go en CSP, worden ondersteund

Meer informatie: Hoe retour- en [exchange-transacties](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) worden verwerkt Meer informatie: Exchange- en [Restitutiebeleid](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Andere vragen: Ga naar [gereserveerde exemplaar docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Een bestaand gereserveerd exemplaar uitwisselen (Selfservice)**

U kunt een reservering inruilen voor een andere reservering van hetzelfde type. U kunt ook een reservering, tot $ 50.000 per jaar, terugbetalen als u deze niet meer nodig hebt. Selfservice-exchange- en annuleermogelijkheden zijn niet beschikbaar voor klanten van de Enterprise Agreement van de Amerikaanse overheid. Andere amerikaanse overheidsabonnementstypen, waaronder Pay-As-You-Go en CSP, worden ondersteund. U moet toegang hebben tot de eigenaar van de reserveringsorder om een bestaande reservering te kunnen omruilen of terug te betalen.

In de volgende stappen wordt de procedure voor het voltooien van de transactie

1.Meld u aan bij uw [Azure-portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecteer de reserveringen die u wilt terugbetalen en klik op **Exchange** 2.Selecteer het VM-product dat u wilt kopen en typ een hoeveelheid. Zorg ervoor dat het nieuwe aankooptotaal groter is dan het retourtotaal [Bepaal de juiste grootte voordat u de aankoop doet.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.De transactie controleren en voltooien

**Restitutie voor een gereserveerd exemplaar**

Als u een reservering wilt terugbetalen, gaat u naar **Reserveringsgegevens** en klikt u op **Restitutie**

**Pro-rated refund:**

**Voorbeelden van pro-ration en minimumvereiste voor restitutie en omruiling** Voorbeeld van reservering vooraf:

- U koopt op 1 januari een ri met een looptijd van één jaar voor $ 120
- Op 7 april wilt u deze reservering terugbetalen of omruilen
- Aangezien de reservering al 97 dagen live is, krijgt u (1-97/365) * $ 120 terug. (dat wil zeggen $ 88,1). Er is momenteel geen boete voor restituties
- Als u wisselt, moet uw nieuwe aankoop groter zijn dan $ 88,1
- Er is momenteel geen boete voor restituties

**Voorbeeld van reservering van factureringsplan:**

- U koopt een ri met een looptijd van één jaar voor $ 10 per maand
- Op 7 april wilt u deze reservering terugbetalen of omruilen
- Aangezien de laatste betaling 7 dagen heeft plaatsgevonden, krijgt u (1-7-31) * $ 10 terug. (dat wil zeggen $ 7,74)
- De toekomstige geannuleerde betalingen zijn $ 80. Er is momenteel geen boete voor restituties
- Met deze annulering wordt $ 87,74 aftrekken van de limiet van $ 50.000
- Als u wisselt, moet de totale waarde van nieuwe aankoop groter zijn dan $ 87,74

**Factuur voor de laatste factureringsperiode kan niet worden gezien**

Enkele mogelijke redenen waarom u mogelijk geen factuur ziet:

- U hebt een maandelijks tegoedbedrag met uw abonnement dat u niet hebt overschreden of u hebt een gratis proefabonnement. Een factuur wordt alleen gegenereerd wanneer u geld verschuldigd bent
- Het is minder dan 30 dagen vanaf de dag dat u zich hebt geabonneerd op Azure
- De factuur wordt nog niet gegenereerd. Wachten tot het einde van de factureringsperiode
- Als u niet de accountbeheerder bent, zijn oudere facturen mogelijk niet beschikbaar voor u

**Uw factuur downloaden van Azure Portal (.pdf)**

- Selecteer uw abonnement op [de pagina Abonnementen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in azure portal als gebruiker met toegang tot [facturen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Facturen **selecteren**
- Klik **op Factuur downloaden** om een kopie van uw PDF-factuur te bekijken. Zie Waarom zie **ik** geen factuur voor de laatste factureringsperiode als deze niet [beschikbaar is?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Uw factuur per e-mail ontvangen (.pdf)**

- Selecteer uw abonnement op [de pagina](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Abonnementen. Klik **op Facturen** en e-mail mijn factuur
- Klik **op Opt in** en accepteer de voorwaarden. U moet zich inschrijven voor elk abonnement dat u bezit

Opmerking: Als u na het volgen van de stappen geen e-mailbericht ontvangt, moet u ervoor zorgen dat uw e-mailadres juist is in de communicatievoorkeuren [in uw profiel](https://account.windowsazure.com/profile)

**Uw gebruiksgegevens downloaden van de Azure-portal**

- Meld u aan bij [het Azure Account Center](https://account.windowsazure.com/Subscriptions) als [accountbeheerder](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecteer het abonnement waarvoor u de factuur- en gebruiksgegevens wilt gebruiken
- **Factureringsgeschiedenis selecteren**
- Selecteer **Huidige instructie weergeven** om een schatting van uw kosten te bekijken op het moment dat de schatting is gegenereerd
- Selecteer **Gebruik downloaden** om de dagelijkse gebruiksgegevens te downloaden als een CSV-bestand. Als er twee versies beschikbaar zijn, downloadt u versie 2

Andere vragen: [Ga naar gereserveerde exemplaar docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Aanbevolen documenten**

- [Factureringsprincipes](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meer inzicht in de manier waarop de korting op gereserveerde exemplaren wordt toegepast](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Uw Factuur voor Azure-facturering en gegevens voor dagelijks gebruik downloaden of weergeven](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meer inzicht in de manier waarop de korting op gereserveerde exemplaren wordt toegepast](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Het gebruik van gereserveerde exemplaren voor uw abonnement op betalen per gebruik begrijpen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Het gebruik van gereserveerde exemplaren voor uw ondernemingsinschrijving begrijpen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-softwarekosten niet inbegrepen bij Gereserveerde exemplaren](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gereserveerde exemplaren in het CSP-programma (Partner Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)