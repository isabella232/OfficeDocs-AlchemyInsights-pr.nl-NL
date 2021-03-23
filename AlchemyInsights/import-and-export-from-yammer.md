---
title: Importeren en exporteren vanuit Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035439"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="eb9e8-102">Importeren en exporteren vanuit Yammer</span><span class="sxs-lookup"><span data-stu-id="eb9e8-102">Import and export from Yammer</span></span>

<span data-ttu-id="eb9e8-103">**Importeren**</span><span class="sxs-lookup"><span data-stu-id="eb9e8-103">**Import**</span></span>

<span data-ttu-id="eb9e8-104">Opties voor het importeren van gebruikers variëren, afhankelijk van of uw Yammer-netwerk zich in de native modus voor [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)of niet.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="eb9e8-105">**Niet-native modus:** Gebruikers kunnen worden geïmporteerd in groepen met [Behulp](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) van Toevoegen uit adresboek (limiet tot 100 gebruikers) binnen groepsinstellingen of in het netwerk met [bulkupdate](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) binnen netwerkbeheerder.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="eb9e8-106">**Native Mode:** Activiteiten voor lidmaatschap van groepen en lidmaatschap van netwerken moeten worden uitgevoerd vanuit de [Microsoft 365-beheerportal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD-portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)of met een andere Azure AD-optie.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="eb9e8-107">Netwerken in de autochtone modus hebben geen toegang meer tot Bulkupdate en andere oudere functies.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="eb9e8-108">Yammer heeft het importeren van inhoud vanuit netwerkbeheerder nooit ondersteund, zelfs niet wanneer de functie Gegevens exporteren werd gebruikt in een ander netwerk.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="eb9e8-109">Inhoud kan opnieuw worden gepost door partneroplossingen of de Yammer REST-API's.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="eb9e8-110">**Exporteren**</span><span class="sxs-lookup"><span data-stu-id="eb9e8-110">**Export**</span></span>

<span data-ttu-id="eb9e8-111">[Als u netwerkgegevens exporteert binnen netwerkbeheerder,](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) kan inhoud uit Yammer-netwerken worden geëxporteerd, inclusief berichten en bestanden.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="eb9e8-112">Bijlagen kunnen zeer groot zijn en de uitvoer kan veel tijd in beslag nemen.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="eb9e8-113">Het is raadzaam actieve netwerken te exporteren met behulp van de [Data Export API](https://developer.yammer.com/docs/data-export-api) in segmenten per dag of week.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="eb9e8-114">Microsoft Support biedt hiervoor geen aangepaste scripts.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="eb9e8-115">Er bestaat [een aparte AVG-export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) om inhoud voor een afzonderlijke gebruiker te exporteren.</span><span class="sxs-lookup"><span data-stu-id="eb9e8-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>