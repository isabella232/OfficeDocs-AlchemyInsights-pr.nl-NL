---
title: Safe bijlagen inschakelen voor SharePoint Online, OneDrive en Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332374"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Safe bijlagen inschakelen voor SharePoint Online, OneDrive en Microsoft Teams

1. Als u de referenties van uw globale beheerder of beveiligingsbeheerder gebruikt, opent u de Microsoft 365 Defender-portal bij en gaat u naar Beleidsregels & regels <https://security.microsoft.com>  \>  \> **Bedreigingsbeleid Safe Bijlagen** in  de sectie Beleid

   Als u rechtstreeks naar de pagina **Safe bijlagen** wilt gaan, gebruikt u <https://security.microsoft.com/safeattachmentv2> .

2. Klik op **Safe pagina Bijlagen** op Algemene **instellingen.**
3. Selecteer in het flyout dat wordt weergegeven de optie Microsoft Defender in Office 365 voor **SharePoint, OneDrive en Microsoft Teams** en selecteer **vervolgens Opslaan.**

    **Tip:** Ga als volgt te werk om de beveiliging van Safe bijlagen voor SharePoint, OneDrive en Microsoft Teams:
    - Als u wilt voorkomen dat gebruikers schadelijke bestanden downloaden, gebruikt u de waarde voor de `$true` parameter *DisallowInfectedFileDownload* op de cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** in SharePoint Online PowerShell. Zie Gebruik SharePoint Online PowerShell om te voorkomen dat gebruikers schadelijke bestanden downloaden voor [meer informatie.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Een waarschuwingsbeleid maken voor gedetecteerde bestanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Zie voor meer informatie Safe Bijlagen voor Office 365 voor [SharePoint, OneDrive en Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
