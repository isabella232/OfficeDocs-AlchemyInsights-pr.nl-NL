---
title: Aangepaste meldingen met intune verzenden
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720641"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="ecd26-102">Aangepaste meldingen verzenden naar de gebruikers van beheerde iOS-en Android-apparaten</span><span class="sxs-lookup"><span data-stu-id="ecd26-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="ecd26-103">Aangepaste meldingen voor intune worden verwerkt door de bedrijfs portal-app op het apparaat van een gebruiker.</span><span class="sxs-lookup"><span data-stu-id="ecd26-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="ecd26-104">Vervolgens maakt de app een pushbericht op dat apparaat.</span><span class="sxs-lookup"><span data-stu-id="ecd26-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="ecd26-105">Hieronder ziet u de vereisten voor het inschakelen van de ontvangst van aangepaste meldingen en voor de app moet u vervolgens de push melding maken:</span><span class="sxs-lookup"><span data-stu-id="ecd26-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="ecd26-106">Op het apparaat moet de bedrijfs portal-app zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="ecd26-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="ecd26-107">Op het toestel moet de bedrijfs portal-app pushmeldingen verzenden.</span><span class="sxs-lookup"><span data-stu-id="ecd26-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="ecd26-108">Wanneer de app is geïnstalleerd of bijgewerkt, wordt de gebruiker gevraagd om meldingen toe te staan.</span><span class="sxs-lookup"><span data-stu-id="ecd26-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="ecd26-109">Op Android-apparaten moeten Google play-services zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="ecd26-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="ecd26-110">Het apparaat moet zijn geregistreerd met intune.</span><span class="sxs-lookup"><span data-stu-id="ecd26-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="ecd26-111">Zie de [documentatie bij de functie](https://docs.microsoft.com/intune/custom-notifications)voor meer informatie over het verzenden van een bericht.</span><span class="sxs-lookup"><span data-stu-id="ecd26-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
