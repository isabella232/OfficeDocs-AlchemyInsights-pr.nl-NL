---
title: Toepassingen configureren en aanpassen
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063616"
---
# <a name="configure-and-customize-applications"></a>Toepassingen configureren en aanpassen

**Toepassingen configureren**

1. [Snelstartgids: Configureer eigenschappen](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) voor een toepassing in uw Azure Active Directory-tenant (Azure AD) en laat zien hoe u enkele eigenschappen voor een app kunt configureren.
2. Om uw toepassingen te helpen integreren met Azure Active Directory, hebben we een [verzameling](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) zelfstudies ontwikkeld die u de configuratie doorloopt.
3. [Als u een toepassing voor een](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) toepassingsproxy configureert, weet u hoe u een toepassingsproxytoepassing configureert in Azure AD om uw on-premises toepassingen beschikbaar te stellen aan de cloud.
4. [Download PingAccess en](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)configureer uw toepassing: Volg de instructies in *PingAccess* voor Azure AD configureren om toepassingen te beveiligen die zijn gepubliceerd via microsoft Azure AD-toepassingsproxy op de website van Ping Identity en de nieuwste versie van PingAccess te downloaden.

**Fouten in onjuist geconfigureerde toepassing (AADSTS650056)**

1. Controleer of u toegang hebt tot de toepassing via het aanmeldingsadres dat u hebt verstrekt door de eigenaar van de toepassing. Anders betekent dit dat u zich via het normale proces bij de toepassing moet aanmelden. In de meeste gevallen wordt dit automatisch opgelost. Als dat niet zo is, kan dit bericht u helpen bij het oplossen van problemen.
2. **Als uw organisatie eigenaar is van de toepassing** (dat wil zeggen dat de toepassingsregistratie in uw organisatie is):
    - We raden u ten minste aan de of gedelegeerde machtiging `User.Read` van Microsoft `openid` **Graph** toe te voegen.
    - Zorg ervoor dat de toepassing en alle machtigingen instemt. U kunt dit controleren door de kolom **Status van** de toepassingsregistratie in API-machtigingen **te bekijken.**
    - In sommige gevallen is de toepassing mogelijk van derden, maar is deze mogelijk geregistreerd in uw organisatie. Controleer of deze toepassing wordt vermeld in uw App-registraties (niet enterprise-toepassingen).
    - Als dit foutbericht nog steeds wordt weergegeven. Dan moet u mogelijk de toestemmings-URL opbouwen die wordt beschreven in **stap 4.**
3. **Als uw organisatie niet de eigenaar van de toepassing is en deze** als toepassing van derden gebruikt:
    - Als u de globale/bedrijfsbeheerder bent, moet u het toestemmingsscherm zien. Zorg ervoor dat u het selectievakje **'Toestemming namens uw organisatie' incheckt.**
    - Als u het toestemmingsscherm niet ziet, verwijdert u de Enterprise-toepassing en probeert u het opnieuw.
    - Als dit foutbericht nog steeds wordt weergegeven. Dan moet u mogelijk de toestemmings-URL opbouwen die wordt beschreven in **stap 4.**
4. Stel de toestemmings-URL handmatig in om te worden gebruikt: als de toepassing is ontworpen voor toegang tot een bepaalde bron, kunt u mogelijk de toestemmingsknoppen van de Azure Portal niet gebruiken. U moet uw eigen toestemmings-URL handmatig genereren en deze gebruiken.
    - U moet de toepassing en de `{App-Id}` `{App-Uri-Id}` toepassingseigenaar op te halen. `{Tenant-Id}` wordt uw tenant-id. Dit is uw `yourdomain.onmicrosoft.com` adreslijst-id.
    - Als de toepassing zichzelf voor de resource gebruikt, is de ene `{App-Id}` `{App-Uri-Id}` toepassing gelijk.
5. Zie Problemen bij het aanmelden bij op SAML gebaseerde apps met een enkele aanmelding [voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Toepassingen aanpassen**

- U kunt een huisstijl toevoegen aan de aanmeldingspagina van [Azure Active Directory van](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) uw organisatie. Gebruik het logo en aangepaste kleurenschema's van uw organisatie om uw aanmeldingspagina's voor Azure Active Directory (Azure AD) een consistent uiterlijk te geven.
- [Voeg uw aangepaste domeinnaam toe met behulp van de Azure Active Directory-portal:](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) elke nieuwe Azure AD-tenant wordt geleverd met een oorspronkelijke domeinnaam. U kunt de oorspronkelijke domeinnaam niet wijzigen of verwijderen, maar u kunt wel de namen van uw organisatie toevoegen. Door aangepaste domeinnamen toe te voegen, kunt u gebruikersnamen maken die voor uw gebruikers bekend zijn.
