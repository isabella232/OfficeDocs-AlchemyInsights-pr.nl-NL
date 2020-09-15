---
title: de 5.7.750-service van 1048 is niet beschikbaar. Client geblokkeerd voor het verzenden van niet-geregistreerde domeinen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664237"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="7d7c4-103">5.7.750-client geblokkeerd voor verzending van niet-geregistreerde domein</span><span class="sxs-lookup"><span data-stu-id="7d7c4-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="7d7c4-104">De fout treedt op wanneer een groot aantal berichten wordt verzonden vanuit domeinen die niet in de Tenant zijn ingericht (toegevoegd als geaccepteerde domeinen en gevalideerd).</span><span class="sxs-lookup"><span data-stu-id="7d7c4-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="7d7c4-105">Om deze fout te voorkomen, kunt u een e-mail stroom verbinding op basis van certificaat gebruiken waarbij het domein van het certificaat een ingerichte domein is, of u kunt alle verzonden domeinen inrichten.</span><span class="sxs-lookup"><span data-stu-id="7d7c4-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
