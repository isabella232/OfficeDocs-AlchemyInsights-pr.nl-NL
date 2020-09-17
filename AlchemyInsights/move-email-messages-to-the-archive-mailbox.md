---
title: E-mailberichten verplaatsen naar het archief Postvak
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799775"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail verplaatsen naar het archief Postvak

Als u wilt dat wij geautomatiseerde controles uitvoeren voor de instellingen die hieronder worden vermeld, selecteert u de knop terug <--boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het verplaatsen van e-mail naar het archief postvak.

1. Ga na of een **Archief postvak** is ingeschakeld. Als dat niet zo is, voert u de stappen in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) uit om het archief postvak in te schakelen.

2. Als u berichten automatisch wilt archiveren in het archief postvak, moet u een Bewaar label met de actie **verplaatsen naar archief** instellen om **automatisch toe te passen op een volledig postvak (standaard)**. Voer de volgende stappen uit om de tag te maken: [standaardlabel voor archiveren](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Vervolgens voegt u de tag **Archief** toe aan uw bewaarbeleid. Kies in het Exchange-Beheercentrum de optie **bewaarbeleid** > de **tag verplaatsen naar archief** toevoegen aan het beleid > **Opslaan**.

4. [Wijs het bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nu toe aan het postvak van de specifieke gebruiker. Het beleid wordt toegepast op zowel het **primaire** als het **Archief** postvak.

Mogelijk moet u de Managed folder Assistant (MFA) gebruiken om de nieuwe instellingen toe te passen op het postvak van de gebruiker. Voer de volgende opdracht uit terwijl [u verbonden bent met Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde map voor een specifiek postvak te starten:
  
Start-ManagedFolderAssistant id <name of the mailbox>

Zie voor meer informatie over het instellen van een archiefbeleid [een archief-en verwijderingsbeleid instellen voor postvakken](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  