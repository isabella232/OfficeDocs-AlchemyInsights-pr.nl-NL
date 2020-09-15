---
title: ATP voor SharePoint, OneDrive en Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715556"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="0483f-102">ATP voor SharePoint, OneDrive en Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0483f-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="0483f-103">Voer de volgende stappen uit om Advanced Threat Protection in te schakelen:</span><span class="sxs-lookup"><span data-stu-id="0483f-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="0483f-104">Ga naar [https://protection.office.com](https://protection.office.com) en meld u aan met een globale beheerder of een beheerdersaccount voor beveiliging.</span><span class="sxs-lookup"><span data-stu-id="0483f-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="0483f-105">Kies in het linker navigatiedeelvenster onder **Threat Management**de optie **beleids** \> **veilige bijlagen**.</span><span class="sxs-lookup"><span data-stu-id="0483f-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="0483f-106">Selecteer **ATP inschakelen voor SharePoint, OneDrive en Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="0483f-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="0483f-107">[Maak een waarschuwings beleid](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) voor meldingen om meldingen te ontvangen wanneer we kwaadaardige bestanden detecteren.</span><span class="sxs-lookup"><span data-stu-id="0483f-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="0483f-108">Zie het volgende [onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)voor uitgebreide instructies.</span><span class="sxs-lookup"><span data-stu-id="0483f-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="0483f-109">**Opmerking**: met behulp van deze optie wordt niet elk afzonderlijk bestand in SharePoint Online, OneDrive voor bedrijven of Microsoft teams gescand.</span><span class="sxs-lookup"><span data-stu-id="0483f-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="0483f-110">Bestanden worden asynchroon gescand door een proces waarbij activiteiten met gedeelde activiteiten, gast activiteiten en bedreigings signalen worden gebruikt om te zoeken naar schadelijke bestanden.</span><span class="sxs-lookup"><span data-stu-id="0483f-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="0483f-111">Zie het volgende [onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0483f-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
