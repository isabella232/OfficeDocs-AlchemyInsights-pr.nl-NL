---
title: Versleuteling met transportregels
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915087"
---
# <a name="encryption-with-transport-rules"></a>Versleuteling met transportregels

In het [Exchange-beheercentrum](https://go.microsoft.com/fwlink/p/?linkid=834822) (SBV) kunt u de mogelijkheden van Office Message Encryption (OME) in de regels voor de e-mailstroom gebruiken om berichtversleuteling te activeren. Kies de optie **Office 365-berichtversleuteling en -rechtenbeveiliging toepassen** op de voorwaarde van de transportregel.

- Zie voor meer informatie bij [Regel van e-mailstroom voor versleutelen definiëren](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- In PowerShell gebruikt u de cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) en stelt u de parameter *ApplyOME* in op $true.
