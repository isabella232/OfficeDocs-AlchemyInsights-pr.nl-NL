---
title: Een auditlogboekrol toewijzen in het Office 365-beveiligings- & compliancecentrum
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744601"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Een auditlogboekrol toewijzen in het Office 365-beveiligings- & compliancecentrum

Als u in het Office 365-auditlogboek wilt zoeken, moet een beheerder de rol **Alleen-weergeven** of de rol **Auditlogboeken** in Exchange Online krijgen toegewezen. Deze rollen zijn standaard toegewezen aan de rollengroepen Compliancebeheer en Organisatiebeheer. Globale beheerders in Office 365 en Microsoft 365 worden automatisch toegevoegd als leden van de rollengroep Organisatiebeheer.

Als u een gebruiker wilt laten zoeken met het minimumniveau van bevoegdheden, maakt u een aangepaste rollengroep in Exchange Online, voegt u de rol **Alleen-weergeven** auditlogboeken of de rol **Auditlogboeken** toe en voegt u de gebruiker toe als lid van de nieuwe rollengroep.

Zie Rollengroepen beheren [in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) en Het auditlogboek doorzoeken in het beveiligings- & [compliancecentrum voor meer informatie.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)