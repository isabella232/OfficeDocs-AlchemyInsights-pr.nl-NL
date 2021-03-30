---
title: Single-Sign voor apparaten met azure Active Directory-apparaten
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404590"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="c58f8-102">Eén aanmelding voor azure Active Directory-apparaten</span><span class="sxs-lookup"><span data-stu-id="c58f8-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="c58f8-103">Als u een on-premises Ad-omgeving (Active Directory) hebt en u wilt deelnemen aan uw ad-domeincomputers met Azure AD, kunt u dit doen door hybride Azure AD-join te doen.</span><span class="sxs-lookup"><span data-stu-id="c58f8-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="c58f8-104">[How To: Plan your hybrid Azure Active Directory join implementation provides](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="c58f8-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="c58f8-105">Azure AD-apparaten configureren voor on-premises Single-Sign On using Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="c58f8-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="c58f8-106">**PrT-problemen (Primary Refresh Token)** Een prt (Primary Refresh Token) is een belangrijk artefact van Azure AD-verificatie op Windows 10-, Windows Server 2016- en latere versies, iOS- en Android-apparaten.</span><span class="sxs-lookup"><span data-stu-id="c58f8-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="c58f8-107">Het is een JSON Web Token (JWT) die speciaal is uitgegeven aan microsoft first party token brokers om single sign-on (SSO) in te stellen voor de toepassingen die op deze apparaten worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="c58f8-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="c58f8-108">[In Wat is een primaire vernieuwings-token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)geven we informatie over hoe een PRT wordt uitgegeven, gebruikt en beveiligd op Windows 10-apparaten.</span><span class="sxs-lookup"><span data-stu-id="c58f8-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="c58f8-109">**WamDefaultSet: JA en AzureADPrt: JA** Deze velden geven aan of de gebruiker zich bij het aanmelden bij het apparaat heeft geverifieerd bij Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c58f8-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="c58f8-110">Als de waarden **NEE zijn,** kan dit een gevolg zijn:</span><span class="sxs-lookup"><span data-stu-id="c58f8-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="c58f8-111">Slechte opslagsleutel in de TPM die bij registratie aan het apparaat is gekoppeld (controleer de KeySignTest tijdens het uitvoeren van verhoogde waarden).</span><span class="sxs-lookup"><span data-stu-id="c58f8-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="c58f8-112">Alternatieve aanmeldings-id</span><span class="sxs-lookup"><span data-stu-id="c58f8-112">Alternate Login ID</span></span>
- <span data-ttu-id="c58f8-113">HTTP-proxy niet gevonden</span><span class="sxs-lookup"><span data-stu-id="c58f8-113">HTTP Proxy not found</span></span>

<span data-ttu-id="c58f8-114">Problemen met apparaten oplossen met de opdracht dsregcmd - [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="c58f8-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
