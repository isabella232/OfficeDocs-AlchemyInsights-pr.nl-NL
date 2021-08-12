---
title: Problemen met wachtwoordgebaseerde naadloze eenmalige aanmelding (SSO) oplossen
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972819"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Problemen met wachtwoordgebaseerde naadloze eenmalige aanmelding (SSO) oplossen

Zie Op wachtwoord gebaseerde verificatie met een wachtwoord voor meer informatie over de basisprincipes van wachtwoordgebaseerde [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Wachtwoordgebaseerde aanmelding configureren**

1. [Eenmalige aanmelding configureren](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) op basis van een wachtwoord: dit artikel gaat in op meer informatie over de op wachtwoord gebaseerde SSO-optie. Als voor de toepassing die u toevoegt aangepaste configuratie is vereist en u een op wachtwoord gebaseerde aanmeldingsaanvraag moet gebruiken, is dit artikel voor u bedoeld.
2. Eén aanmelding op basis van een wachtwoord [configureren voor on-prem-apps-](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) Toepassingsproxy ondersteunt verschillende modi voor één aanmelding. Aanmelding op basis van een wachtwoord is bedoeld voor toepassingen met een combinatie van gebruikersnaam/wachtwoord voor verificatie. Wanneer u aanmelding op basis van een wachtwoord configureert voor uw toepassing, moeten uw gebruikers zich eenmaal aanmelden bij de on-premises toepassing. Daarna worden Azure Active Directory aanmeldingsgegevens op en worden deze automatisch aan de toepassing verstrekt wanneer uw gebruikers deze op afstand openen.
    - U had de app al moeten publiceren en testen met toepassingsproxy. Als dit niet het beste is, volgt u de stappen in Toepassingen publiceren met [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) en gaat u verder met de configuratie van op een wachtwoord gebaseerde SSSO voor on-prem-apps.

Zie Eenmalige aanmelding op basis van een wachtwoord oplossen [in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) voor problemen met wachtwoordgebaseerde aanmelding
