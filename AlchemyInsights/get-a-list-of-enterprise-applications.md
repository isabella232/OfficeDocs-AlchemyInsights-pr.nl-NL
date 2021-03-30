---
title: Een lijst met enterprise-toepassingen krijgen
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404531"
---
# <a name="get-a-list-of-enterprise-applications"></a>Een lijst met enterprise-toepassingen krijgen

1. Zie [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)voor een lijst met ondernemingstoepassingen (alle toepassingen **of** gefilterd op weergavenaam, id, ID-URL's, enzovoort).
2. Zie [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)voor een lijst met serviceprincipaalobjecten (alle objecten of gefilterd op id) via de powershell-opdracht.
3. Als u een lijst **met geconfigureerde SAML-apps wilt krijgen,** kunt u mogelijk de volgende PowerShell-scripts volgen:

    Elke toepassing is een OAuth-app of SAML-app (zowel galerie- als niet-galerie-apps) die twee objecten in AAD hebben gemaakt wanneer ze worden geregistreerd. Het ene wordt het toepassingsobject genoemd en het andere is het object Service principal. Wanneer u de eigenschappen van een Service Principal-object dumpt met PowerShell, ziet u dat elke toepassing een bepaald aantal tags heeft dat aan het object is gekoppeld, zoals:

    - OAuth-apps zouden een tag hebben met de naam **" WindowsAzureActiveDirectoryIntegratedApp**"
    - Galerie SAML-apps zou een tag hebben met de naam "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Non-Gallery SAML Apps zou een tag hebben met de naam "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Daarom kunt u deze tags gebruiken en erachter komen wat voor app het is. De tag **WindowsAzureActiveDirectoryIntegratedApp** is gebruikelijk voor alle typen apps. U kunt het volgende fragment gebruiken om alle SAML-apps (zowel galerie als niet-galerie) op te geven:

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Zie [SamL-apps](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)identificeren in Azure AD voor meer informatie.

4. **Alleen webtoepassingen** zoeken en gebruiken: Gebruik de onderstaande opdracht om alle Azure AD-toepassingen te downloaden met het toepassingstype 'Web app/API'

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Alleen native toepassingen zoeken en weergeven:** Voer de volgende opdracht uit om alle native clienttoepassingen (desktop/mobiel apparaat) te krijgen.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Alle geregistreerde Azure AD-toepassingsgegevens** exporteren naar CSV: Met de onderstaande opdracht worden alle Azure AD-apps met de vereiste details geëxporteerd naar een CSV-bestand:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv 'C:\AzureADApps.csv' -NoTypeInformation -Codering UTF8

7. **Een lijst met ongebruikte Azure-apps exporteren :** auditrapport

    Azure AD kan toepassingslogboeken maximaal 30 dagen tonen, mits u een Azure AD Premium-licentie hebt.
    U hebt twee opties om de gegevens langer dan 30 dagen te bewaren. U kunt de [API's voor Azure AD Reporting gebruiken](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) om de gegevens programmatisch op te halen en op te slaan in een database. U kunt ook auditlogboeken integreren in een SIEM-systeem van derden.

    U kunt ook de lijst met apps downloaden voor alle toepassingen en eigendomstoepassingen onder Azure Active Directory>App Registrations>Download>Alle toepassingen/eigendomstoepassingen.

    Zie Lijsttoepassingen - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/application-list) en [toepassingsresourcetype - Microsoft Graph v1.0 voor](https://docs.microsoft.com/graph/api/resources/application)een lijst met toepassingen via MS Graph .
