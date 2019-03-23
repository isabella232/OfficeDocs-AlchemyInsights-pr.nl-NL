---
title: 1332 OWA - postvak (s) worden niet uitgevoerd voor een postbus
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784337"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="34fb7-102">Een regel voor postvak in werkt niet zoals verwacht</span><span class="sxs-lookup"><span data-stu-id="34fb7-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="34fb7-103">Controleer of de volgende instellingen:</span><span class="sxs-lookup"><span data-stu-id="34fb7-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="34fb7-104">Een bericht kan worden omgeleid, doorgestuurd of beantwoord automatisch op basis van regels voor postvak in slechts één keer.</span><span class="sxs-lookup"><span data-stu-id="34fb7-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="34fb7-105">Een omleiding regel (regel voor het postvak of e-mailregel stroom, ook bekend als een regel vervoer) kan een maximum van tien doorsturen geadresseerden toevoegen aan een bericht.</span><span class="sxs-lookup"><span data-stu-id="34fb7-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="34fb7-106">Zie [limieten voor journaal, vervoer, en postvak in](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="34fb7-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="34fb7-107">Regels van postvak in werken op het postvak van de andere berichten niet.</span><span class="sxs-lookup"><span data-stu-id="34fb7-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="34fb7-108">Zie voor meer informatie over de postbus alternatieve logboekregistratie [postbus alternatieve logboekregistratie in](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="34fb7-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="34fb7-109">U kunt deze problemen oplossen door Zie [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="34fb7-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="34fb7-110">Als de bovenstaande problemen zijn niet van toepassing, het postvak in regel diagnostisch rapport uitvoeren voordat u het probleem aan Microsoft Support escaleren:</span><span class="sxs-lookup"><span data-stu-id="34fb7-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="34fb7-111">Open het postvak in Outlook op het web en klik op **Instellingen** \> **Opties** \> **e-mail organiseren** \> **regels voor postvak in**.</span><span class="sxs-lookup"><span data-stu-id="34fb7-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="34fb7-112">Klik onderaan de pagina op **Als uw regels niet, klikt u hier werkt voor het genereren van een diagnostisch rapport**.</span><span class="sxs-lookup"><span data-stu-id="34fb7-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

