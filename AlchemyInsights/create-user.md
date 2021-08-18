---
title: Gebruiker maken
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323281"
---
# <a name="create-user"></a>Gebruiker maken

**AANKONDIGING:**

- [De aanmeldingsondersteuning voor WebView bij Google wordt vanaf 4 januari 2021 verwijderd.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Test of uw apps mogelijk worden beïnvloed door de richtlijnen [van Google voor](https://go.microsoft.com/fwlink/?linkid=2157323) het testen van compatibiliteit te volgen.
- Zorg ervoor dat u de systeemwebweergave of systeembrowser gebruikt wanneer u zich aanmeldt bij uw gebruikers met google-accounts voor consumenten. Zie Problemen met het aanmelden [bij toepassing(en) met alleen de Chrome-browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)voor meer informatie.

**Ik kan geen nieuwe gebruiker maken in mijn Azure AD-adreslijst**

1. Zorg ervoor dat u gemachtigd bent om een nieuwe standaardgebruiker te maken. Alleen de globale beheerder of de rol van gebruikerbeheerder in Azure Active Directory (AD) kan een nieuwe standaardgebruiker maken. Als u niet in een van deze rollen zit, vraagt u een beheerder om u toe te voegen aan een van deze rollen of om het nieuwe gebruikersaccount voor u te maken.
1. Controleer of de gebruikersnaam zich in een domein dat is geverifieerd in uw Azure AD. Als u geen geverifieerde aangepaste domeinnamen hebt in uw Azure AD, kunt u het oorspronkelijke Azure AD-domein gebruiken, dat eindigt op *.onmicrosoft.com.
1. Controleer of de gebruikersnaam zich in een domein dat niet is federatief aan Azure AD vanuit uw on-premises AD. Gebruikers kunnen niet worden toegevoegd in de cloud met domeinnamen die vanuit on-premises federatief zijn.
1. Zorg ervoor dat geen andere gebruiker of contactpersoon al de gebruikersnaam heeft die u aan de nieuwe gebruiker wilt toewijzen. Gebruikersnamen moeten uniek zijn in Azure AD.
1. Zie [Azure AD-rollen en -beheerders](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) voor uw Azure AD.
1. Bekijk de [domeinnamen voor](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) uw Azure AD.
1. Controleer [auditlogboeken](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) voor meer gedetailleerde informatie over een onlangs gemaakte of verwijderde gebruiker, zoals wie de actie heeft uitgevoerd en wanneer.
1. Zie De [Azure-portal](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)gebruiken om een nieuwe gebruiker te maken in uw Azure AD voor meer informatie over het toevoegen van nieuwe gebruikers.
1. [Azure AD-beheerrollen:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)beheerdersrolmachtigingen in Azure Active Directory
1. U kunt azure [AD PowerShell ook gebruiken om een nieuwe gebruiker te maken.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
