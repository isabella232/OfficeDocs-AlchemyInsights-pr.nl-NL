---
title: Problemen met gebruikersbeheer
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
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035530"
---
# <a name="user-management-issues"></a>Problemen met gebruikersbeheer

**Wat gebeurt er met huidige toegewezen gebruikers aan de toepassing als ik de eigenschap 'Gebruikerstoewijzing vereist' uit schakel (deze eigenschap instellen op Nee)?**

Het uitschakelen van **de vereiste gebruikerstoewijzing** heeft GEEN invloed op de momenteel toegewezen gebruikers. Als u deze eigenschap uit kunt uitschakelen, hebben alleen alle gebruikers toegang tot de toepassing. Alle vermelde gebruikers en gebruikers die aan groepen in de toepassing zijn toegewezen, blijven geldig.

- Zie - Azure AD-app beperken tot een set gebruikers [- Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Zie Gebruikerstoewijzing beheren voor een app in Azure Active Directory als u gebruikers en groepen wilt toewijzen aan ondernemingstoepassingen in Azure Active Directory [(Azure](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)AD), vanuit de Azure-portal of met PowerShell.
- Als u machtigingen voor het maken en beheren van toepassingen wilt delegeren, zie Machtigingen voor beheerders van [toepassingsbeheer gedelegeerden - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Specifieke enterprise-apps verbergen voor gebruikers:** gebruik de volgende stappen om alle Microsoft 365-apps te verbergen in het **MyApps-deelvenster.** De apps zijn nog steeds zichtbaar in de Office 365-portal.

 1. Meld u aan bij de Azure-portal als globale beheerder voor uw adreslijst. 
 2. Selecteer **Azure Active Directory**. 
 3. Selecteer **Gebruikers**. 
 4. Selecteer **Gebruikersinstellingen.** 
 5. Klik **onder Enterprise-toepassingen** op Beheren hoe eindgebruikers hun toepassingen **starten en weergeven.** 
 6. Voor **gebruikers kunnen alleen Office 365-apps in de Office 365-portal zien,** klikt u op **Ja.** 
 7. Klik op **Opslaan**. 
 8. Zie Een Enterprise-toepassing verbergen vanuit de gebruikerservaring [in Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Als u een SaaS-app (Software as a Service) aan veel organisaties aanbiedt, kunt u uw app zo configureren dat aanmeldingen worden geaccepteerd vanuit een Azure Active Directory -tenant (Azure AD). Deze configuratie wordt 'uw toepassing multi-tenant maken' genoemd. Gebruikers in een Azure AD-tenant kunnen zich aanmelden bij uw app nadat ze hebben ingestemd met het gebruik van hun account met uw app. Zie Apps maken die zich aanmelden [bij Azure AD-gebruikers - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Hoe kan een eindgebruiker toegang krijgen tot de toepassing nadat deze aan de toepassing is toegewezen?**

Elke app in enterprise application blade heeft een koppeling voor eindgebruikers om toegang te krijgen. Gebruikers kunnen de app ook op een eenvoudige manier openen via **de Myapps-portal.**

- **Wilt u weten welke toepassingen en typen toepassingen door gebruikers worden gebruikt?**

U kunt aanmeldingsrapporten voor de afgelopen 30 dagen downloaden **van portal.azure.com > Azure Active directory> Signins> downloadrapporten.**

- Lees hoe u [tenantbrede beheerders toestemming verleent voor een toepassing](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) en [Configureren hoe eindgebruikers toestemming geven voor toepassingen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Meer [inzicht in de manier waarop toestemming werkt](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) en Toestemming voor toepassingen [beheren.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


