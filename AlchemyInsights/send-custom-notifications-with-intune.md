---
title: Aangepaste meldingen verzenden met intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886852"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="e094b-102">Aangepaste meldingen verzenden naar gebruikers van beheerde iOS-en Android-apparaten</span><span class="sxs-lookup"><span data-stu-id="e094b-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="e094b-103">Aangepaste meldingen voor intune worden verwerkt door de bedrijfs portal-app op het apparaat van een gebruiker.</span><span class="sxs-lookup"><span data-stu-id="e094b-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="e094b-104">De app maakt vervolgens de pushmelding op dat apparaat.</span><span class="sxs-lookup"><span data-stu-id="e094b-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="e094b-105">De volgende zijn apparaatvereisten ter ondersteuning van de ontvangst van aangepaste meldingen en voor de app vervolgens de pushmelding maken:</span><span class="sxs-lookup"><span data-stu-id="e094b-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="e094b-106">Het apparaat moet de bedrijfs portal-app hebben geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="e094b-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="e094b-107">Het apparaat moet de bedrijfs portal-app toestaan om pushmeldingen te verzenden.</span><span class="sxs-lookup"><span data-stu-id="e094b-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="e094b-108">Wanneer de app is geïnstalleerd of bijgewerkt, wordt de gebruiker gevraagd om meldingen toe te staan.</span><span class="sxs-lookup"><span data-stu-id="e094b-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="e094b-109">Op Android-apparaten moeten Google play-services zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="e094b-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="e094b-110">Het apparaat moet zijn geregistreerd bij intune.</span><span class="sxs-lookup"><span data-stu-id="e094b-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="e094b-111">Zie de documentatie bij de [functie](https://docs.microsoft.com/intune/custom-notifications)voor meer informatie, zoals het verzenden van een bericht.</span><span class="sxs-lookup"><span data-stu-id="e094b-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
