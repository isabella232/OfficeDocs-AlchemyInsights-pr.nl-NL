---
title: E-mail berichten verplaatsen naar de archiefmap Postvak
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822157"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail verplaatsen naar de archiefmap Postvak

1. Bevestig dat een **postbus archiveren** is ingeschakeld. Als u dit niet doet, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) om het postvak archiveren in te schakelen.

2. Als u berichten automatisch wilt archiveren in het archief postvak, moet een inhoudings label met de actie **verplaatsen naar archiveren** worden ingesteld op **automatisch toepassen op volledige postbus (standaard)-tag**. Gebruik de stappen hier voor het maken van de tag: [standaard-tag archiveren](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Voeg vervolgens de **Archive** -tag toe aan uw bewaarbeleid. Kies in het Beheercentrum van Exchange **bewaarbeleid** > de **tag verplaatsen naar archief** toevoegen aan het beleid > **Opslaan**.

4. [Wijs het bewaarbeleid nu toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker. Hetzelfde beleid wordt toegepast op de **primaire** en de **archiefmap** postvak.

Het kan nodig zijn de beheerde mapassistent (MFA) uit te voeren en de nieuwe instellingen toe te passen op het postvak van de gebruiker. Voer de volgende opdracht uit terwijl u verbonden bent met [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde mapassistent voor een specifiek postvak te starten:
  
Start-ManagedFolderAssistant-Identity<name of the mailbox>

Zie [een beleid voor archiveren en verwijderen instellen voor postvakken](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)voor meer informatie over het instellen van een archief beleid.
  