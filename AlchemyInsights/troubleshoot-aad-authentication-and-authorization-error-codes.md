---
title: Foutcodes voor Azure AD Authentication and Authorization (AADSTS) oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035636"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Foutcodes voor Azure AD Authentication and Authorization (AADSTS) oplossen

Als u AAD-verificatie- en autorisatiefoutcodes (AADSTS) wilt oplossen, voert u de volgende aanbevolen stappen uit:

1. **Foutcodes in uw toepassing verwerken**

- De **OAuth2.0-spec**, biedt richtlijnen voor het verwerken van fouten tijdens verificatie met behulp van het foutgedeelte https://tools.ietf.org/html/rfc6749#section-5.2 van de foutreactie.

    - **fout**: Een foutcodereeks die kan worden gebruikt voor het classificeren van typen fouten die optreden en die moet worden gebruikt om op fouten te reageren.
    - Het **foutveld** bevat verschillende mogelijke waarden: bekijk de protocoldocumentatiekoppelingen en OAuth 2.0-specs voor meer informatie over specifieke fouten en hoe u hierop kunt reageren.

- Hier is een voorbeeld van een foutreactie:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Huidige foutcodegegevens opschonen**

- Foutcodes en berichten kunnen worden gewijzigd. Zie voor de meest recente informatie de pagina om AADSTS-foutbeschrijvingen, oplossingen en enkele voorgestelde https://login.microsoftonline.com/error tijdelijke oplossingen te zoeken.
- U kunt ook [AADSTS-foutcodes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) zoeken en oplossen in het artikel [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Hulp krijgen**

- [Ondersteunings-](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) en helpopties voor ontwikkelaars: als u een antwoord nodig hebt op een vraag of hulp bij het oplossen van een probleem dat niet in onze documentatie wordt bestreken, is het misschien tijd om contact op te nemen met experts voor hulp. Dit artikel bevat verschillende suggesties voor het verkrijgen van antwoorden op uw vragen terwijl u apps ontwikkelt die zijn geïntegreerd met het Microsoft-identiteitsplatform.








