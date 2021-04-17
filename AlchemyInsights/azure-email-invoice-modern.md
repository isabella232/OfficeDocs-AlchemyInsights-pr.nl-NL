---
title: Moderne facturering per e-mail in Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820821"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="c854e-102">Facturering per e-mail in Azure</span><span class="sxs-lookup"><span data-stu-id="c854e-102">Email invoicing in Azure</span></span>

<span data-ttu-id="c854e-103">U moet een rol van eigenaar of inzender hebben in het factureringsprofiel of het factureringsaccount om de voorkeur voor e-mailfacturen bij te werken.</span><span class="sxs-lookup"><span data-stu-id="c854e-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="c854e-104">Zodra u zich heeft aangemeld, ontvangen alle gebruikers met de rol van eigenaar, inzender, lezer of factuurbeheerder in een factureringsprofiel de factuur per e-mail.</span><span class="sxs-lookup"><span data-stu-id="c854e-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="c854e-105">Meld u aan bij de [Microsoft Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c854e-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="c854e-106">Zoek naar **Kostenbeheer en facturering**.</span><span class="sxs-lookup"><span data-stu-id="c854e-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="c854e-107">Selecteer **Facturen** aan de linkerkant en selecteer vervolgens **Factuur per e-mail verzenden** bovenaan de pagina.</span><span class="sxs-lookup"><span data-stu-id="c854e-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="c854e-108">Als u meerdere factureringsprofielen hebt, selecteert u een factureringsprofiel en selecteert u **Aanmelden**.</span><span class="sxs-lookup"><span data-stu-id="c854e-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="c854e-109">Selecteer **Bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="c854e-109">Select **Update**.</span></span>
6. <span data-ttu-id="c854e-110">Als u meerdere factureringsprofielen hebt, selecteert u een factureringsprofiel en selecteert u **Aanmelden**.</span><span class="sxs-lookup"><span data-stu-id="c854e-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="c854e-111">U geeft anderen toegang om facturen te bekijken, te downloaden en te betalen door hun de rol van factuurmanager voor een MCA- of MPA-factureringsprofiel toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="c854e-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="c854e-112">Als u ervoor hebt gekozen om uw factuur per e-mail te ontvangen, ontvangen gebruikers de facturen ook per e-mail.</span><span class="sxs-lookup"><span data-stu-id="c854e-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="c854e-113">Meld u aan bij de [Microsoft Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c854e-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="c854e-114">Zoek naar **Kostenbeheer en facturering**.</span><span class="sxs-lookup"><span data-stu-id="c854e-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="c854e-115">Selecteer **Factureringsprofielen** aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="c854e-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="c854e-116">Selecteer in de lijst met factureringsprofielen een factureringsprofiel waaraan u een rol van factuurmanager wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="c854e-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="c854e-117">Selecteer **Toegangsbeheer (IAM)** aan de linkerkant en selecteer vervolgens **Toevoegen** aan de bovenkant van de pagina.</span><span class="sxs-lookup"><span data-stu-id="c854e-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="c854e-118">Selecteer in de vervolgkeuzelijst Rol de optie **Factuurbeheer**.</span><span class="sxs-lookup"><span data-stu-id="c854e-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="c854e-119">Voer het e-mailadres van de gebruiker in om toegang te verlenen.</span><span class="sxs-lookup"><span data-stu-id="c854e-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="c854e-120">Selecteer **Opslaan** om de rol toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="c854e-120">Select **Save** to assign the role.</span></span>
