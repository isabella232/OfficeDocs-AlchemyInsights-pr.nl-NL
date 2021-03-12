---
title: Veelvoorkomende problemen met DKIM-recordopmaak oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744886"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="42071-102">Veelvoorkomende problemen met DKIM-recordopmaak oplossen</span><span class="sxs-lookup"><span data-stu-id="42071-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="42071-103">De meeste DKIM-instellingen zijn gerelateerd aan onjuiste DNS-records.</span><span class="sxs-lookup"><span data-stu-id="42071-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="42071-104">Als u de DKIM-set-upproblemen wilt oplossen, controleert u of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt.</span><span class="sxs-lookup"><span data-stu-id="42071-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="42071-105">Zie Wat u moet doen om DKIM handmatig in te stellen [in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="42071-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="42071-106">Zie DNS-records maken bij een [DNS-hostingprovider voor Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)als u hulp nodig hebt bij DNS-records in het algemeen.</span><span class="sxs-lookup"><span data-stu-id="42071-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="42071-107">Nadat u uw DKIM DNS-records bij de DNS-hostingservice voor uw domein hebt gemaakt of bijgewerkt, moet u wachten totdat de DNS-records worden doorgegeven.</span><span class="sxs-lookup"><span data-stu-id="42071-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
