---
title: Problemen met “Openen met Verkenner“ oplossen in SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803033"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b5717-102">Problemen met “Openen met Verkenner“ oplossen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b5717-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="b5717-103">De opdracht Openen met Verkenner opent een lokaal exemplaar van Windows Verkenner, die de mappenstructuur op de server weergeeft, waarop de SharePoint-site wordt gehost.</span><span class="sxs-lookup"><span data-stu-id="b5717-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="b5717-104">We raden u dus aan om [SharePoint-bestanden te synchroniseren met de nieuwe OneDrive-synchronisatieclient](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, die beschikt over [Bestanden op aanvraag](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), omdat u daarmee lokaal toegang tot uw bestanden hebt en omdat dat het snelst werkt.</span><span class="sxs-lookup"><span data-stu-id="b5717-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="b5717-105">Als u ervoor hebt gekozen om de Verkenner-weergave te gebruiken in plaats van de nieuwe OneDrive-synchronisatieclient, moet u de stappen en aanbevolen procedures in de volgende artikelen volgen:</span><span class="sxs-lookup"><span data-stu-id="b5717-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b5717-106">Het gebruik van de opdracht Openen met Explorer om problemen op te lossen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b5717-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- <span data-ttu-id="b5717-107">[Openen in Verkenner gebruiken om bibliotheekbestanden te kopiëren of te verplaatsen](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="b5717-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

> [!Note]  
> <span data-ttu-id="b5717-108">De knop **Openen in Verkenner** verschijnt niet in de nieuwe bibliotheekervaring.</span><span class="sxs-lookup"><span data-stu-id="b5717-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b5717-109">Selecteer de vervolgkeuzelijst **Weergave** in de rechterbovenhoek (de naam van de vervolgkeuzelijst is afhankelijk van de huidige weergave) en selecteer vervolgens **Weergeven in Verkenner**.</span><span class="sxs-lookup"><span data-stu-id="b5717-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="b5717-110">De functie Openen met Verkenner van SharePoint maakt gebruik van ActiveX-besturingselementen en wordt daarom alleen ondersteund in Internet Explorer 10 of 11.</span><span class="sxs-lookup"><span data-stu-id="b5717-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b5717-111">Openen met Explorer werkt in Windows niet in Microsoft Edge, Google Chrome of Mozilla Firefox, of met het Mac-platform.</span><span class="sxs-lookup"><span data-stu-id="b5717-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b5717-112">Om deze reden is de optie Verkennerweergave mogelijk niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="b5717-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="b5717-113">[Waarom knoppen niet beschikbaar zijn op het lint van SharePoint](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="b5717-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

