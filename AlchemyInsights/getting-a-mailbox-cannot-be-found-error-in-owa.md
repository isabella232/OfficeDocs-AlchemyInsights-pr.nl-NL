---
title: 126 Het verkrijgen van een postvak kan niet worden gevonden fout in OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426657"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="adebe-102">Krijgt u een foutbericht voor een postvak dat niet is gevonden in de webversie van Outlook?</span><span class="sxs-lookup"><span data-stu-id="adebe-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="adebe-103">Als u de webversie van Outlook  gebruikt en een postvak niet kan worden gevonden voor fout, heeft het account dat u hebt gebruikt om verbinding te maken met de webversie van Outlook geen Exchange Online-licentie en is er daarom geen postvak gekoppeld aan het account.</span><span class="sxs-lookup"><span data-stu-id="adebe-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="adebe-104">Uw beheerder kan een licentie aan uw account toewijzen door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="adebe-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="adebe-105">Open het [Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/homepage) en  ga naar **Actieve** gebruikers onder de sectie Gebruikers en selecteer de gebruiker die de fout ziet.</span><span class="sxs-lookup"><span data-stu-id="adebe-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="adebe-106">Ga op de pagina van de gebruiker die wordt geopend  naar de sectie Licenties en apps, selecteer de juiste locatiewaarde en **wijs** een licentie toe die Exchange Online bevat (vouw de licentie uit om de details ervan te zien).</span><span class="sxs-lookup"><span data-stu-id="adebe-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="adebe-107">Wanneer u gereed bent, klikt u op **Wijzigingen opslaan**.</span><span class="sxs-lookup"><span data-stu-id="adebe-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="adebe-108">Als de licentie al aan een gebruikersaccount is toegewezen, helpt het verwijderen en opnieuw toewijzen van de licentie in sommige gevallen om het probleem op te lossen en correct in te stellen in het systeem:</span><span class="sxs-lookup"><span data-stu-id="adebe-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="adebe-109">Controleer of uw M365 Exchange Online -abonnementen (en andere, als u er al bent) actueel zijn en nog niet onlangs zijn verlopen.</span><span class="sxs-lookup"><span data-stu-id="adebe-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="adebe-110">Nadat u ervoor hebt zorgen dat uw abonnement niet is verlopen en er een geldige licentie is toegewezen aan het gebruikersaccount, kan het tot 24 uur duren voordat de licentie is ingericht, zodat u mogelijk moet wachten totdat het probleem is opgelost.</span><span class="sxs-lookup"><span data-stu-id="adebe-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="adebe-111">Zie Licenties toewijzen [en beheren voor meer informatie.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="adebe-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>