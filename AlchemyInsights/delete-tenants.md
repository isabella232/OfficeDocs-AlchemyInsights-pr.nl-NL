---
title: Tenant verwijderen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564486"
---
# <a name="delete-tenant"></a>Tenant verwijderen

Als u een Azure AD wilt verwijderen, moet u het volgende doen:
- U bent een globale beheerder voor de adreslijst.
- U bent niet aangemeld met een account dat de standaardmap bevat, zoals contoso.onmicrosoft.com, in het aangemelde account, zoals admin@contoso.onmicrosoft.com.
- Verwijder actieve toepassingen in de Directory voordat u ze verwijdert. Als u actieve toepassingen wilt verwijderen, gaat u naar app-registraties en verwijdert u de bestaande toepassingen.
- Er zijn geen actieve abonnementen voor Microsoft Online Services, zoals Microsoft Azure, Office 365 of Azure AD Premium die zijn gekoppeld aan de adreslijst. Verbind uw abonnementen of beëindig het annuleren van actieve abonnementen via Azure support en facturering. Meer informatie over het annuleren van Office 365-en Azure-abonnementen. Zie [een Azure-abonnement aan uw Azure AD-Tenant koppelen of toevoegen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)voor meer informatie over het koppelen of toevoegen van een bestaand abonnement aan een Tenant.
- Er is geen actieve licentie. Zie een [abonnement verwijderen om de licentie te verwijderen voor informatie over het](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)verwijderen van licenties.
- Er zijn geen andere actieve gebruikers in de adreslijst, naast uzelf als de globale beheerder, wanneer ze probeert Azure AD te verwijderen. Verwijder andere actieve gebruikers en afhankelijkheden van een aangepaste domeinnaam in de Tenant, moet u deze ook verwijderen, zoals gebruikers die zijn gemaakt met admin@contoso.com.

Voor meer gedetailleerde stappen voor:
- Verwijder ' Azure Active Directory ' of ' abonnement ' en Zie [Azure Active Directory verwijderen](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Als u toepassingen verwijdert uit de adreslijst, raadpleegt u [toepassingen verwijderen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
