---
title: 'Fout: de regels op deze computer komen niet overeen'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690958"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="98d82-102">Fout: de regels op deze computer komen niet overeen</span><span class="sxs-lookup"><span data-stu-id="98d82-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="98d82-103">Als u de bijgewerkte status van dit bekende probleem wilt zien, raadpleegt u [de regels op deze computer komen niet overeen met de regels op Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="98d82-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="98d82-104">Het Outlook-team heeft een oplossing geïmplementeerd in Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="98d82-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="98d82-105">De fix is al op Insider Fast en gaat naar het Monthly-kanaal, te laat 2020.</span><span class="sxs-lookup"><span data-stu-id="98d82-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="98d82-106">Wanneer u de vaste build hebt, kunt u het volgende doen: ' welke regels wilt u de laatste keer bewaren.</span><span class="sxs-lookup"><span data-stu-id="98d82-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="98d82-107">Kies server wanneer hierom wordt gevraagd, ga opnieuw in Outlook en Schakel regels die zijn uitgeschakeld opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="98d82-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="98d82-108">Wanneer de fix beschikbaar is, gebruikt u de volgende tijdelijke oplossing:</span><span class="sxs-lookup"><span data-stu-id="98d82-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="98d82-109">**Tijdelijke oplossing**: er is een probleem opgetreden bij recente rapporten voor personen die uitsluitend clientregels hebben gemaakt in de bureaubladversie van Outlook.</span><span class="sxs-lookup"><span data-stu-id="98d82-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="98d82-110">Als u het probleem blijft ondervinden, kunt u overwegen om de regels te verwijderen en regels alleen in OWA (Outlook Web app) te maken en te bewerken tot het probleem is opgelost.</span><span class="sxs-lookup"><span data-stu-id="98d82-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="98d82-111">Als u de regels niet handmatig kunt verwijderen, kunt u een Outlook-opdracht uitvoeren wanneer u Outlook start voor het uitvoeren van Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="98d82-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="98d82-112">De regels voor de client en server worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="98d82-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="98d82-113">Alle regels voor alle accounts in het Outlook-profiel worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="98d82-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="98d82-114">Deze opdracht wordt verder beschreven in het artikel opdrachtregelopties.</span><span class="sxs-lookup"><span data-stu-id="98d82-114">This command is further documented in the Command-line switches article.</span></span>

