---
title: API-machtigingen en toestemmingsproces
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
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932056"
---
# <a name="api-permissions-and-consent-process"></a>API-machtigingen en toestemmingsproces

Als uw app toegang heeft tot gegevens in Microsoft Graph, moet de gebruiker of beheerder deze de juiste machtigingen verlenen via een toestemmingsproces. [Microsoft Graph machtigingenverwijzing bevat](https://docs.microsoft.com/graph/permissions-reference) de machtigingen die zijn gekoppeld aan elke belangrijke set Microsoft-Graph API's. Het bevat ook richtlijnen voor het gebruik van de machtigingen.

**Service principal instellen of bijwerken**

- [Serviceprincipal maken:](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) in dit artikel wordt beschreven hoe u een nieuw servicePrincipal-object maakt.
- [Maak een Azure AD-app &-service](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) principal in de portal: in dit artikel wordt beschreven hoe u een nieuwe Azure Active Directory-toepassing en service principal (Azure AD) kunt maken die kunnen worden gebruikt met het op rollen gebaseerde toegangsbeheer.
- [Apps & service-principals in Azure AD: in](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) dit artikel worden toepassingsregistratie, toepassingsobjecten en service-principals in Azure Active Directory beschreven: wat ze zijn, hoe ze worden gebruikt en hoe ze aan elkaar zijn gerelateerd.

**App-registratie toevoegen of bijwerken en toestemming geven voor beheerders**

- [Een app-registratie maken:](https://docs.microsoft.com/graph/api/application-post-applications) in dit artikel ziet u hoe u een nieuw toepassingsobject maakt.
- [Een app-registratie bijwerken - API-machtigingen](https://docs.microsoft.com/graph/api/application-update) - In dit artikel wordt beschreven hoe u de eigenschappen van een toepassingsobject kunt bijwerken.
- [Toestemming van beheerder verlenen:](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) voor toestemming van de beheerder en toestemming in het algemeen is vereist dat een beheerder expliciet toestemming verleent.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Rollenbeheercontainer voor geïntegreerde roldefinities en roltoewijzingen voor Microsoft 365 RBAC-providers die meerdere principals en meerdere scopes in één roltoewijzing ondersteunen. Dit verschilt van *het resourcetype rbacApplication.* Microsoft Intune is een voorbeeld van een dergelijke RBAC-provider. Een roltoewijzing in Intune kan een matrix van principals en een matrix van bereikgroepen hebben. **Dit is in beta, wat betekent dat het nog in ontwikkeling is en niet wordt aanbevolen voor gebruik in de productie.**
