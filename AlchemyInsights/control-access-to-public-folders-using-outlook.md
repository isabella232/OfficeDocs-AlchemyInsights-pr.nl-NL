---
title: Toegang tot openbare mappen beheren in Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032553"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Toegang tot openbare mappen beheren in Outlook

Bepalen welke gebruikers toegang hebben tot openbare mappen in Outlook:

1. Gebruik `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: gebruikers toegang geven tot openbare mappen in Outlook  
$false: gebruikers toegang weigeren tot openbare mappen in Outlook. Dit is de standaardwaarde.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Opmerking: met deze procedure kunt u alleen verbindingen met de bureaubladversie van Outlook voor Windows-clients beheren. Gebruikers hebben nog steeds toegang tot openbare mappen met behulp van OWA of Outlook voor Mac.

Zie [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) (Beheerde verbindingen met openbare mappen in Outlook) voor meer informatie.
