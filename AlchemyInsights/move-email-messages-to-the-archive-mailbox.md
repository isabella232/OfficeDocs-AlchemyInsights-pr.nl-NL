---
title: E-mailberichten verplaatsen naar het postvak Archiveren
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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522766"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail verplaatsen naar het archiefpostvak

Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de terugknop <- boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het verplaatsen van e-mail naar zijn archiefpostvak.

1. Controleer of een **archiefpostvak** is ingeschakeld. Als dit niet het zo is, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) om het archiefpostvak in te schakelen.

2. Als u berichten automatisch wilt archiveren naar het archiefpostvak, moet een bewaartag met de actie **Verplaatsen naar archief** worden ingesteld om automatisch te worden toegepast op de tag hele **postvak (standaard).** Gebruik de stappen hier om de tag te maken: [Archiefstandaardtag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Voeg vervolgens de **archieftag** toe aan uw bewaarbeleid. Kies in het Exchange-beheercentrum **Bewaarbeleid** > voegt u de **tag Verplaatsen naar archief** toe aan het beleid > **Opslaan**.

4. [Wijs nu het bewaarbeleid toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker. Hetzelfde beleid wordt toegepast op zowel het **postvak Primair** als **Archief.**

Het kan nodig zijn om de Managed Folder Assistant (MFA) te dwingen de nieuwe instellingen uit te voeren en toe te passen op het postvak van de gebruiker. Voer de volgende opdracht uit terwijl [u is verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de assistent beheerde mappen voor een specifiek postvak te starten:
  
Start-ManagedFolderAssistant -Identiteit<name of the mailbox>

Zie [Een archief- en verwijderingsbeleid voor postvakken instellen voor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)meer informatie over het instellen van een archiefbeleid.
  