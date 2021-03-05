---
title: De inrichtingsservice configureren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481851"
---
# <a name="configuring-the-provision-service"></a>De inrichtingsservice configureren

Voor automatische inrichting door gebruikers moet Azure AD geldige referenties hebben waarmee verbinding kan worden maken met de Web Services-API van Werkdag. Verder wordt met de knop Verbinding testen op de app Werkdag naar AD-gebruikers inrichting ook gevalideerd of er verbinding kan worden gemaakt met de Azure AD Connect Provisioning-agent die is gekoppeld aan het AD-domein.

Als azure portal een fout retourneert bij het opslaan van de referenties, volgt u de onderstaande aanbevolen stappen:

1. Bevestig dat u het gebruikersaccount van het Workday Integration System hebt geconfigureerd, zoals vermeld in het gedeelte Voor zelfstudie de gebruiker van het integratiesysteem [configureren in Werkdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Controleer of de Azure AD Connect Provisioning Agent Service actief is op uw on-premises Windows-server met behulp van de servicebeheerconsole. U kunt ook de status van de agent in de Azure Portal controleren door te klikken op de knop On-premises agenten weergeven.
3. Zorg ervoor dat u de waarde voor het veld 'Gebruikersnaam werkdag' in de notatie username@workday-tenantnaam. Als de naam van de werkdag-tenant ontbreekt, mislukt de verificatie op werkdag.
4. Als u de integratie met de tenant voor de implementatie van Werkdag configureert, houd dan rekening met de geplande downtime van uw werkdag-tenant. Op de werkdag is de tijd voor de implementatie van tenants gepland in het weekend (meestal van vrijdagnacht tot zaterdagochtend) en storingen van de connectiviteit tijdens deze downtime zijn een bekend probleem dat automatisch wordt opgelost zodra de implementatieten weer online zijn.
5. In zeldzame gevallen kan deze fout ook worden weergegeven als het wachtwoord van de gebruiker van het integratiesysteem is gewijzigd vanwege het vernieuwen van de tenant of als het account is vergrendeld of verlopen. Controleer de status van de gebruiker van het integratiesysteem met uw werkdagbeheerder.

Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
