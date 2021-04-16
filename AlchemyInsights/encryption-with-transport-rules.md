---
title: Versleuteling met transportregels
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813863"
---
# <a name="encryption-with-transport-rules"></a>Versleuteling met transportregels

In het [Exchange-beheercentrum](https://go.microsoft.com/fwlink/p/?linkid=834822) (SBV) kunt u de mogelijkheden van Office Message Encryption (OME) in de regels voor de e-mailstroom gebruiken om berichtversleuteling te activeren. Kies de optie **Office 365-berichtversleuteling en -rechtenbeveiliging toepassen** op de voorwaarde van de transportregel.

- Zie voor meer informatie bij [Regel van e-mailstroom voor versleutelen definiëren](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- In PowerShell gebruikt u de cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) en stelt u de parameter *ApplyOME* in op $true.
