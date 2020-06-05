---
title: AIP-labelbeleid maken
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569033"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="1e5fb-102">AIP-labelbeleid maken</span><span class="sxs-lookup"><span data-stu-id="1e5fb-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="1e5fb-103">Azure Information Protection(AIP)-labels kunnen worden gebruikt met het volledige bereik van gegevens die een organisatie doorgaans maakt en opslaat, van de laagste classificatie van persoonsgegevens tot de hoogste classificatie van zeer vertrouwelijke gegevens.</span><span class="sxs-lookup"><span data-stu-id="1e5fb-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="1e5fb-104">Azure Information Protection Policies is van toepassing op de klassieke client Azure Information Protection (AIP) en niet op de [AIP Unified Labeling-client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="1e5fb-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="1e5fb-105">U meerdere elementen configureren in een AIP-beleid, inclusief opties zoals:</span><span class="sxs-lookup"><span data-stu-id="1e5fb-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="1e5fb-106">Optie voor welk label beheerders of gebruikers documenten en e-mails laat classificeren en beschermen (optioneel)</span><span class="sxs-lookup"><span data-stu-id="1e5fb-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="1e5fb-107">Optie om classificatie af te dwingen wanneer gebruikers documenten opslaan en e-mail verzenden</span><span class="sxs-lookup"><span data-stu-id="1e5fb-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="1e5fb-108">Optie om een e-mailbericht automatisch te labelen op basis van de bijlagen.</span><span class="sxs-lookup"><span data-stu-id="1e5fb-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="1e5fb-109">Optie om te bepalen of de informatiebeveiligingsbalk wordt weergegeven in Office-toepassingen</span><span class="sxs-lookup"><span data-stu-id="1e5fb-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="1e5fb-110">Zie: [Overzicht van het azure-beleid voor informatiebescherming](https://docs.microsoft.com/azure/information-protection/overview-policy)voor aanvullende opties en informatie over azure information protection.</span><span class="sxs-lookup"><span data-stu-id="1e5fb-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="1e5fb-111">Zie voor andere nuttige bronnen met betrekking tot AIP-beleid:</span><span class="sxs-lookup"><span data-stu-id="1e5fb-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="1e5fb-112">Zelfstudie: Beleidsinstellingen voor Azure Information Protection configureren en een nieuw label maken</span><span class="sxs-lookup"><span data-stu-id="1e5fb-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="1e5fb-113">Het azure-beleid voor informatiebeveiliging configureren</span><span class="sxs-lookup"><span data-stu-id="1e5fb-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="1e5fb-114">Gevoeligheidslabels en hun beleid maken en configureren</span><span class="sxs-lookup"><span data-stu-id="1e5fb-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="1e5fb-115">Handleidingen voor veelvoorkomende scenario's die Azure Information Protection gebruiken</span><span class="sxs-lookup"><span data-stu-id="1e5fb-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="1e5fb-116">Documentatie over Azure Information Protection controleren</span><span class="sxs-lookup"><span data-stu-id="1e5fb-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="1e5fb-117">Vereisten voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="1e5fb-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="1e5fb-118">Zelfstudie snel starten voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="1e5fb-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="1e5fb-119">Azure Information Protection-client downloaden</span><span class="sxs-lookup"><span data-stu-id="1e5fb-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)