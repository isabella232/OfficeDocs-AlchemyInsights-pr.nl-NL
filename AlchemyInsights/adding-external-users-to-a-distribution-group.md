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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663508"
---
# <a name="add-external-users-to-a-distribution-group"></a>Externe gebruikers toevoegen aan een distributiegroep

Het toevoegen van een externe contactpersoon aan een distributiegroep (DG) bestaat uit twee stappen:
  
1. Een e-mail contactpersoon voor de externe gebruiker maken:
    
    1. Ga naar de **Users**  >  pagina[contactpersonen](https://admin.microsoft.com/adminportal/home#/Contact) van gebruikers in het Beheercentrum. 
    
    2. Selecteer **een contactpersoon toevoegen**.
    
    3. Typ de gegevens voor de contactpersoon en selecteer **toevoegen**.
    
2. De e-mail contactpersoon toevoegen aan de DG:
    
    1. Ga in het Beheercentrum naar de pagina **groepen**  >  [groepen](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Ga naar de DG waaraan u de externe gebruiker wilt toevoegen en selecteer deze om het dialoogvenster bewerken te openen.
    
    3. Selecteer op het tabblad **leden** de optie **AllesWeergeven en leden beheren**. 
    
    4. Selecteer **leden toevoegen**.
    
    5. Selecteer de e-mail contactpersoon die u in de vorige stap hebt gemaakt en selecteer vervolgens **Opslaan**.
    
Als uw externe gebruikers na deze stappen niet e-mailberichten kunnen verzenden naar de DG of geen e-mailberichten ontvangen, is het mogelijk dat de DG alleen is gemarkeerd voor het toestaan van e-mailberichten van interne gebruikers. U kunt deze configuratie controleren en deze oplossing volgen op de [onderstaande instructies.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Opmerking:** Deze instructies zijn niet van toepassing als het type van de groep ' Microsoft 365 Group ' in plaats van ' distributiegroep ' is. Als dat het geval is, kunt u de externe gebruiker rechtstreeks toevoegen aan de groep vanuit Outlook. In [dit artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)vindt u meer informatie over gasten van microsoft 365 en de instructies voor het toevoegen van externe gast groepen.
  