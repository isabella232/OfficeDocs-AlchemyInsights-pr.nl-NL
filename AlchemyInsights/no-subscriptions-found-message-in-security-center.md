---
title: Geen abonnementen gevonden bericht in het Beveiligingscentrum
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544103"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="3f401-102">Geen abonnementen gevonden bericht in het Beveiligingscentrum</span><span class="sxs-lookup"><span data-stu-id="3f401-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="3f401-103">Als u tijdens het openen van Microsoft Defender-beveiligingscentrum een bericht 'Geen abonnementen gevonden' krijgt, betekent dit dat de Azure Active Directory (AAD) die wordt gebruikt om de gebruiker aan te melden bij de portal, geen Microsoft Defender ATP heeft.</span><span class="sxs-lookup"><span data-stu-id="3f401-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="3f401-104">De Windows E5- en Office E5-licenties zijn afzonderlijke licenties.</span><span class="sxs-lookup"><span data-stu-id="3f401-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="3f401-105">Open een ondersteuningscase als de licentie is aangeschaft, maar niet is ingericht op dit AAD-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="3f401-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="3f401-106">Of u hebt:</span><span class="sxs-lookup"><span data-stu-id="3f401-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="3f401-107">Een mogelijk probleem met het inrichten van licenties.</span><span class="sxs-lookup"><span data-stu-id="3f401-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="3f401-108">U hebt de licentie per ongeluk ingericht op een andere Microsoft AAD dan de licentie die wordt gebruikt voor verificatie in de service.</span><span class="sxs-lookup"><span data-stu-id="3f401-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>