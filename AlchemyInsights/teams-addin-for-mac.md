---
title: Invoegtoepassing teams voor Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629491"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="8242c-102">Invoegtoepassing teams voor Mac</span><span class="sxs-lookup"><span data-stu-id="8242c-102">Teams add-in for Mac</span></span>

<span data-ttu-id="8242c-103">Voer de volgende stappen uit als u een ontbrekende invoegtoepassing voor teams voor een Mac-besturingssysteem wilt problemen:</span><span class="sxs-lookup"><span data-stu-id="8242c-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="8242c-104">**Stap 1:** Als u een hybride Exchange on-premises (2016 CU3 of hoger) hebt, gebruikt u het hulpprogramma Test-HMA.ps1 om te controleren of de hybride moderne verificatie correct is geconfigureerd.</span><span class="sxs-lookup"><span data-stu-id="8242c-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="8242c-105">Zie [hybride instellingen voor moderne verificatie valideren voor Outlook voor IOS en Android](https://aka.ms/AA980zq)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8242c-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="8242c-106">**Opmerking** Gebruik de notatie voor de UPN-adres (bijvoorbeeld [username@contoso.com](mailto:username@contoso.com)), niet DOMEIN\gebruikersnaam.</span><span class="sxs-lookup"><span data-stu-id="8242c-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="8242c-107">Doe dit ook voor gebruikers met postvakken van Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8242c-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="8242c-108">**Stap 2:** Laat de gebruiker naar **extra**  >  **accounts**gaan... in Outlook voor Mac, zoekt en selecteert u het account.</span><span class="sxs-lookup"><span data-stu-id="8242c-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="8242c-109">Controleer of de naam van de gebruikersnaam in de weergegeven UPN-indeling is (bijvoorbeeld [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="8242c-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="8242c-110">**Stap 3:** Controleer of de gebruiker een licentie heeft voor Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="8242c-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="8242c-111">De gebruiker moet het Office 365 voor Mac-abonnement, productversie 16,24 of hoger, gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8242c-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>