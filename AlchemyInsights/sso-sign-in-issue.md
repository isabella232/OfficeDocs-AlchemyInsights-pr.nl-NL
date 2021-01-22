---
title: Naadloze aanmeldingsproblemen met eenmalige aanmelding van gebruikers
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935120"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Naadloze aanmeldingsproblemen met eenmalige aanmelding van gebruikers

Nadat de gebruiker is geverifieerd, worden de referenties van de gebruiker in de browser in de cache opgeslagen, zodat in dezelfde browser de toepassing automatisch wordt aanmelden met hetzelfde account. Dit kan het lastig maken voor een andere gebruiker of één gebruiker om zich aan te melden bij meerdere accounts op één apparaat. Om dit op te lossen: 1. Probeer u aan te melden in een andere browser. 2. Leeg de cache en/of cookies van de browser en probeer u opnieuw aan te melden.

Als u nog steeds aanmeldingsproblemen ondervindt, raden we u aan de volgende stappen vast te stellen en te automatiseren:

1. Installeer de secure browseruitbreiding mijn [apps](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) om Azure Active Directory (Azure AD) te helpen betere diagnose en oplossingen te bieden bij het gebruik van de testervaring in de Azure Portal.
2. Reproduceer de fout met behulp van de testervaring op de pagina voor app-configuratie in de Azure Portal. Zie Op SAML gebaseerde toepassingen voor een aanmelding op basis van SAML voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Als u de testervaring in de Azure Portal gebruikt met de secure browseruitbreiding voor Mijn apps, kunt **u stap 4 overslaan.**
4. De configuratiepagina voor een enkele aanmelding op basis van SAML openen:
    - Open de [Azure-portal](https://portal.azure.com/) en meld u aan als **globale beheerder** of **coadmin.**
    - Open de **Azure Active Directory-extensie** door **Alle services boven** aan het hoofdnavigatiemenu aan de linkerkant te selecteren.
    - Typ Azure Active Directory in het filterzoekvak en selecteer het **Azure Active Directory-item.**
    - Selecteer **Ondernemingstoepassingen** in het linkernavigatiemenu van Azure Active Directory.
    - Selecteer **Alle toepassingen om** een lijst met al uw toepassingen te bekijken. Als de wante toepassing hier niet wordt weergegeven, gebruikt  u het **filterbesturingselement** boven aan de lijst met alle toepassingen en stelt u de optie Voorstelling in op **Alle toepassingen.** 
    - Selecteer de toepassing die u wilt configureren voor een een aanmelding.
    - Nadat de toepassing is geladen, **selecteert u** Een aanmelding in het linkernavigatiemenu van de toepassing.
    - Selecteer **SSO op basis van SAML.**
5. Op basis van de fout vindt u meer informatie over de aanbevolen stappen die u moet volgen. Zie Problemen met aanmelden bij op SAML gebaseerde apps voor een enkel aanmelding [geconfigureerde app.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Raadpleeg de volgende richtlijnen om andere aanmeldingsproblemen voor gebruikers op te lossen:
    - [Enkel Sign-On SAML-protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Aanmeldingsfouten oplossen met Azure Active Directory-rapporten](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Onverwachte toestemmingsprompt](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Fout in toestemming van gebruiker](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemen met aanmelden vanuit Mijn apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Fout op aanmeldingspagina van toepassing](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Probleem bij het aanmelden bij een Microsoft-app](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
