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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044983"
---
# <a name="configure-and-customize-applications"></a>Toepassingen configureren en aanpassen

**Toepassingen configureren**

1. [Snelstart: Eigenschappen configureren voor een toepassing in uw Azure Active Directory (Azure AD)-tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) laat zien hoe u een aantal eigenschappen voor een app configureert.
2. Om uw toepassingen te integreren met Azure Active Directory, hebben we een verzameling [zelfstudies](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) ontwikkeld die u door de configuratie helpen.
3. [Als u een toepassing voor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) toepassingsproxy configureert, begrijpt u hoe u een Toepassingsproxytoepassing configureert in Azure AD om uw on-premises toepassingen aan de cloud te laten zien.
4. [PingAccess downloaden](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)en uw toepassing configureren: Volg de instructies in *PingAccess* configureren voor Azure AD om toepassingen te beveiligen die zijn gepubliceerd met Microsoft Azure AD Application Proxy op de website pingidentiteit en download de nieuwste versie van PingAccess.

**Verkeerd geconfigureerde toepassingsfouten (AADSTS650056)**

1. Zorg ervoor dat u toegang hebt tot de toepassing vanaf het aanmeldingsadres van de eigenaar van de toepassing. Meld u anders aan bij de toepassing via het normale proces. In de meeste gevallen wordt dit automatisch automatisch opgelost. Als dit niet het probleem is, kan dit bericht u helpen het probleem op te lossen en op te lossen.
2. **Als uw organisatie eigenaar is van de toepassing** (wat betekent dat de toepassingsregistratie in uw organisatie is):
    - We raden ten minste de machtiging of gedelegeerde machtiging van Microsoft aan `User.Read` `openid` **Graph** wordt toegevoegd.
    - Zorg ervoor dat de toepassing en alle machtigingen worden ingestemd. U kunt dit controleren door de kolom **Status van** de toepassingsregistratie binnen **API-machtigingen te bekijken.**
    - In sommige scenario's is de toepassing mogelijk van derden, maar kan deze zijn geregistreerd in uw organisatie. Controleer of deze toepassing wordt vermeld in uw App-registraties (niet enterprise-toepassingen).
    - Als u dit foutbericht blijft zien. Vervolgens moet u mogelijk de toestemmings-URL maken die in **stap 4 wordt beschreven.**
3. **Als uw organisatie niet de eigenaar van de toepassing is en deze** gebruikt als een toepassing van derden:
    - Als u de globale/bedrijfsbeheerder bent, ziet u het toestemmingsscherm. Zorg ervoor dat u het selectievakje **'Toestemming namens uw organisatie' incheckt.**
    - Als u het toestemmingsscherm niet ziet, verwijdert u de Enterprise-toepassing en probeert u het opnieuw.
    - Als u dit foutbericht blijft zien. Vervolgens moet u mogelijk de toestemmings-URL maken die in **stap 4 wordt beschreven.**
4. Maak handmatig de **toestemmings-URL** die moet worden gebruikt: Als de toepassing is ontworpen voor toegang tot een specifieke resource, kunt u mogelijk de toestemmingsknoppen niet gebruiken vanuit de Azure-portal, u moet handmatig uw eigen toestemmings-URL genereren en deze gebruiken.
    - U moet het en het van de eigenaar van `{App-Id}` `{App-Uri-Id}` de toepassing krijgen. `{Tenant-Id}` wordt uw tenant-id. Dit is of `yourdomain.onmicrosoft.com` uw adreslijst-id.
    - Als de toepassing zelf toegang heeft tot de resource, is `{App-Id}` de toepassing `{App-Uri-Id}` hetzelfde.
5. Zie Problemen bij het aanmelden bij op SAML gebaseerde apps met één aanmelding [voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Toepassingen aanpassen**

- Huisstijl toevoegen aan de [Azure Active Directory-aanmeldingspagina](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) van uw organisatie: gebruik het logo en aangepaste kleurenschema's van uw organisatie om uw aanmeldingspagina's van Azure Active Directory (Azure AD) een consistent uiterlijk te geven.
- [Voeg uw aangepaste domeinnaam toe met de Azure Active Directory portal:](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) elke nieuwe Azure AD-tenant wordt geleverd met een eerste domeinnaam. U kunt de oorspronkelijke domeinnaam niet wijzigen of verwijderen, maar u kunt wel de namen van uw organisatie toevoegen. Als u aangepaste domeinnamen toevoegt, kunt u gebruikersnamen maken die bekend zijn bij uw gebruikers.
