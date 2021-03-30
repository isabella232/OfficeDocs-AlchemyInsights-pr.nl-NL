---
title: Ontbrekende toepassingen zoeken op app-registratieblad
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404414"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Ontbrekende toepassingen zoeken op app-registratieblad

1. Toepassingen kunnen niet worden gevonden in de app-registratieportal.

    Als een toepassing een toepassing met meerdere tenants is en deze is geregistreerd in een andere tenant, wordt deze niet weergegeven onder app-registratieblad. Het is echter mogelijk dat u deze onder Enterprise Applications-blade vindt nadat deze is gebruikt (nadat u toestemming hebt gegeven) en de serviceprincipaal is gemaakt in uw tenant. Zie Apps & [service principals in Azure AD - Microsoft identity platform voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Apps kunnen niet worden bekeken in het app-registratieblad, zelfs niet als u een beheerder bent.

    Zorg ervoor dat u in de juiste adreslijst van de Azure-portal bent.
3. Mijn toepassing wordt niet weergegeven onder enterprise applications blade, maar wordt weergegeven wanneer ik de opdracht PowerShell bevraag.

    Soms wordt de toepassing, nadat u de toepassing hebt verwijderd uit de Azure-portal, niet in de portal, maar mogelijk niet volledig verwijderd. Zie voor meer informatie:
    - U kunt de lijst met eerder verwijderde toepassingen ophalen en zien of de toepassing wordt weergegeven in de lijst met de **powershell-opdracht: Get-AzureADDeletedApplication**. Zie [Get-AzureADDeletedApplication (AzureAD) voor meer informatie.](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Als u de toepassing volledig wilt verwijderen, kunt u het volgende proberen in PowerShell: **Remove-AzureADApplication -ObjectId**. Zie [Remove-AzureADApplication (AzureAD) voor meer informatie.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - U kunt ook proberen de verwijderde toepassing te herstellen met de volgende PowerShell-opdracht: **AzureADDeletedApplication herstellen -ObjectId.** Zie [Restore-AzureADDeletedApplication (AzureAD) voor meer informatie.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Kan geen lijst met alle vooraf geïnstalleerde bedrijfstoepassingen vinden in mijn nieuwe Azure-tenant.

    Er zijn standaard geen vooraf geïnstalleerde bedrijfstoepassingen in Azure AD. U moet deze handmatig toevoegen vanuit de optie 'Nieuwe toepassing' door te bladeren vanuit de Azure AD-galerie of een niet-galerietoepassing toe te voegen. Zie Snelstart: Een toepassing toevoegen aan uw [Azure Active Directory-tenant (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)voor meer informatie.
    Als u een globale beheerder bent, hebt u eenvoudig toegang tot uw apps met behulp van het start programma voor apps van [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Mijn apps kunnen niet worden gevonden via de portal Mijn apps.

    Zorg ervoor dat apps niet zijn verborgen op de pagina Mijn apps-verzameling. Zie Verzamelingen [(voorbeeld) in de portal Mijn apps - Azure AD voor meer informatie.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Als u apps wilt starten vanuit de portal Mijn apps, [zie Zoeken naar & apps gebruiken op](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)de portal Mijn apps - Azure AD .
7. De Office 365 Mover-app wordt na de installatie niet weergegeven in de Enterprise Applications-blade.

    De toepassing 'Office 365 Mover' is een multitenant-app die niet hoeft te worden toegevoegd aan AAD met behulp van de sectie Galerietoepassingen onder Enterprise App Registration. Als u toegang wilt tot de Office 365 Mover-app, meldt u zich aan bij de app en vraagt u toestemming van de gebruiker voor de machtigingen. Zodra de gebruiker de toestemming heeft gegeven, wordt deze app automatisch toegevoegd aan de tenant met de e-mail-id die u hebt aangemeld.

    Nadat u zich hebt aanmelden bij de toepassing, kunt u de vermelding van deze toepassing vinden onder het blad Enterprise Applications in AAD. U moet naar die toepassing zoeken door de volledige naam te typen, dat wil zeggen ' Office 365 Mover' of gewoon 'office' te zoeken en de app moet worden weergegeven. Zie Office [365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)zegt dat deze al is geïnstalleerd, maar niet wordt weergegeven in de galerie Ondernemingstoepassing voor meer informatie.
8. Snelstart: In de lijst met toepassingen die uw [Azure Active Directory-tenant (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) gebruiken voor identiteitsbeheer, ziet u hoe u de toepassingen, ook wel apps genoemd, kunt bekijken die al zijn ingesteld voor het gebruik van uw Azure AD-tenant als identiteitsprovider (IdP).
9. [Als u veelvoorkomende problemen met het](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) toevoegen of verwijderen van een toepassing aan Azure Active Directory oplost, begrijpt u de veelvoorkomende problemen bij het bekijken van apps in Azure Active Directory.
