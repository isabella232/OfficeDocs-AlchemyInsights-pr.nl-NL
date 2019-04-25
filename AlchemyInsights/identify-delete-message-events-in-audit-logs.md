---
title: Delete message gebeurtenissen in de controlelogboeken geïdentificeerd
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416705"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="1caa5-102">Controlelogboeken voor verwijderde e-mailberichten</span><span class="sxs-lookup"><span data-stu-id="1caa5-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="1caa5-103">Starten in januari 2019, is Microsoft inschakelen postbus controlelogboeken standaard.</span><span class="sxs-lookup"><span data-stu-id="1caa5-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="1caa5-104">Anders verwijderen bericht om gebeurtenissen te bekijken voor een bepaalde gebruiker, moet u handmatig de delete-acties voor controle inschakelen.</span><span class="sxs-lookup"><span data-stu-id="1caa5-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="1caa5-105">Als postvak controleren registratie al is ingeschakeld voor uw organisatie of voor de specifieke gebruiker, volg de onderstaande stappen.</span><span class="sxs-lookup"><span data-stu-id="1caa5-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="1caa5-106">Log in op de [Office 365 & conformiteit Beveiligingscentrum](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1caa5-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1caa5-107">Klik op **Zoeken en onderzoek** en **Audit-logboek zoeken**selecteren.</span><span class="sxs-lookup"><span data-stu-id="1caa5-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1caa5-108">Selecteer het datumbereik in de velden **begindatum** en **einddatum** .</span><span class="sxs-lookup"><span data-stu-id="1caa5-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1caa5-109">Geef de gebruikersnaam van de gebruiker die u wilt onderzoeken (de gebruiker die de artikelen verwijderd).</span><span class="sxs-lookup"><span data-stu-id="1caa5-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="1caa5-110">Selecteer in het veld **activiteiten** **Verwijderde berichten uit de map Verwijderde Items** en **Moved berichten naar de map Verwijderde Items**.</span><span class="sxs-lookup"><span data-stu-id="1caa5-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="1caa5-111">Klik op **Zoeken**.</span><span class="sxs-lookup"><span data-stu-id="1caa5-111">Click **Search**.</span></span>

<span data-ttu-id="1caa5-112">Selecteer een audit record in de resultaten.</span><span class="sxs-lookup"><span data-stu-id="1caa5-112">In the results, select an audit record.</span></span> <span data-ttu-id="1caa5-113">Klik op **Meer informatie**in het doel details.</span><span class="sxs-lookup"><span data-stu-id="1caa5-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1caa5-114">Meer informatie over het verwijderde item (bijvoorbeeld, de onderwerpregel en de locatie van het item is verwijderd) wordt weergegeven in het veld **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="1caa5-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="1caa5-115">De eigenschap **ClientInfoString** wordt weergegeven als het verwijderen is opgetreden in Outlook, Outlook op het web (voorheen bekend als Outlook Web App) of een ander apparaat.</span><span class="sxs-lookup"><span data-stu-id="1caa5-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="1caa5-116">Zie [vaststellen die e-mail doorsturen voor een postbus instellen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1caa5-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="1caa5-117">**Opmerking**: Verwijderde items met de functie van audit log niet ophalen.</span><span class="sxs-lookup"><span data-stu-id="1caa5-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="1caa5-118">Zie [Verwijderde items in Outlook Web App herstellen](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)voor het ophalen van verwijderde berichten in Outlook op het web.</span><span class="sxs-lookup"><span data-stu-id="1caa5-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
