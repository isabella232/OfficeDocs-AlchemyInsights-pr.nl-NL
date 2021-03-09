---
title: Fout met proxyadres bij het maken van een gedeeld postvak
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568285"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="a531e-102">Fout met proxyadres bij het maken van een postvak of ander object met e-mail</span><span class="sxs-lookup"><span data-stu-id="a531e-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="a531e-103">Als u een object wilt maken dat e-mail kan gebruiken (postvak, gedeeld postvak, enzovoort) en het foutbericht 'Het proxyadres 'SMTP:alias@domain.com' wordt gebruikt...' hebt ontvangen, wordt het gekozen e-mailadres al overgenomen door een ander object in uw organisatie met e-mail.</span><span class="sxs-lookup"><span data-stu-id="a531e-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="a531e-104">U moet de gebruiker, groep, het gedeelde postvak of de openbare map met dit e-mailadres vinden en deze verwijderen of het e-mailadres wijzigen.</span><span class="sxs-lookup"><span data-stu-id="a531e-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="a531e-105">Vervolgens kunt u een nieuw object met e-mail maken met het gratis e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="a531e-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="a531e-106">Gebruik Zoeken op de startpagina om de zoekfunctie te vinden.</span><span class="sxs-lookup"><span data-stu-id="a531e-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="a531e-107">U kunt ook de volgende PowerShell-opdracht van Exchange Online gebruiken om hier naar te zoeken:</span><span class="sxs-lookup"><span data-stu-id="a531e-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="a531e-108">Als u het bestaande e-mailadres niet wilt verwijderen, kiest u een nieuw e-mailadres voor het nieuwe object dat u maakt.</span><span class="sxs-lookup"><span data-stu-id="a531e-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  