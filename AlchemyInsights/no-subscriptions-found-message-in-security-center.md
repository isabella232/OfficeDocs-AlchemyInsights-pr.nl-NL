---
title: Bericht Geen abonnementen gevonden in het Beveiligingscentrum
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713600"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="39d6a-102">Bericht Geen abonnementen gevonden in het Beveiligingscentrum</span><span class="sxs-lookup"><span data-stu-id="39d6a-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="39d6a-103">Als u tijdens het openen van het Microsoft Defender-beveiligingscentrum het bericht 'Geen abonnementen gevonden' ziet, betekent dit dat azure Active Directory (AAD) waarmee de gebruiker zich bij de portal heeft aanmelden, geen Microsoft Defender ATP-licentie heeft.</span><span class="sxs-lookup"><span data-stu-id="39d6a-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="39d6a-104">De licenties voor Windows E5 en Office E5 zijn afzonderlijke licenties.</span><span class="sxs-lookup"><span data-stu-id="39d6a-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="39d6a-105">Open een ondersteuningscase als de licentie is gekocht, maar niet is ingericht voor dit AAD-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="39d6a-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="39d6a-106">U hebt:</span><span class="sxs-lookup"><span data-stu-id="39d6a-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="39d6a-107">Een mogelijk probleem met het inrichten van licenties.</span><span class="sxs-lookup"><span data-stu-id="39d6a-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="39d6a-108">U hebt de licentie per ongeluk ingericht op een ander Microsoft AAD-nummer dan de licentie die voor verificatie in de service is gebruikt.</span><span class="sxs-lookup"><span data-stu-id="39d6a-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>