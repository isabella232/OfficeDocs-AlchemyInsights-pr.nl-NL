---
title: Naadloze eenmalige aanmelding configureren (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966032"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Naadloze eenmalige aanmelding configureren (SSO)

**Toepassingen configureren**

1. U moet de waarden van de leverancier van de toepassing krijgen. U kunt de waarden handmatig invoeren of een metagegevensbestand uploaden om de waarde van de velden op te halen.
2. Veel apps zijn al vooraf geconfigureerd voor gebruik met Azure AD. Deze apps worden weergegeven in de galerie met apps die u kunt bekijken wanneer u een app toevoegt aan uw Azure AD-tenant. De [snelstartreeks loopt](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) door het proces.
3. Als u een niet-galerietoepassing wilt maken, kunt u klikken op **+ Knop Uw** eigen toepassing maken en een naam geven aan uw toepassing.
    - Standaard selecteert u Elke andere toepassing integreren die u niet **vindt in** de galerie, wat de juiste optie is voor toepassingen buiten de galerie.
    - Nadat u de **naam voor** de toepassing hebt gebruikt, wordt er een nieuwe ondernemingstoepassing zonder galerie gemaakt.
    - Vervolgens kunt u  onder Beheren van  die toepassing naar Een enkele aanmelding gaan en ziet u verschillende technieken voor de implementatie ervan in uw omgeving.

**Naadloze aanmelding configureren voor een specifieke toepassing**

Voor de apps in de galerie vindt u gedetailleerde, stapsgewijs instructies. Als u toegang wilt tot de stappen die u kunt doorlopen in een lijst met zelfstudies voor app-configuraties op [zelfstudies voor SaaS-apps.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML-gebaseerde SSSO configureren**

1. [Snelstart: SamL-gebaseerde single sign-on (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)instellen voor een toepassing in uw Azure Active Directory (Azure AD) tenant .
2. Zie Op SAML gebaseerde enkelvoudige aanmelding begrijpen voor meer informatie over de [saml-optie](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)voor een enkele aanmelding.
3. Zie Enkel Sign-On [SAML-protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)voor meer informatie over de SAML 2.0-verificatieaanvragen en -antwoorden die door Azure Active Directory (Azure AD) worden ondersteund voor Single Sign-On (SSO).
4. Zie SamL-gebaseerde eenmalige aanmelding configureren voor uw toepassing in Azure Active Directory (Azure AD) met de Microsoft Graph-API voor meer informatie over het maken en configureren van een op SAML gebaseerde eenmalige aanmelding voor uw toepassing met de [Microsoft Graph-API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Zie How the Microsoft identity platform uses the SAML protocol (Hoe de Microsoft identity platform het SAML-protocol gebruikt) voor meer informatie over het gebruik van [het SAML-protocol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)in Azure AD.

**Tokens en claims configureren**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Zie Claims die in tokens voor een specifieke app in een tenant worden uitgezonden aanpassen [(Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)voor meer informatie over het configureren van claims met PowerShell.
3. Zie Optionele claims voor uw app voor meer informatie over het configureren van optionele [claims.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Zie Adreslijstschemaextensiekenmerken gebruiken in claims voor meer informatie over het gebruik van [adreslijstschemaextensiekenmerken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)voor het verzenden van gebruikersgegevens naar toepassingen in tokenclaims.
5. Zie Configureerbare tokenlevens in de Microsoft identity platform (preview) voor meer informatie over het [configureren van tokenlevens.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Levensduurbeleid voor token configureren (voorbeeld)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - In dit artikel wordt een veelvoorkomende beleidsscenario beschreven waarin u nieuwe regels kunt instellen voor de levensduur van het token. In het voorbeeld leert u hoe u een beleid kunt maken dat vereist dat gebruikers zich vaker verifiëren in uw web-app.

**Problemen met SSO-configuratie oplossen**

- Zie voor veelgestelde vragen over Azure Active Directory Naadloze eenmalige Sign-On (Naadloze aanmeldingssso) Azure Active Directory Naadloze eenmalige [aanmelding: veelgestelde vragen.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Zie [Probleemoplossing](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)Azure Active Directory Naadloze eenmalige aanmelding voor meer informatie over veelvoorkomende problemen met betrekking tot Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).
