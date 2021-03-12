---
title: Problemen met naadloze eenmalige aanmelding (SSO) met een wachtwoord oplossen
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714710"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Problemen met naadloze eenmalige aanmelding (SSO) met een wachtwoord oplossen

Zie Wachtwoordgebaseerde verificatie bij Azure Active [Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)voor meer informatie over de basisprincipes van wachtwoordgebaseerde SSO.

**Wachtwoordgebaseerde eenmalige aanmelding configureren**

1. [Eenmalige aanmelding op basis](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) van een wachtwoord configureren: in dit artikel wordt meer informatie besproken over de optie voor eenmalige aanmelding op basis van een wachtwoord. Als voor de toepassing die u toevoegt een aangepaste configuratie is vereist en u een wachtwoordgebaseerde eenmalige aanmelding moet gebruiken, is dit artikel bedoeld voor u.
2. [Wachtwoordgebaseerde een-op-een-aanmelding configureren voor on-prem-apps.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) Toepassingsproxy ondersteunt verschillende modi voor een een aanmelding. Aanmelden via een wachtwoord is bedoeld voor toepassingen die een combinatie van gebruikersnaam en wachtwoord gebruiken voor verificatie. Wanneer u wachtwoordregistratie voor uw toepassing configureert, moeten uw gebruikers zich eenmaal aanmelden bij de on-premises toepassing. Daarna worden de aanmeldingsgegevens op slaat Azure Active Directory op en wordt deze automatisch aan de toepassing verstrekt wanneer uw gebruikers deze extern openen.
    - U moet uw app al hebben gepubliceerd en getest met toepassingsproxy. Als dat niet zo is, volgt u de stappen in Toepassingen publiceren met behulp van Azure AD-toepassingsproxy en gaat u vervolgens verder met uw configuratie van wachtwoordgebaseerde SSO voor on-prem-apps. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Zie Problemen met eenmalige aanmelding op basis van een wachtwoord [oplossen in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) als u problemen met een wachtwoord voor eenmalige aanmelding wilt oplossen
