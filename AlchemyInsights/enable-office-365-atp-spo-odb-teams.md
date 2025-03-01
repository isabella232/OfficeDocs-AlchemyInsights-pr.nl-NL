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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332154"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defender inschakelen voor Office 365 voor SharePoint Online, OneDrive en Microsoft Teams

1. Ga naar https://protection.office.com en meld u aan.
2. Kies **Bedreigingsbeheerbeleid**  >    >  **Safe Bijlagen**.
3. Selecteer **Defender in Office 365 voor SharePoint, OneDrive en Microsoft Teams** en klik vervolgens op **Opslaan.**
4. (Aanbevolen) Als globale beheerder of SharePoint Online-beheerder kunt u de cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uitvoeren met de parameter **DisallowInfectedFileDownload** die is ingesteld op *waar.*
5. (Aanbevolen) [Waarschuwingen instellen voor](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) gedetecteerde bestanden.

**Opmerking:** Microsoft Defender voor Office 365 scant niet elk bestand in SharePoint Online, OneDrive of Microsoft Teams. Bestanden worden asynchroon gescand, via een proces dat gebruikmaakt van gebeurtenissen voor delen en gastactiviteit, samen met slimme heuristische en bedreigingssignalen om schadelijke bestanden te identificeren. Zie [Microsoft Defender voor Office 365 voor SharePoint, OneDrive en Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
