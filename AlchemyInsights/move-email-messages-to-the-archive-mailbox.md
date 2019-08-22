---
title: E-mailberichten naar de archiefmap Postvak verplaatsen
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
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36548998"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail naar de archiefmap Postvak verplaatsen

1. Bevestigen dat een **postbus archiveren** is ingeschakeld. Als dat niet het geval is, volg de stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) de postbus archiveren inschakelen.

2. U archiveert berichten automatisch naar de archiefmap Postvak in, moet een label bewaren met de actie **verplaatsen om te archiveren** worden ingesteld op **automatisch naar het postvak in zijn geheel (standaard)-code wordt toegepast**. De stappen hier gebruik maken van de code: [tag archief standaard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Voeg vervolgens de tag **archief** aan het bewaarbeleid. Kies in het beheercentrum van Exchange **Bewaarbeleid** > de **verplaatsen naar archief tag** toevoegen aan het beleid > **Opslaan**.

4. Nu [het bewaarbeleid toewijzen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan de specifieke postbus van gebruiker. Hetzelfde beleid zullen worden toegepast op zowel de **primaire** als de **archiefmap** postvak.

Deze zijn nodig om de beheerde map-assistent (MVR gesloten) uit te voeren en de nieuwe instellingen toepassen op het postvak van de gebruiker. Voer de volgende opdracht [verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tijdens het starten van de beheerde map-assistent van een bepaalde postbus:
  
Start ManagedFolderAssistant-id<name of the mailbox>

Zie voor meer informatie over het instellen van een archiveringsbeleid [instellen van een beleid voor archiveren en verwijderen van postvakken](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  