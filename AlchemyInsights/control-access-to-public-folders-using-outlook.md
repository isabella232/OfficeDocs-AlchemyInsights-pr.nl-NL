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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816735"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Toegang tot openbare mappen beheren in Outlook

Bepalen welke gebruikers toegang hebben tot openbare mappen in Outlook:

1. Gebruik `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: gebruikers toegang geven tot openbare mappen in Outlook  
$false: gebruikers toegang weigeren tot openbare mappen in Outlook. Dit is de standaardwaarde.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Opmerking: met deze procedure kunt u alleen verbindingen met de bureaubladversie van Outlook voor Windows-clients beheren. Gebruikers hebben nog steeds toegang tot openbare mappen met behulp van OWA of Outlook voor Mac.

Zie [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) (Beheerde verbindingen met openbare mappen in Outlook) voor meer informatie.
