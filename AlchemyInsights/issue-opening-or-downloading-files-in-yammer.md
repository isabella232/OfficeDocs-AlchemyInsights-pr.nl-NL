---
title: Problemen met het openen of downloaden van bestanden in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148249"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="c68b0-102">Problemen met het openen of downloaden van bestanden in Yammer</span><span class="sxs-lookup"><span data-stu-id="c68b0-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="c68b0-103">Classic Yammer ondersteunt meerdere opties voor bestandsuploads naar berichten en groepen.</span><span class="sxs-lookup"><span data-stu-id="c68b0-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="c68b0-104">Afhankelijk van de netwerkconfiguratie worden bestanden standaard opgeslagen in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c68b0-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="c68b0-105">De bestandenkiezer in de nieuwe Yammer biedt nog niet alle opties die beschikbaar zijn in de klassieke Yammer.</span><span class="sxs-lookup"><span data-stu-id="c68b0-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="c68b0-106">Een toekomstige update voegt extra functies toe.</span><span class="sxs-lookup"><span data-stu-id="c68b0-106">A future update will add additional features.</span></span> <span data-ttu-id="c68b0-107">Zie [Een bestand of afbeelding toevoegen aan een Yammer-gespreksbericht voor](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c68b0-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="c68b0-108">**Kan een bestand niet openen of downloaden**</span><span class="sxs-lookup"><span data-stu-id="c68b0-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="c68b0-109">Een bestand kan worden geüpload naar Yammer, maar ook een koppeling naar een bestand in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c68b0-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="c68b0-110">Als u problemen wilt oplossen, moet u eerst de locatie van het bestand bepalen.</span><span class="sxs-lookup"><span data-stu-id="c68b0-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="c68b0-111">Als het bestand is geüpload naar Yammer, heeft het een URL van \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="c68b0-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="c68b0-112">Controleer of de vereiste URL's en IP-adressen worden gedeblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="c68b0-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="c68b0-113">Zie voor meer informatie het blogbericht [Het gebruik van hardgecodeerde IP-adressen voor Yammer wordt niet aanbevolen.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)</span><span class="sxs-lookup"><span data-stu-id="c68b0-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="c68b0-114">Controleer of een gebruiker die ook een globale beheerder is, het bestand kan downloaden.</span><span class="sxs-lookup"><span data-stu-id="c68b0-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="c68b0-115">Als het bestand privé is, moet u mogelijk de modus Privé-inhoud gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c68b0-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="c68b0-116">Zie [Privé-inhoud bewaken in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c68b0-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="c68b0-117">**Gasten en bestanden op Yammer-netwerkniveau in SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="c68b0-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="c68b0-118">[Gasten op netwerkniveau in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) gebruiken Azure AD B2B niet en zijn intern voor de Yammer-service, zodat ze geen toegang hebben tot Yammer-bestanden die zijn opgeslagen in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c68b0-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="c68b0-119">Maak een externe AAD B2B-gebruiker die met die identiteit toegang heeft tot documentbibliotheken in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c68b0-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="c68b0-120">Zie Ondersteuning voor ondersteuning voor gasten [in Yammer in Yammer voor](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)meer informatie over toekomstige Azure AD B2B-gastondersteuning in Yammer.</span><span class="sxs-lookup"><span data-stu-id="c68b0-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>