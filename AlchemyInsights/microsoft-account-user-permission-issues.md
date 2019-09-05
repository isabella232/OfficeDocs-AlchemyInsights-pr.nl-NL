---
title: Probleem oplossen-gebruiker niet gevonden in map
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754187"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ae04b-102">Probleem oplossen-gebruiker niet gevonden in map</span><span class="sxs-lookup"><span data-stu-id="ae04b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ae04b-103">Als gebruikers ontvangen foutbericht ' gebruiker kan niet worden gevonden ' in de map.</span><span class="sxs-lookup"><span data-stu-id="ae04b-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ae04b-104">Probeer het opnieuw waar het probleem type is gebruiker niet in de map.</span><span class="sxs-lookup"><span data-stu-id="ae04b-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ae04b-105">De volgende stappen kunnen worden voltooid om het probleem op te lossen.</span><span class="sxs-lookup"><span data-stu-id="ae04b-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ae04b-106">Zorg ervoor dat het account dat de e-mail uitnodiging heeft geaccepteerd hetzelfde account is dat wordt gebruikt om later aan te melden.</span><span class="sxs-lookup"><span data-stu-id="ae04b-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ae04b-107">Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en zich aan te melden bij de site.</span><span class="sxs-lookup"><span data-stu-id="ae04b-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ae04b-108">Zie voor meer informatie, [over het beheren van aliassen voor uw micro</a> Soft-account voor het beheren van de aanmelding bij Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ae04b-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ae04b-109">Blader naar elke site (s) waarin de gebruiker de fout ontvangt.</span><span class="sxs-lookup"><span data-stu-id="ae04b-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ae04b-110">Voeg '/_layouts/15/people.aspx/membershipgroupid = 0 ' (binnen de dubbele aanhalingstekens) toe aan het einde van de site-URL.</span><span class="sxs-lookup"><span data-stu-id="ae04b-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ae04b-111">Voorbeeld: https:/_Lt_ "contoso">. SharePoint. com/_layouts/15/people. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="ae04b-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ae04b-112">Selecteer de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="ae04b-112">Select the user from the list.</span></span>

- <span data-ttu-id="ae04b-113">Klik op **Gebruikersmachtigingen verwijderen** uit het lint.</span><span class="sxs-lookup"><span data-stu-id="ae04b-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ae04b-114">Voeg de gebruiker terug en verzend de uitnodiging opnieuw naar de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="ae04b-114">Add back the User and Resend the invite to the user.</span></span>

