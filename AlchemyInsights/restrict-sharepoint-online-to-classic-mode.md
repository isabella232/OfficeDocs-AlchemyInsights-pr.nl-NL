---
title: SharePoint Online beperken tot de klassieke modus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751417"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8d646-102">SharePoint Online beperken tot de klassieke modus</span><span class="sxs-lookup"><span data-stu-id="8d646-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8d646-103">Voor sommige organisaties is de klassieke modus nog steeds vereist.</span><span class="sxs-lookup"><span data-stu-id="8d646-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8d646-104">Hoewel er geen plannen zijn om de klassieke modus op een granulair niveau te verwijderen, kunt u niet langer een volledige organisatie (Tenant) beperken tot de klassieke modus voor lijsten en bibliotheken.</span><span class="sxs-lookup"><span data-stu-id="8d646-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8d646-105">De beheerder heeft de volgende opties voor het beheren van afzonderlijke lijsten en bibliotheken in de klassieke modus met behulp van granulaire schakelopties voor uitchecken, op de volgende niveaus:</span><span class="sxs-lookup"><span data-stu-id="8d646-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8d646-106">siteverzameling</span><span class="sxs-lookup"><span data-stu-id="8d646-106">site collection</span></span>
- <span data-ttu-id="8d646-107">site</span><span class="sxs-lookup"><span data-stu-id="8d646-107">site</span></span>
- <span data-ttu-id="8d646-108">lijst</span><span class="sxs-lookup"><span data-stu-id="8d646-108">list</span></span>
- <span data-ttu-id="8d646-109">bibliotheek</span><span class="sxs-lookup"><span data-stu-id="8d646-109">library</span></span>

<span data-ttu-id="8d646-110">Lijsten die gebruikmaken van bepaalde functies en aanpassingen die niet worden ondersteund door modern, worden ook automatisch doorgeschakeld naar de klassieke modus.</span><span class="sxs-lookup"><span data-stu-id="8d646-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8d646-111">Vanaf 1 april 2019 is het proces voor het uitschakelen van het deactiveren van de Tenant op basis van de moderne lijst en de Bibliotheken, en tot en met 31 mei 2019.</span><span class="sxs-lookup"><span data-stu-id="8d646-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8d646-112">De lijsten en bibliotheken in de klassieke modus als gevolg van het afmelden van de Tenant worden automatisch naar modern verschoven.</span><span class="sxs-lookup"><span data-stu-id="8d646-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8d646-113">Als u de klassieke modus nodig [hebt, raadpleegt u hier meer](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) informatie en PnP PowerShell-instructies [hier](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) met een beschrijving van de functies en hulpprogramma's die u vandaag kunt gebruiken voor de klassieke modus.</span><span class="sxs-lookup"><span data-stu-id="8d646-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
