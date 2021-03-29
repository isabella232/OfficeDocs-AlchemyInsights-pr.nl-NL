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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402262"
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

1. [Snelstart: SamL-gebaseerde single sign-on (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)instellen voor een toepassing in uw Azure Active Directory -tenant (Azure AD).
2. Zie Op SAML gebaseerde enkelvoudige aanmelding begrijpen voor meer informatie over de [saml-optie](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)voor een enkele aanmelding.
3. Zie Enkel Sign-On [SAML-protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)voor meer informatie over de SAML 2.0-verificatieaanvragen en -antwoorden die Azure Active Directory (Azure AD) ondersteunt voor Eenmalige Sign-On (SSO).
4. Zie SamL-gebaseerde eenmalige aanmelding configureren voor uw toepassing in Azure Active Directory (Azure AD) met de Microsoft Graph-API voor meer informatie over het maken en configureren van een op SAML gebaseerde eenmalige aanmelding voor uw toepassing met de [Microsoft Graph-API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Zie Hoe het [Microsoft-identiteitsplatform het SAML-protocol gebruikt](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)voor meer informatie over het gebruik van het SAML-protocol in Azure AD.

**Tokens en claims configureren**

1. [How to: customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Zie Claims die in tokens voor een specifieke app in een tenant worden uitgezonden aanpassen [(Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)voor meer informatie over het configureren van claims met PowerShell.
3. Zie Optionele claims voor uw app voor meer informatie over het configureren van optionele [claims.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Zie Adreslijstschemaextensiekenmerken gebruiken in claims voor meer informatie over het gebruik van [adreslijstschemaextensiekenmerken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)voor het verzenden van gebruikersgegevens naar toepassingen in tokenclaims.
5. Zie [Configureerbare tokenlevens in het Microsoft-identiteitsplatform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)voor meer informatie over het configureren van tokenlevens.
6. [Levensduurbeleid voor token configureren (voorbeeld)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - In dit artikel wordt een veelvoorkomende beleidsscenario beschreven waarin u nieuwe regels kunt instellen voor de levensduur van het token. In het voorbeeld leert u hoe u een beleid kunt maken dat vereist dat gebruikers zich vaker verifiëren in uw web-app.

**Problemen met SSO-configuratie oplossen**

- Zie [Azure Active Directory Seamless Single Sign-On: Veelgestelde vragen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)voor veelgestelde vragen over Azure Active Directory Seamless Single Sign-On (Seamless SSO).
- Zie Azure Active Directory Seamless Single [Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)(Naadloze aanmelding) oplossen voor informatie over veelvoorkomende problemen met Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).
