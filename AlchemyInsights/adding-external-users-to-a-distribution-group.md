---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934828"
---
# <a name="add-external-users-to-a-distribution-group"></a>Externe gebruikers toevoegen aan een distributiegroep

Het toevoegen van een externe contactpersoon aan een distributiegroep (DG) is een proces in twee stappen:
  
1. Een e-mailcontactcontact voor de externe gebruiker maken:
    
    1. Ga in het beheercentrum naar de pagina  >  [Gebruikerscontactcontacten.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Selecteer **Een contactpersoon toevoegen.**
    
    3. Typ de gegevens voor uw contactpersoon en selecteer **Toevoegen.**
    
2. Voeg de e-mailcontactcontacte toe aan uw DG:
    
    1. Ga in het beheercentrum naar de pagina  >  [Groepen groepen.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Zoek de DG aan wie u de externe gebruiker wilt toevoegen en selecteer deze om het dialoogvenster Bewerken te openen.
    
    3. Selecteer op **het** tabblad Leden de optie **Alle leden weergeven en beheren.** 
    
    4. Selecteer **Leden toevoegen.**
    
    5. Selecteer de e-mailcontactcontact die u in de vorige stap hebt gemaakt en selecteer **opslaan.**
    
Als uw externe gebruikers na het volgen van deze stappen geen e-mailberichten naar het DG kunnen verzenden of er geen e-mailberichten van kunnen ontvangen, kan het zijn dat het DG is gemarkeerd om alleen e-mailberichten van interne gebruikers toe te staan. U kunt deze configuratie controleren en deze oplossen volgens de aanwijzingen [hier.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Opmerking:** Deze instructies zijn niet van toepassing als het type van uw groep 'Microsoft 365 groep' is in plaats van 'Distributiegroep'. Als dat het geval is, kunt u de externe gebruiker rechtstreeks toevoegen aan de groep Outlook. Gedetailleerde informatie over Microsoft 365 Groepen gasten en instructies voor het toevoegen van externe gasten vindt u in [dit artikel.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  