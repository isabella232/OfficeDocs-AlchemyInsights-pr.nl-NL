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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329657"
---
# <a name="missing-emails-in-quarantine"></a>Ontbrekende e-mailberichten in quarantaine

Beheerders kunnen [deze berichten bekijken,](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files) vrijgeven of verwijderen

Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com> Quarantaine  \> **controleren.** Of als u rechtstreeks naar de pagina **Quarantaine wilt** gaan, gebruikt <https://security.microsoft.com/quarantine> u .  

Zie Berichten en bestanden in quarantaine beheren als [beheerder in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)voor meer informatie over de zoek-/filterwaarden die u kunt gebruiken.

De cmdlets die u gebruikt voor het weergeven en beheren van berichten en bestanden in quarantaine zijn:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Deze cmdlet is alleen voor berichten, niet voor bestanden uit Safe Bijlagen voor SharePoint, OneDrive of Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
