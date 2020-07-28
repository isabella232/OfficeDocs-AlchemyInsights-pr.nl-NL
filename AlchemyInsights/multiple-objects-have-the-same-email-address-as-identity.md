---
title: Meerdere objecten hebben hetzelfde e-mailadres als identiteit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438932"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Meerdere objecten hebben hetzelfde e-mailadres als identiteit

**Meerdere objecten**

Een van de veelvoorkomende redenen van deze fout is dat u een Outlook Web Access-aanvraag niet goed kan routeren in aanwezigheid van meerdere objecten met hetzelfde e-mailadres als de identiteit. Voer de volgende opdrachten uit om deze objecten te zoeken:

· Ontvanger van get-ontvanger<email address>

· Gebruiker<email address>

· Gebruiker <email address> -SoftDeletedUser

· Contact opnemen<email address>

· Ophalen <email address> -postvak -PublicFolder

· Postvak ophalen <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Als u het probleem wilt oplossen, verwijdert u meerdere objecten met dezelfde e-mailidentiteit en controleert u of er één object is met de specifieke e-mailidentiteit en dat het type ontvanger UserMailbox is.

**Hetzelfde adres wordt gebruikt voor zakelijke en consumentenpostvakken**

Een andere oorzaak is wanneer hetzelfde adres wordt gebruikt voor zakelijke en consumentenpostvakken. In dit geval moet de gebruiker zijn primaire consumentenalias wijzigen totdat Cafe dit scenario ondersteunt. Dit is een permanente fout die niet verdwijnt zonder tussenkomst.

Zie Het [e-mailadres of telefoonnummer voor uw Microsoft-account wijzigen](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)voor meer informatie.