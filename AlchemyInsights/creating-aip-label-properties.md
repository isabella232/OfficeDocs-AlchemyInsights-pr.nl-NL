---
title: BEHEERDERS etiketten maken
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732170"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="d359c-102">BEHEERDERS etiketten maken</span><span class="sxs-lookup"><span data-stu-id="d359c-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="d359c-103">Azure Information Protection-labels (beheerders instelling) kunnen worden gebruikt met de volledige reeks gegevens die een organisatie meestal maakt en opslaat, van de laagste classificatie van persoonlijke gegevens, tot de hoogst mogelijke indeling van uiterst vertrouwelijke gegevens.</span><span class="sxs-lookup"><span data-stu-id="d359c-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="d359c-104">Azure Information Protection-beleid is van toepassing op de klassieke client van Azure Information Protection (BEHEERDERSversie) en niet op de client met het  [beheerders Unified-etiket](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="d359c-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="d359c-105">U kunt meerdere elementen configureren in een beheerders beleid, waaronder opties zoals:</span><span class="sxs-lookup"><span data-stu-id="d359c-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="d359c-106">Optie waarvoor beheerders documenten en e-mailberichten in de gebruikersclassificatie en beveiliging (optioneel) kunnen worden geclassificeerd en beschermd.</span><span class="sxs-lookup"><span data-stu-id="d359c-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="d359c-107">Optie voor het afdwingen van de classificatie wanneer gebruikers documenten opslaan en e-mail verzenden</span><span class="sxs-lookup"><span data-stu-id="d359c-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="d359c-108">Optie voor het automatisch markeren van een e-mailbericht op basis van de bijlagen.</span><span class="sxs-lookup"><span data-stu-id="d359c-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="d359c-109">Optie om te bepalen of de informatie beschermings balk wordt weergegeven in Office-toepassingen</span><span class="sxs-lookup"><span data-stu-id="d359c-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="d359c-110">Zie het volgende artikel voor meer opties en informatie over Azure Information Protection-beleid: [overzicht van Azure Information Protection-beleid](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="d359c-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="d359c-111">Voor andere nuttige informatiebronnen over het beheerders beleid raadpleegt u:</span><span class="sxs-lookup"><span data-stu-id="d359c-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="d359c-112">Zelfstudie: beleidsinstellingen voor Azure Information Protection configureren en een nieuw etiket maken</span><span class="sxs-lookup"><span data-stu-id="d359c-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d359c-113">Het Azure Information Protection-beleid configureren</span><span class="sxs-lookup"><span data-stu-id="d359c-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="d359c-114">Gevoeligheidslabels en hun beleid maken en configureren</span><span class="sxs-lookup"><span data-stu-id="d359c-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="d359c-115">Handleidingen voor veelvoorkomende scenario's die gebruikmaken van Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d359c-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="d359c-116">Azure Information Protection-documentatie raadplegen</span><span class="sxs-lookup"><span data-stu-id="d359c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="d359c-117">Vereisten voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d359c-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="d359c-118">Handleiding aan de slag voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d359c-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d359c-119">Azure Information Protection-client downloaden</span><span class="sxs-lookup"><span data-stu-id="d359c-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)