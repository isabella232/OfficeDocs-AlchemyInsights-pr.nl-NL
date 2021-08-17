---
title: Ontbrekende e-mailberichten in quarantaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892042"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mailberichten in quarantaine

Beheerders kunnen [deze berichten bekijken,](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files) vrijgeven of verwijderen

Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> Quarantaine  \> **controleren.** Of als u rechtstreeks naar de pagina **Quarantaine wilt** gaan, gebruikt <https://security.microsoft.com/quarantine> u .  

Zie Berichten en bestanden in quarantaine beheren als [beheerder in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)voor meer informatie over de zoek-/filterwaarden die u kunt gebruiken.

De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine zijn:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)deze cmdlet is alleen voor berichten, niet voor bestanden van Safe Bijlagen voor SharePoint, OneDrive of Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
