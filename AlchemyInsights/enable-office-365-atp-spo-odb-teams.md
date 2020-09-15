---
title: Office 365 ATP inschakelen voor SharePoint, OneDrive en Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709902"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365 Advanced Threat Protection inschakelen voor SharePoint Online, OneDrive en Microsoft teams

1. Ga naar https://protection.office.com en meld u aan.
2. Selecteer **Threat management**  >  **Policy**  >  **veilige bijlagen**voor het beleid voor bedreigings beheer.
3. Selecteer **ATP voor SharePoint, OneDrive en Microsoft teams inschakelen**en klik op **Opslaan**.
4. Beter Als globale beheerder of een SharePoint Online-beheerder voert u de cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uit waarbij de **DisallowInfectedFileDownload** -parameter is ingesteld op *waar*.
5. Beter [Waarschuwingen instellen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) voor gedetecteerde bestanden.

> [!NOTE]
> Met ATP kan ik elk afzonderlijk bestand in SharePoint Online, OneDrive of Microsoft teams scannen. Bestanden worden asynchroon gescand, via een proces waarbij gebeurtenissen voordelen en gebeurtenissen met gebeurtenissen van een gast worden gebruikt, samen met slimme heuristische en bedreigings signalen om kwaadaardige bestanden te identificeren. Bekijk [ATP voor SharePoint, OneDrive en Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).