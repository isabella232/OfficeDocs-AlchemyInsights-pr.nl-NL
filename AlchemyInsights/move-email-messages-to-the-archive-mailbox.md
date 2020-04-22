---
title: E-mailberichten verplaatsen naar het postvak Archief
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713641"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail verplaatsen naar het archiefpostvak

1. Controleer of een **archiefpostvak** is ingeschakeld. Als dit niet het zo is, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) om het archiefpostvak in te schakelen.

2. Als u berichten automatisch wilt archiveren in het archiefpostvak, moet een bewaartag met de actie **Verplaatsen naar archief** automatisch worden toegepast op de volledige tag van het postvak **(standaard).** Gebruik de stappen hier om de tag te maken: [Archive default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Voeg vervolgens de **archieftag** toe aan uw bewaarbeleid. Kies in het Exchange-beheercentrum **Bewaarbeleid** > de **tag Verplaatsen naar archief** toevoegen aan het beleid > **Opslaan**.

4. [Wijs nu het bewaarbeleid toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker. Hetzelfde beleid wordt toegepast op zowel het **postvak Primair** als **archief.**

Het kan nodig zijn om de Managed Folder Assistant (MFA) uit te voeren en de nieuwe instellingen toe te passen op het postvak van de gebruiker. Voer de volgende opdracht uit terwijl [u bent verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde mapassistent voor een specifiek postvak te starten:
  
Start-ManagedFolderAssistant -Identiteit<name of the mailbox>

Zie [Een archief- en verwijderingsbeleid instellen voor postvakken voor](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)meer informatie over het instellen van een archiefbeleid.
  