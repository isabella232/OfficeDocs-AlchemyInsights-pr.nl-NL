---
title: Active Directory wordt niet gesynchroniseerd
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314199"
---
# <a name="active-directory-not-syncing"></a>Active Directory wordt niet gesynchroniseerd

Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie', of als u ziet dat de adreslijstsynchronisatiestatus in de beheerportal van Office zegt: 'Laatst gesynchroniseerd meer dan 3 dagen geleden', kan het zijn dat AADConnect onjuiste instellingen of onvoldoende machtigingen heeft om een synchronisatie uit te voeren.  

Als u AADConnect opnieuw installeert met behulp van express-instellingen, kan het probleem snel worden opgelost:

1. [Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Volg de instructies voor het snel installeren.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect moet worden geïnstalleerd op Windows Server 2012 of hoger. Deze server moet lid zijn van een domein en kan een domeincontroller of een lidserver zijn. Controleer Vereisten voor Azure AD-Verbinding maken voor een volledige lijst met vereisten en vereisten voor [Azure AD-Verbinding maken.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Zie [Azure AD-Verbinding maken: Accounts en machtigingen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.
