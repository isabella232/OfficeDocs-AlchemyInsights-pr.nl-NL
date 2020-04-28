---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910927"
---
# <a name="add-external-users-to-a-distribution-group"></a>Externe gebruikers toevoegen aan een distributiegroep

Het toevoegen van een extern contact aan een distributiegroep (DG) is een proces in twee stappen:
  
1. Een e-mailcontactpersoon maken voor de externe gebruiker:
    
    1. Ga in het beheercentrum naar de pagina > [Gebruikerscontactpersonen.](https://admin.microsoft.com/adminportal/home#/Contact) **Users** 
    
    2. Selecteer **Een contactpersoon toevoegen**.
    
    3. Typ de gegevens voor uw contactpersoon en selecteer **Toevoegen**.
    
2. Voeg de mailcontact toe aan uw DG:
    
    1. Ga in het beheercentrum naar de pagina **Groepen** > [groepen.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Zoek de DG waaraan u de externe gebruiker wilt toevoegen en selecteer deze om het dialoogvenster bewerken te openen.
    
    3. Selecteer op het tabblad **Leden** **alle leden weergeven en leden beheren**. 
    
    4. Selecteer **Leden toevoegen**.
    
    5. Selecteer de e-mailcontactpersoon die u in de vorige stap hebt gemaakt en selecteer **Opslaan**.
    
Als uw externe gebruikers na het volgen van deze stappen geen e-mails naar de DG kunnen verzenden of er geen e-mails van kunnen ontvangen, kan het zijn dat de DG is gemarkeerd om alleen e-mails van interne gebruikers toe te staan. U deze configuratie controleren en deze herstellen volgens de aanwijzingen [hier.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Let op:** Deze instructies zijn niet van toepassing als het type van uw groep 'Microsoft 365-groep' is in plaats van 'Distributiegroep'. Als dat het geval is, u de externe gebruiker rechtstreeks vanuit Outlook aan de groep toevoegen. Gedetailleerde informatie over gasten van Microsoft 365 Groups en instructies voor het toevoegen van externe gasten vindt u in [dit artikel.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  