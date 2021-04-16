---
title: Dubbelklikken op een Office-bestand wordt niet geopend
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814800"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="2e7c5-102">Dubbelklikken op een Office-bestand wordt niet geopend</span><span class="sxs-lookup"><span data-stu-id="2e7c5-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="2e7c5-103">Nadat u op een Office-bestand hebt geklikt, wordt het programma mogelijk geopend, maar wordt het bestand zelf niet geopend.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="2e7c5-104">Of u krijgt de foutmelding: 'Er is een probleem opgetreden bij het verzenden van de opdracht naar het programma'.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="2e7c5-105">Er zijn veel oorzaken, maar de twee meest voorkomende oplossingen zijn:</span><span class="sxs-lookup"><span data-stu-id="2e7c5-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="2e7c5-106">Controleer vanuit Excel of de optie DDE is uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="2e7c5-107">U kunt de optie vinden door een nieuwe werkmap te maken en vervolgens Bestandsopties > te kiezen **> Geavanceerd.**</span><span class="sxs-lookup"><span data-stu-id="2e7c5-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="2e7c5-108">In de **sectie** Algemeen kunt u het selectievakje Andere toepassingen negeren **die gebruikmaken van DDE (Dynamic Data Exchange) uit.**</span><span class="sxs-lookup"><span data-stu-id="2e7c5-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="2e7c5-109">Voer een onlineherstel uit om de standaardinstellingen te herstellen.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="2e7c5-110">Klik op de knop Start van Windows en zoek naar 'Configuratiescherm'.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="2e7c5-111">Open het **Configuratiescherm** en ga naar **Programma's > programma's en functies.**</span><span class="sxs-lookup"><span data-stu-id="2e7c5-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="2e7c5-112">Klik vervolgens met de rechtermuisknop **op Microsoft Office [Versie]** en kies **Wijzigen > Online herstellen.**</span><span class="sxs-lookup"><span data-stu-id="2e7c5-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="2e7c5-113">Als geen van deze oplossingen werkt, kunt u een completere lijst met oplossingen vinden in het ondersteuningsartikel. Dubbelklikken op een [Office-bestand](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)wordt niet geopend.</span><span class="sxs-lookup"><span data-stu-id="2e7c5-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
