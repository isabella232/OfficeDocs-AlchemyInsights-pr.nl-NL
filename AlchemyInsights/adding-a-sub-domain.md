---
title: Een subdomein toevoegen
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506326"
---
# <a name="adding-a-sub-domain"></a>Een subdomein toevoegen

Subdomeinen kunnen worden toegevoegd aan dezelfde of een andere tenant dan het bovenliggende domein. In beide gevallen moet u uw eigen DNS-instellingen beheren op de website van uw registrar. Als u microsoft uw DNS-instellingen hebt laten beheren met NS-records of als u het domein bij Microsoft hebt gekocht, kunt u geen subdomeinen toevoegen zonder dit eerst te wijzigen.

Voeg eerst het bovenliggende domein toe en voeg vervolgens het subdomein toe. Als het subdomein zich in dezelfde tenant heeft, is er geen extra verificatie nodig. Als u het subdomein toevoegt aan een afzonderlijke tenant, is de DNS txt-record vereist voor eigendomsverificatie voordat u het domein en de extra DNS-records voor de geselecteerde services toevoegt.

- Als u een domein of subdomein wilt toevoegen, volgt u de [wizard](https://admin.microsoft.com/Adminportal#/Domains/Wizard)Domein toevoegen of voegt u het domein of subdomein handmatig toe door naar **Domein** toevoegen domein  >    >  **instellen te gaan.**

Indien nodig:

- Als u wilt wijzigen wie uw DNS-instellingen voor een bestaand domein beheert, gaat u naar **Instellingen**  >  [**Domains,**](https://admin.microsoft.com/Adminportal/Home#/Domains)schakel het selectievakje naast het domein in en selecteert u **VERVOLGENS DNS beheren.** Selecteer in de wizard **Uw eigen DNS-records toevoegen** en voltooi de wizard.
- Als u subdomeinen wilt toevoegen aan een door Microsoft gekocht domein, moet u eerst het domein overbrengen naar een andere registrar en vervolgens de bovenstaande wijziging aan brengen om uw eigen DNS-records te beheren. Zie Een domein van Microsoft overbrengen naar een andere host voor [instructies.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Als u een foutmelding ontvangt dat uw domein al wordt gebruikt door andere leden of personen in uw organisatie, moet u dit niet-beherende account eerst overnemen voordat u het domein gebruikt. Zie Een [niet-beheerbare](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)adreslijst overnemen als beheerder in Azure Active Directory.
