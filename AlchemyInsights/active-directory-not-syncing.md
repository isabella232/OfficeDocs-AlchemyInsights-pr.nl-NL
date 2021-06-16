---
title: Active Directory wordt niet gesynchroniseerd
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930970"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="c4309-102">Active Directory wordt niet gesynchroniseerd</span><span class="sxs-lookup"><span data-stu-id="c4309-102">Active Directory not syncing</span></span>

<span data-ttu-id="c4309-103">Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie', of als u ziet dat de adreslijstsynchronisatiestatus in de beheerportal van Office zegt: 'Laatst gesynchroniseerd meer dan 3 dagen geleden', kan het zijn dat AADConnect onjuiste instellingen of onvoldoende machtigingen heeft om een synchronisatie uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="c4309-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="c4309-104">Als u AADConnect opnieuw installeert met behulp van express-instellingen, kan het probleem snel worden opgelost:</span><span class="sxs-lookup"><span data-stu-id="c4309-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="c4309-105">[Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="c4309-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="c4309-106">[Volg de instructies voor het snel installeren.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="c4309-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="c4309-107">Azure AD Connect moet worden geïnstalleerd op Windows Server 2012 of hoger.</span><span class="sxs-lookup"><span data-stu-id="c4309-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="c4309-108">Deze server moet lid zijn van een domein en kan een domeincontroller of een lidserver zijn.</span><span class="sxs-lookup"><span data-stu-id="c4309-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="c4309-109">Bekijk Vereisten voor Azure AD-Verbinding maken vereisten en vereisten voor [Azure AD-Verbinding maken.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="c4309-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="c4309-110">Zie [Azure AD-Verbinding maken: Accounts en machtigingen](/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.</span><span class="sxs-lookup"><span data-stu-id="c4309-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
