---
title: Selfservice-aankoop van PowerShell
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797716"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="6a3cb-102">Selfservice-aankoop van PowerShell</span><span class="sxs-lookup"><span data-stu-id="6a3cb-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="6a3cb-103">Als u de MSCommerce PowerShell-module wilt gebruiken, moet u deze installeren op een Windows 10-apparaat met TLS 1.2 (lokale beheerdersmachtigingen vereist).</span><span class="sxs-lookup"><span data-stu-id="6a3cb-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="6a3cb-104">Importeren en verbinding maken met de MSCommerce-module.</span><span class="sxs-lookup"><span data-stu-id="6a3cb-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="6a3cb-105">Wanneer u wordt gevraagd u aan te melden, moet u de rolreferenties Globale of Factureringsbeheerder gebruiken.</span><span class="sxs-lookup"><span data-stu-id="6a3cb-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="6a3cb-106">Als u niet over TLS 1.2 hebt, krijgt u mogelijk de volgende foutmelding wanneer u probeert het beleid op te halen of bij te werken:</span><span class="sxs-lookup"><span data-stu-id="6a3cb-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="6a3cb-107">*ErrorMessage -De onderliggende verbinding is gesloten: er* is een onverwachte fout opgetreden bij een verzenden.</span><span class="sxs-lookup"><span data-stu-id="6a3cb-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



