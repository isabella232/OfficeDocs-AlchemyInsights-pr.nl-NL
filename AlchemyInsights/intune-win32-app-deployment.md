---
title: Implementatie van de Win32-app intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461793"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="0a484-102">Implementatie van de Win32-app intune</span><span class="sxs-lookup"><span data-stu-id="0a484-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="0a484-103">Microsoft intune maakt Win32-toepassingen, met inbegrip van, maar niet beperkt tot MSI en. EXE wordt geïmplementeerd op Windows 10-apparaten.</span><span class="sxs-lookup"><span data-stu-id="0a484-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="0a484-104">Voor de toepassing van het implementatie mechanisme is de functie voor intune-beheer uitbreidingen vereist.</span><span class="sxs-lookup"><span data-stu-id="0a484-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="0a484-105">De IME wordt automatisch geïnstalleerd als gevolg van het doel van een PowerShell-script of Win32-Toepassingsimplementatie voor een gebruiker/apparaat.</span><span class="sxs-lookup"><span data-stu-id="0a484-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="0a484-106">Er gelden ook een reeks vereisten waaraan moet worden voldaan om Win32-apps te kunnen implementeren, waaronder:</span><span class="sxs-lookup"><span data-stu-id="0a484-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="0a484-107">Ondersteunde platformen: Windows 10 versie 1607 of hoger (Enterprise, Pro en Education-versies).</span><span class="sxs-lookup"><span data-stu-id="0a484-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="0a484-108">Ondersteunde architectuur: x86 en x64.</span><span class="sxs-lookup"><span data-stu-id="0a484-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="0a484-109">Apparaatbeheer: AAD, lid geworden van automatisch ingeschreven berichten (waaronder hybride domein, en Groepsbeleid automatisch ingeschreven).</span><span class="sxs-lookup"><span data-stu-id="0a484-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="0a484-110">Opmaak van toepassingspakket:. **intunewin**  -bestand dat is gemaakt door het [Microsoft Win32-hulpprogramma](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)voor het voorbereiden van inhoud.</span><span class="sxs-lookup"><span data-stu-id="0a484-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="0a484-111">Zien</span><span class="sxs-lookup"><span data-stu-id="0a484-111">Limitations:</span></span>
    - <span data-ttu-id="0a484-112">Maximale grootte: 8GB.</span><span class="sxs-lookup"><span data-stu-id="0a484-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="0a484-113">Niet-ondersteunde architectuur: wapen.</span><span class="sxs-lookup"><span data-stu-id="0a484-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="0a484-114">Bekijk het document '[een Win32-app in Microsoft intune toevoegen, toewijzen en controleren](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)voor informatie over deze stappen.</span><span class="sxs-lookup"><span data-stu-id="0a484-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="0a484-115">Meer informatie over het oplossen van Toepassingsimplementatie in Windows, waaronder Win32-apps, kunt u bekijken in de volgende documenten:</span><span class="sxs-lookup"><span data-stu-id="0a484-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="0a484-116">Problemen bij het installeren van apps oplossen</span><span class="sxs-lookup"><span data-stu-id="0a484-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="0a484-117">Problemen met Win32-apps oplossen</span><span class="sxs-lookup"><span data-stu-id="0a484-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)