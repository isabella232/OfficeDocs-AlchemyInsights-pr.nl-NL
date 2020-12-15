---
title: Adminstrators-aanbevolen stappen toevoegen en beheren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677255"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Adminstrators-aanbevolen stappen toevoegen en beheren

**De beheerder of mede beheerder van het abonnement bewerken**

- De account beheerder kan beide rollen bewerken, terwijl de abonnement beheerder alleen co-beheerders in de [Azure-Portal](https://ms.portal.azure.com/#home)kan wijzigen.
- [Azure-abonnements beheerders toevoegen of wijzigen](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**De abonnements beheerder of het Co-Administrator voor interne (onvoeren) abonnementen bijwerken**

De service beheerder of de co-beheerder kan de volgende stappen uitvoeren om deze actie uit te voeren:

1. Meld u aan bij de [Azure-Portal](https://ms.portal.azure.com/#home) en klik op **Cost Management + facturering** in het linker blad.
2. Klik op het regelitem met uw abonnement. Hiermee opent u het overzicht voor uw abonnement.
3. Klik in de Blade **abonnement** op **Eigenschappen**. 
4. Klik op de knop **service beheerder** .
5. Voer het e-mailadres in van de gebruiker die u als service beheerder wilt instellen en klik op **OK**.

**Co-beheerder toevoegen/wijzigen/verwijderen**

1. Meld u bij de [Azure-Portal](https://ms.portal.azure.com/#home) aan als een service beheerder.
2. Open [abonnementen](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) en selecteer een abonnement. (Coadminstrators kan alleen worden toegewezen aan het abonnements bereik.)
3. Ga naar **toegangsbeheer (IAM)**  >  **klassieke beheerders**  >  **toevoegen**  >  **co-beheerder** toevoegen om het deelvenster **co-beheerder toevoegen** te openen (als de optie co-beheerder toevoegen is uitgeschakeld, wordt aangegeven dat u geen machtigingen hebt).
4. Selecteer de gebruiker die u wilt toevoegen en klik op **toevoegen**.

**Meer informatie:**
- [Een co-beheerder toevoegen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Een co-beheerder verwijderen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [De service beheerder wijzigen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [De account beheerder weergeven](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Toegang beheren met RBAC en Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Gebruikers toevoegen/verwijderen via Azure Active Directory (AD)**

U kunt nieuwe gebruikers toevoegen of bestaande gebruikers verwijderen uit uw Azure Active Directory-organisatie (Azure AD):

1. Als u een nieuwe gebruiker wilt toevoegen, meldt u zich aan bij de [Azure-Portal](https://ms.portal.azure.com/#home) als gebruiker van de beheerder van de organisatie.
2. Selecteer **Azure Active Directory**, selecteer **gebruikers** en klik vervolgens op **nieuwe gebruiker**.
3. Vul de vereiste gegevens in op de pagina van de **gebruiker** . Klik op **Maken**. De gebruiker wordt gemaakt en toegevoegd aan uw Azure AD-Tenant.

Meer **informatie**:

- [Een nieuwe gebruiker toevoegen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Een gebruiker verwijderen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Gebruikersprofielgegevens toevoegen of bijwerken met Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Aanbevolen documenten**

- [Wat is toegangsbeheer op basis van rollen?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Meer informatie over de verschillende rollen in azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Machtigingen voor beheerdersrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Zelfstudie: toegang verlenen aan een gebruiker met behulp van RBAC en de Azure-Portal](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Problemen met RBAC in azure oplossen](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Uw resources organiseren met Azure-beheergroepen](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Het aanvragen van een kopie van Azure factuur via e-mail aanvragen](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Een creditcard of betaalkaart toevoegen, bijwerken of verwijderen uit Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Het abonnement beheren (opnieuw activeren/Annuleren/activeren)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



