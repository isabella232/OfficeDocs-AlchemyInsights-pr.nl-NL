---
title: Toepassingen verwijderen of herstellen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014796"
---
# <a name="delete-or-restore-applications"></a>Toepassingen verwijderen of herstellen

**Een toepassing verwijderen uit een Azure AD-Tenant**:

1. Selecteer **Enterprise toepassingen** in de **Azure AD-Portal**. Zoek en selecteer de toepassing die u wilt verwijderen.
2. Selecteer in de sectie **beheren** van het linkerdeelvenster **Eigenschappen**.
3. Selecteer **verwijderen** en selecteer vervolgens **Ja** om te bevestigen dat u de app wilt verwijderen uit uw Azure AD-Tenant.

Zie voor meer informatie over het verwijderen van een app [: een toepassing verwijderen uit uw Azure Active Directory (Azure AD)-Tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

In PowerShell worden toepassings proxy configuraties uit een bepaalde toepassing in azure Active Directory verwijderd uit PowerShell en [kan de toepassing](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) helemaal verwijderen, indien opgegeven.

U kunt **een verwijderde toepassing herstellen** met PowerShell. Wanneer de toepassing die u wilt herstellen is vastgesteld, kunt u deze herstellen met [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
