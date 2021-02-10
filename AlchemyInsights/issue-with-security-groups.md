---
title: Probleem met beveiligingsgroepen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177420"
---
# <a name="issue-with-security-groups"></a>Probleem met beveiligingsgroepen

**Als u netwerkfout AADDS104 krijgt**

Ongeldige regels van de netwerkbeveiligingsgroep zijn de meest voorkomende oorzaak van netwerkfouten voor Azure Active Directory Domain Services (AD DS). De netwerkbeveiligingsgroep voor het virtuele netwerk moet toegang verlenen tot bepaalde poorten en protocollen. Als deze poorten worden geblokkeerd, kan het Azure-platform het beheerde domein niet controleren of bijwerken. De synchronisatie tussen Azure AD en Azure AD DS wordt ook beïnvloed. Zorg ervoor dat de standaardpoorten open blijven om onderbreking van de service te voorkomen.

Zie Beveiligingsgroepen toevoegen en controleren voor algemene waarschuwingen voor configuratieproblemen van netwerkbeveiligingsgroepen en [deze op te lossen.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
