---
title: Schakel Office 365 ATP in voor SharePoint, OneDrive en Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543923"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defender inschakelen voor Office 365 voor SharePoint Online, OneDrive en Microsoft Teams

1. Ga naar https://protection.office.com en meld u aan.
2. Kies **Bedreigingsbeheerbeleid**  >    >  **Safe Bijlagen**.
3. Selecteer **Defender in Office 365 voor SharePoint, OneDrive en Microsoft Teams** en klik vervolgens op **Opslaan.**
4. (Aanbevolen) Als globale beheerder of SharePoint Online-beheerder kunt u de cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uitvoeren met de parameter **DisallowInfectedFileDownload** die is ingesteld op *true.*
5. (Aanbevolen) [Waarschuwingen instellen voor](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) gedetecteerde bestanden.

> [!NOTE]
> Microsoft Defender voor Office 365 scant niet elk bestand in SharePoint Online, OneDrive of Microsoft Teams. Bestanden worden asynchroon gescand, via een proces dat gebruikmaakt van gebeurtenissen voor delen en gastactiviteit, samen met slimme heuristische en bedreigingssignalen om schadelijke bestanden te identificeren. Zie [Microsoft Defender voor Office 365 voor SharePoint, OneDrive en Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)