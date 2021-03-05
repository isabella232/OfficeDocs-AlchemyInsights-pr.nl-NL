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
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="85870-102">Werkdag tot ad-gebruiker inrichting gaat in quarantainetoestand</span><span class="sxs-lookup"><span data-stu-id="85870-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="85870-103">**Werkdag tot en met AD User Provisioning gaat in quarantaine, en er worden geen gebruikers gemaakt in AD**</span><span class="sxs-lookup"><span data-stu-id="85870-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="85870-104">De taak Werkdag naar AD-gebruiker provisioning is in quarantaine geplaatst en in de auditlogboeken worden exportfoutgebeurtenissen weergegeven met het foutbericht **Fout: OperationsError-SvcErr: Er is een bewerkingsfout opgetreden. Er is geen betere verwijzing geconfigureerd voor de adreslijstservice. De adreslijstservice kan daarom geen verwijzingen geven naar objecten buiten deze forest.**</span><span class="sxs-lookup"><span data-stu-id="85870-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="85870-105">Deze fout wordt meestal weergegeven als de OU van de Active Directory-container niet juist is ingesteld of als er problemen zijn met de expressietoewijzing die wordt gebruikt voor **bovenliggendeDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="85870-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="85870-106">Controleer de standaard-OU **voor de** parameter Nieuwe gebruikers op typfouten.</span><span class="sxs-lookup"><span data-stu-id="85870-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="85870-107">Controleer of de opgegeven OU al bestaat in uw AD.</span><span class="sxs-lookup"><span data-stu-id="85870-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="85870-108">Als u **parentDistinguishedName** gebruikt in de kenmerktoewijzing, controleert u of het altijd een bekende container binnen het AD-domein evalueert.</span><span class="sxs-lookup"><span data-stu-id="85870-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="85870-109">Controleer de gebeurtenis Exporteren in de auditlogboeken om de gegenereerde waarde te zien.</span><span class="sxs-lookup"><span data-stu-id="85870-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="85870-110">Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="85870-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

