---
title: 'Fout: De regels op deze computer komen niet overeen'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782947"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="04580-102">Fout: De regels op deze computer komen niet overeen</span><span class="sxs-lookup"><span data-stu-id="04580-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="04580-103">Zie De regels op deze [computer](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) komen niet overeen met de regels op Microsoft Exchange als u de bijgewerkte status van dit bekende probleem wilt zien</span><span class="sxs-lookup"><span data-stu-id="04580-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="04580-104">Het Outlook-team heeft een oplossing geïmplementeerd in build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="04580-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="04580-105">De oplossing is al bij Insider Fast en gaat eind juni 2020 naar Monthly Channel.</span><span class="sxs-lookup"><span data-stu-id="04580-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="04580-106">Als u de vaste build hebt, krijgt u mogelijk nog één keer de vraag 'Welke regels wilt u behouden'.</span><span class="sxs-lookup"><span data-stu-id="04580-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="04580-107">Kies Server wanneer u daarom wordt gevraagd en ga terug in Outlook en schakel alle uitgeschakelde regels opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="04580-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="04580-108">Gebruik de volgende tijdelijke oplossing totdat de oplossing beschikbaar is:</span><span class="sxs-lookup"><span data-stu-id="04580-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="04580-109">**Tijdelijke oplossing:** In recente rapporten is het probleem opgetreden voor personen die alleen clientregels hebben gemaakt in de bureaubladversie van Outlook.</span><span class="sxs-lookup"><span data-stu-id="04580-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="04580-110">Als u het probleem blijft tegen komen, kunt u overwegen de regels te verwijderen en vervolgens alleen regels te maken en te bewerken in OWA (Outlook Web App) totdat het probleem is opgelost.</span><span class="sxs-lookup"><span data-stu-id="04580-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="04580-111">Als u de regels niet handmatig kunt verwijderen, kunt u een Outlook-opdracht uitvoeren wanneer u Outlook start door Outlook.exe /cleanrules uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="04580-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="04580-112">Hiermee worden zowel de client- als de serverregels verwijderd.</span><span class="sxs-lookup"><span data-stu-id="04580-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="04580-113">Hiermee worden alle regels voor alle accounts in het Outlook-profiel verwijderd.</span><span class="sxs-lookup"><span data-stu-id="04580-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="04580-114">Deze opdracht wordt verder beschreven in het artikel Command-line switches.</span><span class="sxs-lookup"><span data-stu-id="04580-114">This command is further documented in the Command-line switches article.</span></span>

