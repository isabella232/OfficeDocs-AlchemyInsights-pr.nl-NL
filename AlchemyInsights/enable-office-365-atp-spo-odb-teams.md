---
title: Office 365 ATP inschakelen voor SharePoint en OneDrive Microsoft-Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403028"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365 bedreiging voor geavanceerde beveiliging voor SharePoint Online, OneDrive en Microsoft-Teams

1. Ga naar https://protection.office.com en log in.
2. Kies **Threat management** > **beleid** > **Veilige bijlagen**.
3. Selecteer **ATP voor SharePoint, OneDrive, en Microsoft-Teams inschakelen**en klik vervolgens op **Opslaan**.
4. (Aanbevolen) Als een globale beheerder of beheerder van een SharePoint Online, de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) worden uitgevoerd met de parameter **DisallowInfectedFileDownload** is ingesteld op *true*.
5. (Aanbevolen) [Waarschuwingen instellen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor bestanden gevonden.

> [!NOTE]
> ATP wordt nom scan van elk bestand in SharePoint Online, OneDrive of Microsoft-Teams. Bestanden gescand asynchroon, via een proces dat gebruikmaakt van delen en Gast activiteitsgebeurtenissen en intelligente heuristiek en bedreiging signalen om schadelijke bestanden te identificeren. Zie [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).