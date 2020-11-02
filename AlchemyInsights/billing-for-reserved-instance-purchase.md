---
title: Facturering voor een gereserveerd exemplaar van aankoop
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823031"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturering voor een gereserveerd exemplaar van aankoop

Voor de aankoop van een gereserveerd exemplaar wordt rekening gebracht met de betaalwijze die is gekoppeld aan het abonnement dat u op het moment van aankoop selecteert. Het type abonnement moet een Enterprise Agreement zijn (nummer van aanbieding: MS-AZR-0017P), pay-as-u-go (aanbiedings nummer: MS-AZR-0003P), Microsoft Customer Agreement of CSP.

- Voor een Enterprise-abonnement worden de kosten in rekening gebracht voor het monetaire toezeggings saldo van de inschrijving of in rekening gebracht als overage
- Voor Pay-to-go-abonnementen worden de kosten gefactureerd aan de betaling per creditcard of factuur methode voor het abonnement

**Reservering annuleren**

- **Self-service:** U kunt met behulp van [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)zelf een gereserveerd exemplaar annuleren of uitwisselen. Selecteer de reservering en klik op restitutie of Exchange. U moet beschikken over de eigenaren van de reserverings order voor Exchange of restitutie. U kunt met alleen de reservering verdergaan met restitutie of Exchange. Vraag de eigenaar van de reserverings order om u de reserverings order toegang te geven
- **Exchange-beleid:** U kunt een reservering uitwisselen voor een andere reservering van hetzelfde type – er zijn **geen sancties** voor de reserverings uitwisseling. De totale toezegging met de nieuwe reservering moet groter zijn dan de som van het restitutiebedrag van de geexchangeeerde reservering en de toekomstige maandelijkse aflossing (indien van toepassing).
- **Restitutiebeleid:** De som van de restitutie en de geannuleerde toekomstige betaling mag niet groter zijn dan $50.000 USD in een rolling venster van 12 maanden. Er worden op **dit moment geen boete** aan betaald, maar het bedrag voor toekomstige restituties werd opgeheven.

**Uitzonderingen:** Service voor selfservice uitwisseling en annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement

- **API/PS/cli-** ondersteuning is niet beschikbaar voor annulering en teruggave [van selfservice-uitwisseling en restitutie voor Azure reserveringen](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selfservice Exchange en de mogelijkheid om te annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement. Andere typen US Government-abonnementen, waaronder pay-as-nl-go en CSP, worden ondersteund

Meer informatie: meer informatie [over de manier waarop retour-en Exchange-transacties worden verwerkt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) [meer: meer](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) vragen over het Exchange- [en restitutiebeleid](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)

**Een bestaand gereserveerd exemplaar (Self-Service) uitwisselen**

U kunt een reservering uitwisselen voor een andere reservering van hetzelfde type. Als u het niet meer nodig hebt, betaalt u ook een reservering van maximaal $50.000 USD per jaar. Selfservice Exchange en de mogelijkheid om te annuleren is niet beschikbaar voor klanten van de Amerikaanse overheid Enterprise Agreement. Andere typen US Government-abonnementen, waaronder pay-as-u-go en CSP, worden ondersteund. U moet beschikken over de eigenaren van de reserverings order voor het omwisselen van een bestaande reserve.

De volgende stappen helpen u bij de procedure voor het voltooien van de transactie

1. Meld u aan bij uw [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecteer de reserveringen die u wilt terugbetalen en klik op **Exchange** 2. Selecteer het VM-product dat u wilt kopen en typ een hoeveelheid. Zorg ervoor dat het nieuwe totale aankoopbedrag hoger is dan het retour totaal, [Bepaal de juiste grootte voordat u koopt](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. de transactie controleren en voltooien

**Restitutie voor een gereserveerd exemplaar**

Als u een reservering wilt terugbetalen, gaat u naar **reserverings details** en klikt u op **restitutie**

**Met Pro geclassificeerde restitutie:**

Voor **beelden van Pro-en minimumvereisten voor restitutie en uitwisseling** Voorbeeld van precover reservation:

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

**De factuur voor de laatste factureringsperiode kan niet worden weergegeven**

Mogelijke redenen zijn dat u een factuur niet ziet:

- U hebt een maandbedrag met uw abonnement dat u niet meer weet of als u een gratis proefabonnement hebt. Een factuur wordt alleen gegenereerd wanneer u geld verschuldigt
- 30 dagen na de dag waarop u zich hebt geabonneerd op Azure
- De factuur is nog niet gegenereerd. Wachten tot het einde van de factureringsperiode
- Als u niet de account beheerder bent, zijn oudere facturen mogelijk niet voor u beschikbaar

**Uw factuur downloaden van Azure Portal (. PDF)**

- Selecteer uw abonnement op de pagina [abonnementen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in azure-portal als [een gebruiker met toegang tot facturen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Facturen** selecteren
- Klik op **factuur downloaden** om een kopie van de PDF-factuur weer te geven. Zie [Waarom zie ik geen factuur voor de laatste factuurperiode?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) als dit **niet beschikbaar** is.

**Uw factuur ontvangen via e-mail (. PDF)**

- Selecteer uw abonnement op de pagina [abonnementen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Klik op **factuur** en vervolgens op e-mail verzenden
- Klik op **Afmelden** en accepteer de voorwaarden. U moet zich aanmelden voor elk abonnement dat u bezit

Opmerking: als u na het uitvoeren van de stappen geen e-mail ontvangt, controleert u of uw e-mailadres juist is in de [communicatievoorkeuren van uw profiel](https://account.windowsazure.com/profile)

**Uw gebruiksgegevens downloaden van de Azure-Portal**

- Meld u aan bij het [Azure-account centrum](https://account.windowsazure.com/Subscriptions) als [account beheerder](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecteer het abonnement waarvoor u de factuur en gebruiksinformatie wilt
- **Factureringsgeschiedenis** selecteren
- Selecteer **huidige instructie weergeven** om een raming van uw kosten te zien op het moment dat de raming werd gegenereerd.
- Selecteer **gebruik downloaden** om de dagelijkse gebruiksgegevens te downloaden als een CSV-bestand. Als u twee versies beschikbaar ziet, download versie 2.

Overige vragen: [naar documenten met gereserveerde exemplaren van documenten](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) gaan

**Aanbevolen documenten**

- [Basisprincipes van facturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Inzicht in de manier waarop de gereserveerde exemplaar korting wordt toegepast](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Uw Azure-facturerings factuur en dagelijkse gebruiksgegevens downloaden of weergeven](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Inzicht in de manier waarop de gereserveerde exemplaar korting wordt toegepast](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gebruik van het gereserveerde exemplaar voor uw abonnement voor betalen naar gebruik](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gebruik van het gereserveerde exemplaar van uw Enterprise-registratie](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-softwarekosten die niet zijn opgenomen in gereserveerde exemplaren](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gereserveerde exemplaren in partner Central Cloud Solution Provider (CSP)-programma](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)