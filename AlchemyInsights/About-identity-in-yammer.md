---
title: Over identiteit in Yammer
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
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148197"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="228a9-102">Over identiteit in Yammer</span><span class="sxs-lookup"><span data-stu-id="228a9-102">About identity in Yammer</span></span>

<span data-ttu-id="228a9-103">Het wordt aanbevolen dat alle netwerken de volgende stappen ondernemen om identiteitsgerelateerde problemen te voorkomen:</span><span class="sxs-lookup"><span data-stu-id="228a9-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="228a9-104">Afdwingen Office 365-identiteit na het inrichten van Microsoft 365-accounts voor gebruikers in Azure AD om ervoor te zorgen dat alle gebruikers zich aanmelden met hun primaire Microsoft 365-account.</span><span class="sxs-lookup"><span data-stu-id="228a9-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="228a9-105">Zie [Office 365-identiteit afdwingen voor Yammer-gebruikers voor](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="228a9-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="228a9-106">Meerdere Yammer-netwerken consolideren.</span><span class="sxs-lookup"><span data-stu-id="228a9-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="228a9-107">Met verouderde Yammer-configuraties kunnen meerdere Yammer-netwerken worden verbonden met één tenant.</span><span class="sxs-lookup"><span data-stu-id="228a9-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="228a9-108">Zie [Netwerkmigratie - Meerdere Yammer-netwerken consolideren](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="228a9-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="228a9-109">Optioneel u licenties voor Yammer afdwingen om gebruikers van Yammer te blokkeren als ze geen licentie hebben.</span><span class="sxs-lookup"><span data-stu-id="228a9-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="228a9-110">Zie [Yammer-gebruikerslicenties beheren in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="228a9-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="228a9-111">Controleer ten slotte de gebruikerslijst voor oudere Yammer-netwerken en schort oudere gebruikers op.</span><span class="sxs-lookup"><span data-stu-id="228a9-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="228a9-112">Het wordt aanbevolen om gebruikers op te schorten (te deactiveren) in plaats van ze te verwijderen, omdat verwijdering onomkeerbaar is.</span><span class="sxs-lookup"><span data-stu-id="228a9-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="228a9-113">Zie [Yammer-gebruikers controleren in netwerken die zijn verbonden met Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) en [Gebruikers verwijderen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="228a9-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="228a9-114">Als u Yammer configureert met deze stappen, u ook uw Yammer-netwerk configureren voor native modus voor Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="228a9-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="228a9-115">Zie [Uw Yammer-netwerk configureren voor native modus voor Microsoft 365 voor](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="228a9-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>