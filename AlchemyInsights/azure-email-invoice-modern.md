---
title: E-mail met modern Azure-facturering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922025"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="a1fb0-102">Facturering via e-mail verzenden in azure</span><span class="sxs-lookup"><span data-stu-id="a1fb0-102">Email invoicing in Azure</span></span>

<span data-ttu-id="a1fb0-103">U kunt de voorkeuren voor de e-mail factuur alleen bijwerken als u een eigenaren of een rol van bijdrage hebt.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="a1fb0-104">Als u zich hebt aangemeld, krijgen alle gebruikers met een eigenaar, Inzender, lezers en factuur Manager-rollen een factuur profiel via e-mail.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="a1fb0-105">Meld u aan bij de [Azure-Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="a1fb0-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a1fb0-106">Zoek naar **kostenbeheer + facturering**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="a1fb0-107">Selecteer **facturen** aan de linkerkant en selecteer vervolgens **e-mail factuur** vanaf de bovenkant van de pagina.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="a1fb0-108">Als u meerdere facturerings profielen hebt, selecteert u een factuur profiel en selecteert u vervolgens **Afmelden**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="a1fb0-109">Selecteer **bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-109">Select **Update**.</span></span>
6. <span data-ttu-id="a1fb0-110">Als u meerdere facturerings profielen hebt, selecteert u een factuur profiel en selecteert u vervolgens **Afmelden**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="a1fb0-111">U geeft anderen toegang tot facturen te bekijken, te downloaden en te betalen door hen de rol van factuur beheerder voor een MCA-of MPA-facturerings profiel toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="a1fb0-112">Als u zich hebt aangemeld om uw factuur via e-mail te verzenden, krijgen gebruikers ook de facturen via e-mail.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="a1fb0-113">Meld u aan bij de [Azure-Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="a1fb0-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a1fb0-114">Zoek naar **kostenbeheer + facturering**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="a1fb0-115">Selecteer **facturerings profielen** aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="a1fb0-116">Selecteer in de lijst facturerings profielen een factuur profiel waarvoor u de rol van factuur beheerder wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="a1fb0-117">Selecteer **toegangsbeheer (IAM)** aan de linkerkant en selecteer vervolgens **toevoegen** vanaf de bovenkant van de pagina.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="a1fb0-118">Selecteer in de vervolgkeuzelijst rollen de optie **factuur Manager**.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="a1fb0-119">Voer het e-mailadres van de gebruiker in om toegang te geven.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="a1fb0-120">Selecteer **Opslaan** om de rol toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="a1fb0-120">Select **Save** to assign the role.</span></span>
