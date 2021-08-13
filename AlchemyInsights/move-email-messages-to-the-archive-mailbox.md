---
title: E-mailberichten verplaatsen naar het archiefpostvak
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974952"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail verplaatsen naar het archiefpostvak

Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de knop Terug <-- boven aan deze pagina en voert u vervolgens het e-mailadres in van de gebruiker die problemen heeft met het verplaatsen van e-mail naar het archiefpostvak.

1. Controleer of een **archiefpostvak** is ingeschakeld. Als dit niet het beste is, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) om het archiefpostvak in te stellen.

2. Als u berichten automatisch naar het archiefpostvak  wilt archiveren, moet een bewaarlabel met de actie Verplaatsen naar archief worden ingesteld op automatisch toegepast op het hele **postvak (standaardlabel).** Gebruik de stappen hier om de tag: [Standaardlabel archiveren te maken.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Voeg vervolgens de tag **Archiveren** toe aan uw bewaarbeleid. Kies in Exchange beheercentrum Bewaarbeleid om > **tag** Verplaatsen naar archief toe te voegen aan het beleid > **Opslaan.** 

4. Wijs [nu het bewaarbeleid toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker. Hetzelfde beleid wordt toegepast op  zowel het primaire postvak als het **archiefpostvak.**

Mogelijk moet u de MFA (Managed Folder Assistant) dwingen om de nieuwe instellingen uit te voeren en toe te passen op het postvak van de gebruiker. Voer de volgende opdracht uit [terwijl u verbonden bent met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde mapassistent voor een specifiek postvak te starten:
  
Start-ManagedFolderAssistant -Identiteit <name of the mailbox>

Zie Een archief- en verwijderingsbeleid instellen voor postvakken voor meer informatie over het instellen van een [archiefbeleid.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  