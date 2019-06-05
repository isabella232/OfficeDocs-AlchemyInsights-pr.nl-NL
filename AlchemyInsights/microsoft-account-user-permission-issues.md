---
title: Maken en gebruiken van een gedeeld postvak
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717342"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Oplossen van probleem - gebruiker is niet gevonden in de directory

<p>Als gebruikers het foutbericht <strong>ontvangen &ldquo; &hellip;gebruiker kan&rsquo;t in de directory worden gevonden. Probeer het opnieuw&hellip; </strong> waarbij het Type probleem is <strong> &ldquo;gebruiker niet in map.&rdquo;</strong>, de volgende stappen uit voor het oplossen van het probleem kunnen worden voltooid.</p> <ol> <li>Controleer de account die de e-mailuitnodiging dezelfde account die wordt gebruikt voor het later inloggen is geaccepteerd. Zorg ervoor dat de gebruiker de uitnodiging accepteren en inloggen op de site gebruikt dezelfde account. <br /><br />Voor meer info Zie <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">aliassen voor uw Microsoft-account beheren</a> voor het beheren van de aanmelding voor Office 365. <br /><br /></li> <li>Ga naar elke site (s) waarin de fout wordt ontvangen van de gebruiker. <br /><br />een. Voeg toe <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (tussen de dubbele aanhalingstekens) aan het einde van de URL van de site. <br /><br />Voorbeeld: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Selecteer de gebruiker uit de lijst. <br /><br />c. Klik op <strong>gebruikersmachtigingen vanuit het lint te verwijderen</strong>. <br /><br />d. Toevoegen van de gebruiker en de uitnodiging te verzenden naar de gebruiker.</li> </ol>

