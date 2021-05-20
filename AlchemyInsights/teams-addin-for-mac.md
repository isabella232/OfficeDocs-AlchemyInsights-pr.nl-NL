---
title: Teams invoeging voor Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582065"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="a120c-102">Teams invoeging voor Mac</span><span class="sxs-lookup"><span data-stu-id="a120c-102">Teams add-in for Mac</span></span>

<span data-ttu-id="a120c-103">Als u een probleem wilt oplossen Teams gebruikers van een Mac-besturingssysteem, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="a120c-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="a120c-104">**Stap 1:** Als u hybride Exchange on-premises (2016 CU3 of hoger vereist) hebt, gebruikt u het hulpprogramma Test-HMA.ps1 om te controleren of hybride moderne verificatie correct is geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="a120c-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="a120c-105">Zie Valideren van hybride moderne verificatie voor Outlook [voor iOS en Android voor meer informatie.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="a120c-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="a120c-106">**Opmerking** Gebruik de UPN-adresnotatie [(bijvoorbeeld](mailto:username@contoso.com)username@contoso.com ), niet domein\gebruikersnaam.</span><span class="sxs-lookup"><span data-stu-id="a120c-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="a120c-107">Doe dit zelfs voor gebruikers met Exchange Online postvakken.</span><span class="sxs-lookup"><span data-stu-id="a120c-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="a120c-108">**Stap 2:** Laat de gebruiker naar **Hulpmiddelenaccounts**  >  **gaan**... in Outlook voor Mac en het account zoeken en selecteren.</span><span class="sxs-lookup"><span data-stu-id="a120c-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="a120c-109">Bevestig dat de gebruikersnaam die wordt vermeld, in UPN-indeling staat [(bijvoorbeeld username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="a120c-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="a120c-110">**Stap 3:** Controleer of de gebruiker een gelicentieerde Microsoft Teams is.</span><span class="sxs-lookup"><span data-stu-id="a120c-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="a120c-111">De gebruiker moet het abonnement Office 365 voor Mac, productversie 16.24 of hoger gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a120c-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>