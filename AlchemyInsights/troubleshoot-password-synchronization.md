---
title: Problemen met Wachtwoordsynchronisatie oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664921"
---
# <a name="troubleshoot-password-synchronization"></a>Problemen met Wachtwoordsynchronisatie oplossen

Voor het oplossen van problemen met Wachtwoordsynchronisatie, begint u met deze AAD-verbinding voor het oplossen van problemen om te bepalen waarom wachtwoorden niet worden gesynchroniseerd. Als u wilt beginnen, gaat u naar [directe synchronisatie beheren](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Open een nieuwe Windows PowerShell-sessie op de Azure AD Connect-server en selecteer vervolgens de optie **Run as-beheerder** .

2. Voer Set-ExecutionPolicy RemoteSigned of Set-ExecutionPolicy niet beperkt.

3. Start de wizard Azure AD Connect.

4. Ga naar de pagina aanvullende taken > **volgende problemen oplossen**  >  **Next**.

5. Selecteer **Start** om het menu probleem met PowerShell te openen.

6. Selecteer **problemen met Wachtwoordsynchronisatie oplossen**.

    Het probleem is meestal dat een wachtwoord niet wordt gesynchroniseerd voor een specifiek gebruikersaccount.

    **Info** Wachtwoordsynchronisatie mislukt als de laatste geslaagde Wachtwoordsynchronisatie enige tijd geleden was.

Zie [problemen met wachtwoord hash oplossen met Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synchronisatie voor meer hulp bij het oplossen van Wachtwoordsynchronisatie.