---
title: Problemen met eenmalig aanmelden oplossen voor azure AD-apparaten die lid zijn van Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035466"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="7aeb1-102">Problemen met eenmalig aanmelden oplossen voor azure AD-apparaten die lid zijn van Azure AD</span><span class="sxs-lookup"><span data-stu-id="7aeb1-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="7aeb1-103">Als u een on-premises Ad-omgeving (Active Directory) hebt en u wilt deelnemen aan uw ad-domeincomputers met Azure AD, kunt u dit doen door hybride Azure AD-join te doen.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="7aeb1-104">[How To: Plan your hybrid Azure Active Directory join implementation provides](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="7aeb1-105">Zie Azure [AD-apparaten configureren voor on-premises](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)apparaten Single-Sign Windows Hello voor Bedrijven gebruiken voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="7aeb1-106">**PrT-problemen (Primary Refresh Token)**</span><span class="sxs-lookup"><span data-stu-id="7aeb1-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="7aeb1-107">Een prt (Primary Refresh Token) is een belangrijk artefact van Azure AD-verificatie op Windows 10-, Windows Server 2016- en latere versies, iOS- en Android-apparaten.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="7aeb1-108">Het is een JSON Web Token (JWT) die speciaal is uitgegeven aan microsoft first party token brokers om single sign-on (SSO) in te stellen voor de toepassingen die op deze apparaten worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="7aeb1-109">Zie Wat is een primaire [vernieuwings-token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)voor meer informatie over hoe een PRT wordt uitgegeven, gebruikt en beveiligd op Windows 10-apparaten.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="7aeb1-110">**WamDefaultSet: JA en AzureADPrt: JA**</span><span class="sxs-lookup"><span data-stu-id="7aeb1-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="7aeb1-111">Deze velden geven aan of de gebruiker zich bij het aanmelden bij het apparaat heeft geverifieerd bij Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="7aeb1-112">Als de waarden **NEE zijn,** kan dit het gevolg zijn van:</span><span class="sxs-lookup"><span data-stu-id="7aeb1-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="7aeb1-113">Slechte opslagsleutel in de TPM die bij registratie aan het apparaat is gekoppeld (controleer de KeySignTest tijdens het uitvoeren van verhoogde waarden)</span><span class="sxs-lookup"><span data-stu-id="7aeb1-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="7aeb1-114">Alternatieve aanmeldings-id</span><span class="sxs-lookup"><span data-stu-id="7aeb1-114">Alternate Login ID</span></span>
- <span data-ttu-id="7aeb1-115">HTTP-proxy niet gevonden</span><span class="sxs-lookup"><span data-stu-id="7aeb1-115">HTTP Proxy not found</span></span>

<span data-ttu-id="7aeb1-116">Zie [SSO-status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)als u problemen wilt oplossen met de opdracht dsregcmd.</span><span class="sxs-lookup"><span data-stu-id="7aeb1-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
