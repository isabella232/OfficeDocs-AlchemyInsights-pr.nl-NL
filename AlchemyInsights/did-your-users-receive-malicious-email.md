---
title: Hebben jouw gebruikers een schadelijke e-mail ontvangen
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291787"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="0e438-102">Hebben jouw gebruikers een schadelijke e-mail ontvangen?</span><span class="sxs-lookup"><span data-stu-id="0e438-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="0e438-103">Je kunt de schadelijke e-mail nu rapporteren aan Microsoft via [Inzendingen van beheerder in het Beveiligings- en compliancecentrum](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="0e438-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="0e438-104">Berichten die zijn verzonden via [inzendingen van beheerder](https://sip.protection.office.com/reportsubmission) worden gescand en de volgende resultaten worden weergegeven in de **details**-flyout:</span><span class="sxs-lookup"><span data-stu-id="0e438-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="0e438-105">Of er tijdens de levering een fout zat in de e-mailverificatie van de afzender.</span><span class="sxs-lookup"><span data-stu-id="0e438-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="0e438-106">Informatie over eventuele beleidstreffers die het oordeel over een bericht kunnen hebben beïnvloed of overschreven.</span><span class="sxs-lookup"><span data-stu-id="0e438-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="0e438-107">Huidige deactiveringsresultaten om te zien of de URL's of bestanden in het bericht schadelijk waren of niet.</span><span class="sxs-lookup"><span data-stu-id="0e438-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="0e438-108">Feedback van beoordelaars</span><span class="sxs-lookup"><span data-stu-id="0e438-108">Feedback from graders</span></span>

<span data-ttu-id="0e438-109">Als een overschrijving is gevonden, zou het opnieuw scannen in enkele minuten moeten zijn voltooid.</span><span class="sxs-lookup"><span data-stu-id="0e438-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="0e438-110">Als er geen probleem met de e-mailverificatie was of de levering niet werd beïnvloed door een overschrijving, kan de feedback van beoordelaars maximaal een dag duren.</span><span class="sxs-lookup"><span data-stu-id="0e438-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="0e438-111">Als je het niet eens bent met het uiteindelijke oordeel over een bericht, URL of bestand (geblokkeerd of niet geblokkeerd), dien het bericht dan na een dag opnieuw in voor een nieuwe scan.</span><span class="sxs-lookup"><span data-stu-id="0e438-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="0e438-112">De kans is groot dat het oordeel verandert nadat je het bericht opnieuw hebt ingediend.</span><span class="sxs-lookup"><span data-stu-id="0e438-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="0e438-113">Ondertussen kun je schadelijke e-mail verwijderen uit het postvak IN van gebruikers met behulp van de instructies in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="0e438-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="0e438-114">Klanten met Microsoft Defender voor Office 365 kunnen:</span><span class="sxs-lookup"><span data-stu-id="0e438-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="0e438-115">de [Bedreigingsverkenner gebruiken om verdachte e-mails te zoeken en te verwijderen](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="0e438-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="0e438-116">[Veilige koppelingen gebruiken om de toegang tot een schadelijke URL te blokkeren](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)</span><span class="sxs-lookup"><span data-stu-id="0e438-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="0e438-117">gebruikers volgen die op schadelijke URL's hebben geklikt en deze hebben geopend: [bekijk de phishing-URL en klik op oordeelgegevens](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="0e438-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="0e438-118">handmatig [een geautomatiseerd onderzoek starten](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="0e438-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="0e438-119">Je kunt ook beveiligen tegen schadelijke bestanden en URL's door de instructies te volgen in [Beveiligen tegen schadelijke URL's en bestanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="0e438-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>