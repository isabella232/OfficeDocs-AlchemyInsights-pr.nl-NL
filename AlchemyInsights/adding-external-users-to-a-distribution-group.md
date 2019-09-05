---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737868"
---
# <a name="add-external-users-to-a-distribution-group"></a>Externe gebruikers toevoegen aan een distributiegroep

Het toevoegen van een externe contactpersoon aan een distributiegroep (DG) is een proces in twee stappen:
  
1. Een e-mail contactpersoon voor de externe gebruiker maken:
    
    1. Ga in het Admin Center naar de pagina **** > [contactpersonen](https://admin.microsoft.com/adminportal/home#/Contact) van gebruikers. 
    
    2. Selecteer **een contactpersoon toevoegen**.
    
    3. Typ de informatie voor uw contactpersoon en selecteer **toevoegen**.
    
2. Voeg het e-mail contact toe aan uw DG:
    
    1. Ga in het Beheercentrum naar de pagina **groeps** > [groepen.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Zoek het DG waaraan u de externe gebruiker wilt toevoegen en selecteer het om het dialoogvenster bewerken te openen.
    
    3. Selecteer op het tabblad **leden** de optie **alle weergeven en leden beheren**. 
    
    4. Selecteer **leden toevoegen**.
    
    5. Selecteer de e-mail contactpersoon die u hebt gemaakt in de vorige stap en selecteer vervolgens **Opslaan**.
    
Als u na het volgen van deze stappen uw externe gebruikers geen e-mails kunnen sturen naar het DG of geen e-mails van deze ontvangen, kan het zijn dat het DG is gemarkeerd om alleen e-mails van interne gebruikers toe te staan. U deze configuratie controleren en dit oplossen door de aanwijzingen [hier](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)te volgen.
  
 **Opmerking:** Deze instructies zijn niet van toepassing als het type van uw groep ' Office 365 groep ' in plaats van ' distributiegroep ' is. Als dat het geval is, u de externe gebruiker rechtstreeks vanuit Outlook aan de groep toevoegen. Gedetailleerde informatie over Office 365 groepen gasten en instructies voor het toevoegen van externe gasten zijn te vinden in [dit artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  