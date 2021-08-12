---
title: 'Beheerders toevoegen en beheren : aanbevolen stappen'
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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963782"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Beheerders toevoegen en beheren : aanbevolen stappen

Op basis van uw probleembeschrijving hebben we een oplossing voor u gevonden. De meeste klanten hebben hun probleem zelf kunnen oplossen na het volgen van onze documentatie.

**De abonnementsbeheerder of medebeheerder bewerken**

- De accountbeheerder kan beide rollen bewerken, terwijl de abonnementsbeheerder alleen cobeheerders in de [Azure-portal kan wijzigen.](https://ms.portal.azure.com/#home)
- [Beheerders van Azure-abonnementen toevoegen of wijzigen](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**De abonnementsbeheerder of -Co-Administrator voor interne abonnementen (AIRS) bijwerken**

De servicebeheerder of de medebeheerder kan deze actie zelf uitvoeren met de volgende stappen:

1. Meld u aan bij [de Azure-portal](https://ms.portal.azure.com/#home) en klik op **Kostenbeheer + Facturering** in het linkerblad.
2. Klik op het regelitem met uw abonnement. Hiermee wordt het overzicht voor uw abonnement geopend.
3. Klik op **het blad** Abonnement op **Eigenschappen.** 
4. Klik op **de knop Servicebeheerder.**
5. Voer de e-mail in van de gebruiker die u wilt instellen als servicebeheerder en klik op **OK.**

**Medebeheerder toevoegen/wijzigen/verwijderen**

1. Meld u aan bij [de Azure-portal](https://ms.portal.azure.com/#home) als servicebeheerder.
2. Open [Abonnementen en](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) selecteer een abonnement. (Cobeheerders kunnen alleen worden toegewezen binnen het abonnementsbereik.)
3. Ga naar De klassieke beheerders van Access Control **(IAM)** Voeg medebeheerder toevoegen toe om het deelvenster Medebeheerder toevoegen te openen (Als de optie Medebeheerder toevoegen is uitgeschakeld, geeft dit aan dat u geen machtigingen  >    >    >   hebt). 
4. Selecteer de gebruiker die u wilt toevoegen en klik op **Toevoegen.**

**Meer informatie:**
- [Een medebeheerder toevoegen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Een medebeheerder verwijderen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [De servicebeheerder wijzigen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [De accountbeheerder weergeven](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Toegang beheren met RBAC en Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Gebruikers toevoegen/verwijderen met Azure Active Directory (AD)**

U kunt nieuwe gebruikers toevoegen of bestaande gebruikers verwijderen uit uw Azure Active Directory (Azure AD) organisatie:

1. Als u een nieuwe gebruiker wilt toevoegen, meld u zich aan bij de [Azure-portal](https://ms.portal.azure.com/#home) als gebruiker-beheerder voor de organisatie.
2. Selecteer **Azure Active Directory**, selecteer **Gebruikers** en klik vervolgens op **Nieuwe gebruiker.**
3. Vul op **de** pagina Gebruiker de vereiste informatie in. Klik op **Maken**. De gebruiker wordt gemaakt en toegevoegd aan uw Azure AD-tenant.

**Meer informatie:**

- [Een nieuwe gebruiker toevoegen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Een gebruiker verwijderen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Profielgegevens van een gebruiker toevoegen of bijwerken met Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Aanbevolen documenten**

- [Wat is op rollen gebaseerd toegangsbeheer (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [De verschillende rollen in Azure begrijpen](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Machtigingen voor beheerdersrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Zelfstudie: Toegang verlenen voor een gebruiker met RBAC en de Azure-portal](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Problemen met RBAC oplossen in Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Uw resources organiseren met Azure-beheergroepen](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kopie van Azure-factuur aanvragen via e-mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Een creditcard of betaalkaart toevoegen, bijwerken of verwijderen uit Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Manage (Reactivate/Cancel/Switch) subscription](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



