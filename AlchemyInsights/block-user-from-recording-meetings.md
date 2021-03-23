---
title: Gebruiker blokkeren bij het opnemen van vergaderingen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035367"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="0ac84-102">Gebruiker blokkeren bij het opnemen van vergaderingen</span><span class="sxs-lookup"><span data-stu-id="0ac84-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="0ac84-103">Als u wilt voorkomen **of blokkeren dat** specifieke gebruikers Teams-vergaderingen opnemen, kunt u dit doen via de instellingen voor teamsvergaderingsbeleid.</span><span class="sxs-lookup"><span data-stu-id="0ac84-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="0ac84-104">Schakel in het Microsoft Teams-beheercentrum de instelling **Cloudopname** toestaan uit in het vergaderingsbeleid dat aan die gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="0ac84-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="0ac84-105">Zie Vergaderingsbeleid [beheren in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0ac84-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="0ac84-106">Als u wilt valideren of een specifieke gebruiker wel of niet teamsvergaderingen mag opnemen, gebruikt u de diagnostische ondersteuning.</span><span class="sxs-lookup"><span data-stu-id="0ac84-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="0ac84-107">Voer een nieuwe ondersteuningsquery uit en typ **diag:** opname van vergadering: de diagnostische instelling controleert de beleidsinstellingen voor de opgegeven gebruiker en bepaalt de beleidsinstellingen.</span><span class="sxs-lookup"><span data-stu-id="0ac84-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="0ac84-108">Houd er rekening mee dat het enkele uren kan duren voordat nieuwe beleidsinstellingen van kracht worden. Als u zojuist een wijziging hebt aangebracht, wacht u een paar uur voordat u de diagnostische gegevens opnieuw kunt uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="0ac84-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="0ac84-109">Voor meer informatie bekijkt u [Cloudopname in- of uitschakelen.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="0ac84-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
