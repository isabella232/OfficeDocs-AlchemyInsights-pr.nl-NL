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
# <a name="import-and-export-from-yammer"></a>Importeren en exporteren vanuit Yammer

**Importeren**

Opties voor het importeren van gebruikers variëren, afhankelijk van of uw Yammer-netwerk zich in de native modus voor [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)of niet.

- **Niet-native modus:** Gebruikers kunnen worden geïmporteerd in groepen met [Behulp](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) van Toevoegen uit adresboek (limiet tot 100 gebruikers) binnen groepsinstellingen of in het netwerk met [bulkupdate](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) binnen netwerkbeheerder.
- **Native Mode:** Activiteiten voor lidmaatschap van groepen en lidmaatschap van netwerken moeten worden uitgevoerd vanuit de [Microsoft 365-beheerportal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD-portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)of met een andere Azure AD-optie. Netwerken in de autochtone modus hebben geen toegang meer tot Bulkupdate en andere oudere functies.

> [!IMPORTANT]
> Yammer heeft het importeren van inhoud vanuit netwerkbeheerder nooit ondersteund, zelfs niet wanneer de functie Gegevens exporteren werd gebruikt in een ander netwerk. Inhoud kan opnieuw worden gepost door partneroplossingen of de Yammer REST-API's.

**Exporteren**

[Als u netwerkgegevens exporteert binnen netwerkbeheerder,](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) kan inhoud uit Yammer-netwerken worden geëxporteerd, inclusief berichten en bestanden. Bijlagen kunnen zeer groot zijn en de uitvoer kan veel tijd in beslag nemen. Het is raadzaam actieve netwerken te exporteren met behulp van de [Data Export API](https://developer.yammer.com/docs/data-export-api) in segmenten per dag of week. Microsoft Support biedt hiervoor geen aangepaste scripts.

Er bestaat [een aparte AVG-export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) om inhoud voor een afzonderlijke gebruiker te exporteren.