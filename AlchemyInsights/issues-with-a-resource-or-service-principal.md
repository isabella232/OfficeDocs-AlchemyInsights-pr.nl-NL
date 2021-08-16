---
title: Problemen met een Resource of Service Principal
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028071"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemen met een Resource of Service Principal

1. Als u nog maar net aan de slag bent, worden toepassings- en serviceprincipaalobjecten [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) beschreven voor toepassingsregistratie, toepassingsobjecten en service-principals in Azure Active Directory: wat ze zijn, hoe ze worden gebruikt en hoe ze aan elkaar zijn gerelateerd. Er wordt ook een voorbeeldscenario voor meerdere tenants weergegeven om de relatie tussen het toepassingsobject van een toepassing en de bijbehorende serviceprincipaalobjecten te illustreren.
2. U kunt meer informatie krijgen over de relatie tussen toepassingen en service-principals door toepassingen en [serviceprincipaalobjecten in](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)Azure Active Directory.
3. [How to:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Use the portal to create an Azure AD application and service principal that can access resources shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Met de [service principal API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kunt u programmatisch exemplaren van toepassingen beheren en bepalen wat een toepassing binnen uw tenant kan doen.
5. [servicePrincipal resourcetype bevat](https://docs.microsoft.com/graph/api/resources/serviceprincipal) alle eigenschappen en methoden voor het servicePrincipal-resourcetype.
6. [Verschillen in resourcetype tussen Azure AD-Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) worden belicht verschillen tussen Azure AD-Graph en Microsoft Graph resources. Hier ziet u resources die verschillende namen hebben of die niet beschikbaar zijn. Ook worden bronnen belicht die beschikbaar zijn in de bètaversie van Microsoft Graph maar niet in de v1.0-versie.

**Problemen met gastgebruikers**

- Snelstart: Als u gastgebruikers toevoegt aan uw adreslijst in de [Azure-portal,](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) ziet u hoe u een nieuwe gastgebruiker toevoegt aan uw Azure AD-adreslijst via de Azure-portal, een uitnodiging verzendt en ziet hoe het inwisselingsproces van de gastgebruiker eruitziet.
- [Zelfstudie: Maak gebruikersstromen in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) laat zien hoe u een aantal aanbevolen gebruikersstromen maakt met behulp van de Azure-portal. Zie De wachtwoordreferentiesstroom voor resourceeigenaar configureren in Azure AD B2C als u informatie zoekt over het instellen van een ROPC-stroom (Resource Owner Password Credentials) in uw toepassing.
