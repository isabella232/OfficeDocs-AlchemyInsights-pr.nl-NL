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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506913"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Geavanceerde bedreigingsbeveiliging van Office 365 inschakelen voor SharePoint Online, OneDrive en Microsoft Teams

1. Ga naar https://protection.office.com en meld je aan.
2. Kies **veilige**bijlagen voor  >  **bedreigingsbeheerbeleid**  >  **Safe Attachments**.
3. Selecteer **ATP inschakelen voor SharePoint, OneDrive en Microsoft Teams**en klik op **Opslaan**.
4. (Aanbevolen) Voer als globale beheerder of SharePoint Online-beheerder de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uit met de parameter **DisallowInfectedFileDownload** ingesteld op *true*.
5. (Aanbevolen) [Waarschuwingen instellen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor gedetecteerde bestanden.

> [!NOTE]
> ATP scant elk bestand in SharePoint Online, OneDrive of Microsoft Teams. Bestanden worden asynchroon gescand, via een proces dat het delen en gastactiviteitsgebeurtenissen gebruikt, samen met slimme heuristiek en bedreigingssignalen om schadelijke bestanden te identificeren. Zie [ATP voor SharePoint, OneDrive en Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).