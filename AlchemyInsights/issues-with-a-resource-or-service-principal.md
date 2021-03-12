---
title: Problemen met een resource of service-principal
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713660"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemen met een resource of service-principal

1. Als u net aan de slag gaat, worden toepassings- en [service-principalobjecten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) beschreven waarin toepassingsregistratie, toepassingsobjecten en service-principals in Azure Active Directory worden beschreven: wat ze zijn, hoe ze worden gebruikt en hoe ze aan elkaar zijn gerelateerd. Er wordt ook een voorbeeldscenario met meerdere tenants weergegeven ter illustratie van de relatie tussen het toepassingsobject en de bijbehorende service-principalobjecten van een toepassing.
2. U vindt meer informatie over de relatie tussen toepassingen en service-principals door toepassingen en [service-principalobjecten te](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)lezen in Azure Active Directory.
3. [How to:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Use the portal to create an Azure AD application and service principal that can access resources shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Met de [service principal-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kunt u programmatisch exemplaren van toepassingen beheren en bepalen wat een toepassing in uw tenant kan doen.
5. [ServicePrincipal-resourcetype bevat](https://docs.microsoft.com/graph/api/resources/serviceprincipal) alle eigenschappen en methoden voor het servicePrincipal-resourcetype.
6. [Verschillen in resourcetype tussen Azure AD Graph en Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) zijn de verschillen tussen Azure AD Graph- en Microsoft Graph-bronnen. Hier worden resources met verschillende namen of die niet beschikbaar zijn. Ook worden bronnen weergegeven die beschikbaar zijn in de bètaversie van Microsoft Graph, maar niet in de versie v1.0.

**Problemen met gastgebruikers**

- [Snelstartgids:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Als u gastgebruikers toevoegt aan uw adreslijst in de Azure Portal, ziet u hoe u een nieuwe gastgebruiker kunt toevoegen aan uw Azure AD-adreslijst via de Azure Portal, een uitnodiging kunt verzenden en kunt bekijken hoe de uitnodiging voor de gastgebruiker wordt inwisseld.
- [Zelfstudie: Maak gebruikersstromen in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) en zie hoe u een aantal aanbevolen gebruikersstromen maakt met behulp van de Azure Portal. Als u informatie zoekt over het instellen van een ROPC-stroom (Resource Owner Password Credentials) in uw toepassing, zie De stroom wachtwoordreferenties voor de resourceeigenaar configureren in Azure AD B2C.
