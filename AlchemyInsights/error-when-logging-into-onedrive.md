---
title: 0x8004de40-fout bij het starten van OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823017"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="19360-102">0x8004de40-fout bij het starten van OneDrive</span><span class="sxs-lookup"><span data-stu-id="19360-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="19360-103">Als u een foutmelding krijgt **0x8004de40** wanneer u zich aanmeldt bij OneDrive, start u de computer opnieuw op terwijl u verbinding hebt met het domein van uw werk of school.</span><span class="sxs-lookup"><span data-stu-id="19360-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="19360-104">Als u deze foutmelding krijgt nadat u de computer opnieuw hebt opgestart, kunt u dit proberen wanneer u verbinding hebt met uw werk-of school domein:</span><span class="sxs-lookup"><span data-stu-id="19360-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="19360-105">Klik op Start en typ **cmd** of **Command prompt**  in het zoekvak, klik met de rechtermuisknop op de opdrachtprompt-app en selecteer  **als administrator uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="19360-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="19360-106">Als u wordt gevraagd om een beheerderswachtwoord of een bevestiging, typt u het wachtwoord of klikt u op **toestaan** .</span><span class="sxs-lookup"><span data-stu-id="19360-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="19360-107">Typ in het venster met de opdracht prompt de tekst **dsregcmd/Leave**  en wacht totdat de opdracht klaar is.</span><span class="sxs-lookup"><span data-stu-id="19360-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="19360-108">Typ vervolgens **dsregcmd/join** en wacht tot de opdracht klaar is.</span><span class="sxs-lookup"><span data-stu-id="19360-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="19360-109">Start de computer opnieuw op.</span><span class="sxs-lookup"><span data-stu-id="19360-109">Reboot your computer.</span></span>
