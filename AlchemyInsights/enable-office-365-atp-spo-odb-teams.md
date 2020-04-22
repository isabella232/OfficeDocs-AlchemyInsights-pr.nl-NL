---
title: Office 365 ATP inschakelen voor SharePoint, OneDrive en Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703421"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365 geavanceerde bescherming tegen bedreigingen inschakelen voor SharePoint Online, OneDrive en Microsoft Teams

1. Ga https://protection.office.com naar en meld je aan.
2. Kies Veilige bijlagen **voor** > beleid voor**bedreigingsbeheer****Policy** > .
3. Selecteer **ATP inschakelen voor SharePoint, OneDrive en Microsoft Teams**en klik op **Opslaan**.
4. (Aanbevolen) Voer als globale beheerder of SharePoint Online-beheerder de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uit met de parameter **DisallowInfectedFileDownload** ingesteld op *true.*
5. (Aanbevolen) [Waarschuwingen instellen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor gedetecteerde bestanden.

> [!NOTE]
> ATP scant elk bestand in SharePoint Online, OneDrive of Microsoft Teams. Bestanden worden asynchroon gescand, via een proces dat gebruik maakt van gebeurtenissen op het gebied van delen en gastactiviteiten, samen met slimme heuristiek en bedreigingssignalen om schadelijke bestanden te identificeren. Zie [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).