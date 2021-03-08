---
title: Een rol in het auditlogboek toewijzen in het Office 365-& compliancecentrum
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523974"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="cd26f-102">Een rol in het auditlogboek toewijzen in het Office 365-& compliancecentrum</span><span class="sxs-lookup"><span data-stu-id="cd26f-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="cd26f-103">Als u in het Office 365-auditlogboek wilt zoeken, moet aan een beheerder de rol **Alleen-weergeven** of de rol **Auditlogboeken** in Exchange Online worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="cd26f-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="cd26f-104">Deze rollen zijn standaard toegewezen aan de rollengroepen Compliancebeheer en Organisatiebeheer.</span><span class="sxs-lookup"><span data-stu-id="cd26f-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="cd26f-105">Globale beheerders in Office 365 en Microsoft 365 worden automatisch toegevoegd als leden van de rollengroep Organisatiebeheer.</span><span class="sxs-lookup"><span data-stu-id="cd26f-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="cd26f-106">Als u een gebruiker in staat wilt stellen te zoeken met het minimumniveau van machtigingen, maakt u een aangepaste rollengroep in Exchange Online, voegt u de rol Auditlogboeken **alleen-weergeven** of de rol **Auditlogboeken** toe en voegt u de gebruiker toe als lid van de nieuwe rollengroep.</span><span class="sxs-lookup"><span data-stu-id="cd26f-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="cd26f-107">Zie Rollengroepen beheren [in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) en zoeken in het auditlogboek in het & compliancecentrum voor meer [informatie.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="cd26f-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>