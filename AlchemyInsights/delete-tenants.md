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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993888"
---
# <a name="delete-tenant"></a>Tenant verwijderen

Als u een Azure AD wilt verwijderen, controleert u het volgende:
- U bent een globale beheerder in de adreslijst.
- U bent NIET aangemeld met een account met de standaardmap, zoals contoso.onmicrosoft.com in het aangemelde account, zoals admin@contoso.onmicrosoft.com.
- Verwijder alle actieve toepassingen in de adreslijst voordat u deze verwijdert. Als u actieve toepassingen wilt verwijderen, gaat u naar App-registraties en verwijdert u de bestaande toepassingen.
- Er zijn geen actieve abonnementen voor Microsoft Online Services, zoals Microsoft Azure, Office 365 of Azure AD Premium gekoppeld aan de adreslijst. Overdraag uw abonnementen of bespoedigen de opzegging van actieve abonnementen via Azure Support en Facturering. Meer informatie over Het annuleren van Office 365 en Azure-abonnementen. Zie Een Azure-abonnement koppelen of toevoegen aan uw [Azure AD-tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)voor informatie over het koppelen of toevoegen van een bestaand abonnement aan een tenant.
- Er is geen actieve licentie. Zie Abonnement verwijderen om licentie te verwijderen als u licenties [wilt verwijderen.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Er zijn geen andere actieve gebruikers in de directory naast uzelf als globale beheerder wanneer u probeert de Azure AD te verwijderen. Verwijder andere actieve gebruikers en eventuele afhankelijkheden van een aangepaste domeinnaam in de tenant moeten ook worden verwijderd, zoals gebruikers die zijn gemaakt met admin@contoso.com.

Voor meer informatie over hoe u:
- Verwijder 'Azure Active Directory' of 'abonnement', zie [Verwijderen Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Als u toepassingen in de adreslijst verwijdert, zie [Toepassingen verwijderen.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
