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
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="f74fe-102">Een lijst met enterprise-toepassingen krijgen</span><span class="sxs-lookup"><span data-stu-id="f74fe-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="f74fe-103">Zie [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)voor een lijst met ondernemingstoepassingen (alle toepassingen **of** gefilterd op weergavenaam, id, ID-URL's, enzovoort).</span><span class="sxs-lookup"><span data-stu-id="f74fe-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="f74fe-104">Zie [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)voor een lijst met serviceprincipaalobjecten (alle objecten of gefilterd op id) via de powershell-opdracht.</span><span class="sxs-lookup"><span data-stu-id="f74fe-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="f74fe-105">Als u een lijst **met geconfigureerde SAML-apps wilt krijgen,** kunt u mogelijk de volgende PowerShell-scripts volgen:</span><span class="sxs-lookup"><span data-stu-id="f74fe-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="f74fe-106">Elke toepassing is een OAuth-app of SAML-app (zowel galerie- als niet-galerie-apps) die twee objecten in AAD hebben gemaakt wanneer ze worden geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="f74fe-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="f74fe-107">Het ene wordt het toepassingsobject genoemd en het andere is het object Service principal.</span><span class="sxs-lookup"><span data-stu-id="f74fe-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="f74fe-108">Wanneer u de eigenschappen van een Service Principal-object dumpt met PowerShell, ziet u dat elke toepassing een bepaald aantal tags heeft dat aan het object is gekoppeld, zoals:</span><span class="sxs-lookup"><span data-stu-id="f74fe-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="f74fe-109">OAuth-apps zouden een tag hebben met de naam **" WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="f74fe-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="f74fe-110">Galerie SAML-apps zou een tag hebben met de naam "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="f74fe-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="f74fe-111">Non-Gallery SAML Apps zou een tag hebben met de naam "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="f74fe-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="f74fe-112">Daarom kunt u deze tags gebruiken en erachter komen wat voor app het is.</span><span class="sxs-lookup"><span data-stu-id="f74fe-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="f74fe-113">De tag **WindowsAzureActiveDirectoryIntegratedApp** is gebruikelijk voor alle typen apps.</span><span class="sxs-lookup"><span data-stu-id="f74fe-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="f74fe-114">U kunt het volgende fragment gebruiken om alle SAML-apps (zowel galerie als niet-galerie) op te geven:</span><span class="sxs-lookup"><span data-stu-id="f74fe-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="f74fe-115">Zie [SamL-apps](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)identificeren in Azure AD voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f74fe-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="f74fe-116">**Alleen webtoepassingen** zoeken en gebruiken: Gebruik de onderstaande opdracht om alle Azure AD-toepassingen te downloaden met het toepassingstype 'Web app/API'</span><span class="sxs-lookup"><span data-stu-id="f74fe-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="f74fe-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="f74fe-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="f74fe-118">**Alleen native toepassingen zoeken en weergeven:** Voer de volgende opdracht uit om alle native clienttoepassingen (desktop/mobiel apparaat) te krijgen.</span><span class="sxs-lookup"><span data-stu-id="f74fe-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="f74fe-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="f74fe-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="f74fe-120">**Alle geregistreerde Azure AD-toepassingsgegevens** exporteren naar CSV: Met de onderstaande opdracht worden alle Azure AD-apps met de vereiste details geëxporteerd naar een CSV-bestand:</span><span class="sxs-lookup"><span data-stu-id="f74fe-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="f74fe-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="f74fe-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="f74fe-122">Export-Csv 'C:\AzureADApps.csv' -NoTypeInformation -Codering UTF8</span><span class="sxs-lookup"><span data-stu-id="f74fe-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="f74fe-123">**Een lijst met ongebruikte Azure-apps exporteren :** auditrapport</span><span class="sxs-lookup"><span data-stu-id="f74fe-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="f74fe-124">Azure AD kan toepassingslogboeken maximaal 30 dagen tonen, mits u een Azure AD Premium-licentie hebt.</span><span class="sxs-lookup"><span data-stu-id="f74fe-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="f74fe-125">U hebt twee opties om de gegevens langer dan 30 dagen te bewaren.</span><span class="sxs-lookup"><span data-stu-id="f74fe-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="f74fe-126">U kunt de [API's voor Azure AD Reporting gebruiken](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) om de gegevens programmatisch op te halen en op te slaan in een database.</span><span class="sxs-lookup"><span data-stu-id="f74fe-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="f74fe-127">U kunt ook auditlogboeken integreren in een SIEM-systeem van derden.</span><span class="sxs-lookup"><span data-stu-id="f74fe-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="f74fe-128">U kunt ook de lijst met apps downloaden voor alle toepassingen en eigendomstoepassingen onder Azure Active Directory>App Registrations>Download>Alle toepassingen/eigendomstoepassingen.</span><span class="sxs-lookup"><span data-stu-id="f74fe-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="f74fe-129">Zie Lijsttoepassingen - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/application-list) en [toepassingsresourcetype - Microsoft Graph v1.0 voor](https://docs.microsoft.com/graph/api/resources/application)een lijst met toepassingen via MS Graph .</span><span class="sxs-lookup"><span data-stu-id="f74fe-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
