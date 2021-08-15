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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033273"
---
# <a name="configuring-the-provision-service"></a>De inrichtingsservice configureren

Voor het geautomatiseerde inrichten van gebruikers is voor Azure AD geldige referenties vereist waarmee deze verbinding kan maken met de Workday Web Services API. Bovendien wordt met de knop Verbinding testen op de app Workday to AD User Provisioning ook gevalideerd of deze verbinding kan maken met de Azure AD Verbinding maken Provisioning Agent die is gekoppeld aan het AD-domein.

Als de Azure-portal een fout retourneert bij het opslaan van de referenties, volgt u de onderstaande aanbevolen stappen:

1. Bevestig dat u het gebruikersaccount van het Workday Integration System hebt geconfigureerd, zoals wordt vermeld in de sectie Integratiesysteemgebruiker configureren [in Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Controleer of de Azure AD Verbinding maken Provisioning Agent Service actief is op uw on-premises Windows server met de Services Management Console. U kunt ook de status van de agent in de Azure-portal controleren door op de knop On-premises agenten weergeven te klikken.
3. Zorg ervoor dat u de waarde voor het veld 'Gebruikersnaam van werkdag' in de indeling username@workday-tenantnaam. Als de naam van de werkdag-tenant ontbreekt, mislukt De verificatie van Werkdag.
4. Als u de integratie met workday-implementatie tenant configureert, noteert u de geplande downtimeuren van uw Workday-tenant. Werkdag heeft de tijd voor de implementatieten tenants gepland in het weekend (meestal van vrijdag avond tot zaterdagochtend) en verbindingsfouten tijdens dit downtimevenster is een bekend probleem dat automatisch wordt opgelost zodra de implementatieten tenants weer online zijn.
5. In zeldzame gevallen ziet u deze fout ook als het wachtwoord van de gebruiker van het integratiesysteem is gewijzigd vanwege tenantvernieuwing of als het account is vergrendeld of verlopen. Controleer de status van de gebruiker van het integratiesysteem met uw Workday-beheerder.

Zie Zelfstudie: Werkdag configureren voor automatische gebruikers inrichting voor meer informatie over het configureren van [werkdagen voor geautomatiseerde inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
