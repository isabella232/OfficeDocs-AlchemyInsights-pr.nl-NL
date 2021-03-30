---
title: Problemen met Azure AD-join oplossen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404630"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="340d6-102">Problemen met Azure AD-join oplossen</span><span class="sxs-lookup"><span data-stu-id="340d6-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="340d6-103">Als u apparaatregistraties voor het eerst instelt, controleert u of u Inleiding tot apparaatbeheer hebt bekeken [in Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) die u begeleidt bij het instellen van Apparaten onder het besturingselement naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="340d6-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="340d6-104">Als u apparaten rechtstreeks registreert bij Azure AD en deze registreert bij Intune, moet u ervoor zorgen dat u [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) hebt geconfigureerd en de licentie eerst [hebt](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) ingesteld.</span><span class="sxs-lookup"><span data-stu-id="340d6-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="340d6-105">Controleer of u gemachtigd bent om bewerkingen uit te voeren in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="340d6-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="340d6-106">Alleen een globale beheerder in Azure AD kan instellingen voor apparaatregistraties beheren.</span><span class="sxs-lookup"><span data-stu-id="340d6-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="340d6-107">Zie Azure AD Join plannen als u azure AD join [wilt implementeren.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="340d6-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="340d6-108">Zie Veelgestelde vragen over [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) en voor Windows 10 Pro-apparaat voor meer informatie over het oplossen van veelvoorkomende problemen met Azure AD-join. Zie Kan niet deelnemen aan Windows [10 Pro-computer](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) met Azure AD - Moet upgraden naar - Microsoft Community</span><span class="sxs-lookup"><span data-stu-id="340d6-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
