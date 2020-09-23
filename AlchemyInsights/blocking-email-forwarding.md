---
title: 726 blokkeert het doorsturen van e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219850"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="0f707-102">Doorsturen van e-mail blokkeren of de blokkering opheffen</span><span class="sxs-lookup"><span data-stu-id="0f707-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="0f707-103">Zie [doorsturen van E-mail configureren](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)om het doorsturen van e-mail voor een specifiek postvak in of uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="0f707-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="0f707-104">Op het tenantniveau wordt de besturing van extern doorsturen uitgevoerd met behulp van het uitgaande antispambeleid.</span><span class="sxs-lookup"><span data-stu-id="0f707-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="0f707-105">Als de instelling op uit of automatisch is ingesteld, kan het doorsturen van e-mail blokkeren met de fout ' 550 5.7.520 toegang geweigerd ' wordt niet toegestaan dat uw organisatie de fout externe forwarding toestaat '.</span><span class="sxs-lookup"><span data-stu-id="0f707-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="0f707-106">Als doorsturen is ingesteld op geblokkeerd, is dit de fout die uw gebruikers te zien krijgen.</span><span class="sxs-lookup"><span data-stu-id="0f707-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="0f707-107">Als het doorsturen wordt geblokkeerd, controleert u of het beleid is geconfigureerd voor het inschakelen van extern doorsturen.</span><span class="sxs-lookup"><span data-stu-id="0f707-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="0f707-108">U kunt het uitgaande spam filter beleid controleren vanuit beveiligings-en compliance Center, of door opdracht Get-HostedOutboundSpamFilterPolicy | FL name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="0f707-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="0f707-109">Als u de optie voor het doorsturen van e-mail wilt instellen, krijgt u de status van beleid nu te zien.</span><span class="sxs-lookup"><span data-stu-id="0f707-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="0f707-110">Opmerking: het wordt aanbevolen dat u de functie voor extern doorsturen uitgeschakeld laat voor het standaardbeleid voor uitgaande spam filters en dit alleen inschakelen voor de gebruikers die extern doorsturen willen maken door een aangepast beleid te maken voor deze gebruikers.</span><span class="sxs-lookup"><span data-stu-id="0f707-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="0f707-111">Meer informatie vindt u in [externe e-mail forwarding configureren in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="0f707-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>