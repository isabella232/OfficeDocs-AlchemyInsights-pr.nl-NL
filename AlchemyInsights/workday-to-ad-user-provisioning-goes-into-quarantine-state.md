---
title: Workday to AD User Provisioning gaat in quarantainetoestand
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036487"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning gaat in quarantainetoestand

**Workday to AD User Provisioning gaat in quarantainetoestand en er worden geen gebruikers gemaakt in AD**

De taak Workday to AD User Provisioning is in quarantainetoestand geplaatst en in de auditlogboeken worden exportfouten weergegeven met het foutbericht **Fout: OperationsError-SvcErr: Er is een bewerkingsfout opgetreden. Er is geen superieure verwijzing geconfigureerd voor de adreslijstservice. De adreslijstservice kan daarom geen verwijzingen naar objecten** buiten dit forest geven. Deze fout wordt meestal weergegeven als de active directorycontainerou niet correct is ingesteld of als er problemen zijn met de expressietoewijzing die wordt gebruikt voor **bovenliggendeDistinguishedName.**

Controleer de parameter Standaardou voor **nieuwe** gebruikers op typfouten. Controleer of de opgegevenou al bestaat in uw AD. Als u **parentDistinguishedName** gebruikt in de kenmerktoewijzing, moet u ervoor zorgen dat deze altijd wordt geëvalueerd naar een bekende container binnen het AD-domein. Controleer de gebeurtenis Exporteren in de auditlogboeken om de gegenereerde waarde te zien.

Zie Zelfstudie: Werkdag configureren voor automatische gebruikers inrichting voor meer informatie over het configureren van [werkdagen voor geautomatiseerde inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

