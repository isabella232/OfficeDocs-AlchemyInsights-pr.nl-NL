---
title: Problemen met SAML-ondertekeningscertificaat oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692909"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Problemen met SAML-ondertekeningscertificaat oplossen

Voer de volgende aanbevolen stappen uit om het probleem met het SAML-handtekeningcertificaat op te lossen:

1. Wanneer u een bedrijfstoepassing toevoegt die SSO ondersteunt, wordt in Azure een certificaat gegenereerd dat het [SAML-handtekeningcertificaat wordt genoemd.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Dit certificaat heeft een vervaldatum van 3 jaar. Zie De vervaldatum voor uw federatiecertificaat aanpassen en doorvernieuwen naar een nieuw certificaat als u de vervaldatum van uw certificaat [wilt wijzigen.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure gebruikt dit certificaat om de SAML-tokens te ondertekenen die door de toepassing zijn aangevraagd en deze naar de toepassing te sturen voor een succesvolle eenmalige aanmelding. Download het certificaat van de Azure Portal en stuur het naar de leverancier van de toepassing om het SSO-proces te voltooien.

Nadat dit proces is voltooid, vertrouwt uw toepassing dit certificaat en worden alle SAML-tokens die door dit certificaat zijn ondertekend, geaccepteerd door de toepassing.

3. Als dit certificaat is verlopen, maakt u een nieuw certificaat, werk het bij naar de leverancier van de toepassing en maakt u het vervolgens actief aan de Azure-kant. Zie Een certificaat verlengen [dat binnenkort verloopt, voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Als het certificaat verloopt, wordt de gebruiker niet geblokkeerd.

4. [Voeg een e-mailadres toe voor meldingen](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) die moeten worden ontvangen voordat het huidige certificaat verloopt.

> [!NOTE]
> Stap 4 is optioneel.

5. Wijzig de opties voor SAML-certificaat ondertekening van een toepassing en het algoritme voor certificaat ondertekening. Zie Opties voor het ondertekenen van certificaten en het [handtekeningsalgoritme wijzigen voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

