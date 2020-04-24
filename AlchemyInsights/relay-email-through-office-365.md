---
title: E-mail omleiden via Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785190"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="ff83e-102">Een multifunctioneel apparaat of een toepassing instellen voor het verzenden van e-mail</span><span class="sxs-lookup"><span data-stu-id="ff83e-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="ff83e-103">Zie [Een multifunctioneel apparaat of een toepassing instellen voor het verzenden van e-mail via Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3) voor meer informatie over de opties en de uit te voeren stappen.</span><span class="sxs-lookup"><span data-stu-id="ff83e-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="ff83e-104">**Opmerking:** als u een apparaat of toepassing hebt die sinds kort niet meer werkt, houd er dan rekening mee dat volgens planning onlangs is begonnen met het [uitschakelen van het 3DES-encryptiealgoritme](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="ff83e-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="ff83e-105">Als u de apparaten wilt zien die worden beïnvloed, gaat u naar het [SMTP-verificatierapport voor clients](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ff83e-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="ff83e-106">Veelvoorkomende fouten kunnen lijken op: verificatiefouten, TLS-fouten, encryptiealgoritmefouten, algoritmen die niet overeenkomen of verbroken verbinding.</span><span class="sxs-lookup"><span data-stu-id="ff83e-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="ff83e-107">Hoe u het probleem op kunt lossen:</span><span class="sxs-lookup"><span data-stu-id="ff83e-107">To resolve the issue:</span></span>
 - <span data-ttu-id="ff83e-108">**Windows Server 2003 IIS SMTP werkt niet meer. Er is een nieuwe versie van Windows vereist.**</span><span class="sxs-lookup"><span data-stu-id="ff83e-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="ff83e-109">Neem contact op met de fabrikant van uw toepassing of apparaat om na te vragen of een modern encryptiealgoritme wordt ondersteund of of er een update is.</span><span class="sxs-lookup"><span data-stu-id="ff83e-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
