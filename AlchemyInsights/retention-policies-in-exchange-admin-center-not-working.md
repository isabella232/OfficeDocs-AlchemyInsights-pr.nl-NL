---
title: Bewaarbeleid in Exchange-beheercentrum werkt niet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952223"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9a238-102">Bewaarbeleid in exchange-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="9a238-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="9a238-103">Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de knop Terug < boven aan deze pagina en voert u vervolgens het e-mailadres in van de gebruiker die problemen heeft met bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="9a238-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="9a238-104">Als u problemen hebt met bewaarbeleid in het Exchange-beheercentrum dat niet van toepassing is op postvakken of items die niet naar het archiefpostvak worden verplaatst, controleert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="9a238-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="9a238-105">**Hoofdoorzaken:**</span><span class="sxs-lookup"><span data-stu-id="9a238-105">**Root Causes:**</span></span>

- <span data-ttu-id="9a238-106">**Beheerde mapassistent** heeft het postvak van de gebruiker niet verwerkt.</span><span class="sxs-lookup"><span data-stu-id="9a238-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9a238-107">Met de assistent voor beheerde mappen wordt geprobeerd om elk postvak in uw cloudorganisatie eens in de zeven dagen te verwerken.</span><span class="sxs-lookup"><span data-stu-id="9a238-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="9a238-108">**Oplossing:** Voer de assistent beheerde map uit.</span><span class="sxs-lookup"><span data-stu-id="9a238-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="9a238-109">**RetentionHold** is **ingeschakeld** in het postvak.</span><span class="sxs-lookup"><span data-stu-id="9a238-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9a238-110">Als het postvak is geplaatst op een Bewaarbewaring, wordt het bewaarbeleid voor het postvak in die periode niet verwerkt.</span><span class="sxs-lookup"><span data-stu-id="9a238-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="9a238-111">**Oplossing:** Controleer de status van bewaringsinstelling en werk zo nodig bij.</span><span class="sxs-lookup"><span data-stu-id="9a238-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="9a238-112">Zie Bewaring van [postvak voor meer informatie.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="9a238-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="9a238-113">**Opmerking:** Als een postvak kleiner is dan 10 MB, wordt het postvak niet automatisch verwerkt door de Assistent voor beheerde mappen.</span><span class="sxs-lookup"><span data-stu-id="9a238-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9a238-114">Zie voor meer informatie over bewaarbeleid in het Exchange-beheercentrum:</span><span class="sxs-lookup"><span data-stu-id="9a238-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="9a238-115">Bewaarlabels en bewaarbeleid</span><span class="sxs-lookup"><span data-stu-id="9a238-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="9a238-116">[Een bewaarbeleid toepassen op postvakken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) of [bewaarlabels toevoegen of verwijderen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="9a238-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="9a238-117">Het type bewaring voor een postvak identificeren</span><span class="sxs-lookup"><span data-stu-id="9a238-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
