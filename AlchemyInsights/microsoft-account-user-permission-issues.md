---
title: Problemen oplossen-gebruiker is niet gevonden in de adreslijst
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725402"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="7cc44-102">Problemen oplossen-gebruiker is niet gevonden in de adreslijst</span><span class="sxs-lookup"><span data-stu-id="7cc44-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="7cc44-103">Als gebruikers in de adreslijst foutbericht ' gebruiker kan niet vinden ' wordt weergegeven, probeer het dan opnieuw.</span><span class="sxs-lookup"><span data-stu-id="7cc44-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="7cc44-104">U kunt de volgende stappen uitvoeren om het probleem op te lossen.</span><span class="sxs-lookup"><span data-stu-id="7cc44-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="7cc44-105">Zorg ervoor dat de account die de uitnodiging voor e-mail heeft geaccepteerd, gelijk is aan het account waarmee u zich later aanmeldt.</span><span class="sxs-lookup"><span data-stu-id="7cc44-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="7cc44-106">Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en u aan te melden bij de site.</span><span class="sxs-lookup"><span data-stu-id="7cc44-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="7cc44-107">Zie [aliassen voor uw Microsoft-account beheren voor meer informatie over </a> het beheren van de microsoft 365-aanmelding](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7cc44-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="7cc44-108">Blader naar een of meer sites waarbij de gebruiker de fout ontvangt.</span><span class="sxs-lookup"><span data-stu-id="7cc44-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="7cc44-109">U kunt "/_layouts/15/people.aspx/membershipgroupid = 0" (binnen de dubbele aanhalingstekens) toevoegen aan het einde van de URL van de site.</span><span class="sxs-lookup"><span data-stu-id="7cc44-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="7cc44-110">Voorbeeld: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="7cc44-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="7cc44-111">Selecteer de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="7cc44-111">Select the user from the list.</span></span>

- <span data-ttu-id="7cc44-112">Klik op **Gebruikersmachtigingen verwijderen** op het lint.</span><span class="sxs-lookup"><span data-stu-id="7cc44-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="7cc44-113">De gebruiker opnieuw toevoegen en de uitnodiging opnieuw verzenden aan de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="7cc44-113">Add back the User and Resend the invite to the user.</span></span>

