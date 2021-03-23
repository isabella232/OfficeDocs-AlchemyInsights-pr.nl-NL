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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="6324a-102">Foutcodes voor Azure AD Authentication and Authorization (AADSTS) oplossen</span><span class="sxs-lookup"><span data-stu-id="6324a-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="6324a-103">Als u AAD-verificatie- en autorisatiefoutcodes (AADSTS) wilt oplossen, voert u de volgende aanbevolen stappen uit:</span><span class="sxs-lookup"><span data-stu-id="6324a-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="6324a-104">**Foutcodes in uw toepassing verwerken**</span><span class="sxs-lookup"><span data-stu-id="6324a-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="6324a-105">De **OAuth2.0-spec**, biedt richtlijnen voor het verwerken van fouten tijdens verificatie met behulp van het foutgedeelte https://tools.ietf.org/html/rfc6749#section-5.2 van de foutreactie.</span><span class="sxs-lookup"><span data-stu-id="6324a-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="6324a-106">**fout**: Een foutcodereeks die kan worden gebruikt voor het classificeren van typen fouten die optreden en die moet worden gebruikt om op fouten te reageren.</span><span class="sxs-lookup"><span data-stu-id="6324a-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="6324a-107">Het **foutveld** bevat verschillende mogelijke waarden: bekijk de protocoldocumentatiekoppelingen en OAuth 2.0-specs voor meer informatie over specifieke fouten en hoe u hierop kunt reageren.</span><span class="sxs-lookup"><span data-stu-id="6324a-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="6324a-108">Hier is een voorbeeld van een foutreactie:</span><span class="sxs-lookup"><span data-stu-id="6324a-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="6324a-109">**Huidige foutcodegegevens opschonen**</span><span class="sxs-lookup"><span data-stu-id="6324a-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="6324a-110">Foutcodes en berichten kunnen worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="6324a-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="6324a-111">Zie voor de meest recente informatie de pagina om AADSTS-foutbeschrijvingen, oplossingen en enkele voorgestelde https://login.microsoftonline.com/error tijdelijke oplossingen te zoeken.</span><span class="sxs-lookup"><span data-stu-id="6324a-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="6324a-112">U kunt ook [AADSTS-foutcodes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) zoeken en oplossen in het artikel [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="6324a-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="6324a-113">**Hulp krijgen**</span><span class="sxs-lookup"><span data-stu-id="6324a-113">**Get Help**</span></span>

- <span data-ttu-id="6324a-114">[Ondersteunings-](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) en helpopties voor ontwikkelaars: als u een antwoord nodig hebt op een vraag of hulp bij het oplossen van een probleem dat niet in onze documentatie wordt bestreken, is het misschien tijd om contact op te nemen met experts voor hulp.</span><span class="sxs-lookup"><span data-stu-id="6324a-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="6324a-115">Dit artikel bevat verschillende suggesties voor het verkrijgen van antwoorden op uw vragen terwijl u apps ontwikkelt die zijn geïntegreerd met het Microsoft-identiteitsplatform.</span><span class="sxs-lookup"><span data-stu-id="6324a-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








