---
title: Werkdag tot ad-gebruiker inrichting gaat in quarantainetoestand
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481355"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Werkdag tot ad-gebruiker inrichting gaat in quarantainetoestand

**Werkdag tot en met AD User Provisioning gaat in quarantaine, en er worden geen gebruikers gemaakt in AD**

De taak Werkdag naar AD-gebruiker provisioning is in quarantaine geplaatst en in de auditlogboeken worden exportfoutgebeurtenissen weergegeven met het foutbericht **Fout: OperationsError-SvcErr: Er is een bewerkingsfout opgetreden. Er is geen betere verwijzing geconfigureerd voor de adreslijstservice. De adreslijstservice kan daarom geen verwijzingen geven naar objecten buiten deze forest.** Deze fout wordt meestal weergegeven als de OU van de Active Directory-container niet juist is ingesteld of als er problemen zijn met de expressietoewijzing die wordt gebruikt voor **bovenliggendeDistinguishedName.**

Controleer de standaard-OU **voor de** parameter Nieuwe gebruikers op typfouten. Controleer of de opgegeven OU al bestaat in uw AD. Als u **parentDistinguishedName** gebruikt in de kenmerktoewijzing, controleert u of het altijd een bekende container binnen het AD-domein evalueert. Controleer de gebeurtenis Exporteren in de auditlogboeken om de gegenereerde waarde te zien.

Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

