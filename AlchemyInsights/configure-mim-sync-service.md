---
title: MIM-synchronisatieservice configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481354"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="0f722-102">MIM-synchronisatieservice configureren</span><span class="sxs-lookup"><span data-stu-id="0f722-102">Configure MIM Sync service</span></span>

<span data-ttu-id="0f722-103">Microsoft Identity Manager (MIM) Synchronization Service is een onderdeel van MIM.</span><span class="sxs-lookup"><span data-stu-id="0f722-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="0f722-104">Het is een centrale on-premises service die informatie opgeslagen en integreert voor organisaties met meerdere on-premises directories en databases.</span><span class="sxs-lookup"><span data-stu-id="0f722-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="0f722-105">U kunt het probleem met MIM-synchronisatie mogelijk oplossen als het probleem is opgelost in een recente update voor MIM of een van de andere problemen is die in de onderstaande sectie worden genoemd.</span><span class="sxs-lookup"><span data-stu-id="0f722-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="0f722-106">**Aanbevolen stappen**</span><span class="sxs-lookup"><span data-stu-id="0f722-106">**Recommended steps**</span></span>

1. <span data-ttu-id="0f722-107">Controleer of u een recente update van MIM Sync gebruikt en bekijk de opmerkingen bij de [release van MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) om te bepalen of het probleem is opgelost in een update.</span><span class="sxs-lookup"><span data-stu-id="0f722-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="0f722-108">Als het probleem wordt veroorzaakt door de connector Generic LDAP, Generic SQL, Lotus Domino of Web Services, controleert u of u een recente update van de [algemene connectors gebruikt.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="0f722-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="0f722-109">Als een MIM Sync-run stopt met een fout, raadpleegt u de tabel met run error [codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) om de mogelijke oorzaken te bepalen.</span><span class="sxs-lookup"><span data-stu-id="0f722-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="0f722-110">Als het uitvoeren stopt met een **uitbreidings-DLL-uitzondering,** klikt u op die woorden om het venster Eigenschappen van verbindingsruimteobject te openen en klikt u op Stapel **traceren...** voor meer informatie over de onderliggende oorzaak, zoals wordt beschreven in [Uitbreiding-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) </span><span class="sxs-lookup"><span data-stu-id="0f722-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="0f722-111">Als het pcns-onderdeel (Password Change Notification Service) fout **6025** in het gebeurtenislogboek meldt tijdens wachtwoordsynchronisatie, raadpleegt u de handleiding voor het oplossen van problemen met [pcns-rapportagefout 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="0f722-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="0f722-112">Als de volledige synchronisatie met de FIM Service  Management Agent traag is, controleert u of de instelling voor automatisch groeien is vertraagd voor TempDB, zoals is beschreven in Problemen met trage of hangende volledige [synchronisatie.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="0f722-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="0f722-113">Als u een fout ziet van een gestopte server met failed-creation-via-web-services met behulp van de FIM Service Management Agent, bekijkt u [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) voor een overzicht van de oorzaken.</span><span class="sxs-lookup"><span data-stu-id="0f722-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

