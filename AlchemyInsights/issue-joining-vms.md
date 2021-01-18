---
title: Problemen bij het samenvoegen van VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884978"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="58602-102">Problemen bij het samenvoegen van VMs</span><span class="sxs-lookup"><span data-stu-id="58602-102">Issue joining VMs</span></span>

<span data-ttu-id="58602-103">Voer de volgende stappen uit als u problemen wilt oplossen die zich voordoen tijdens het bijwonen van Vm's.</span><span class="sxs-lookup"><span data-stu-id="58602-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="58602-104">Probeer u aan te melden met de **UPN** -indeling (bijvoorbeeld ' joeuser@contoso.com ') in plaats van de **SAMAccountName** -indeling (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="58602-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="58602-105">Zorg ervoor dat u Wachtwoordsynchronisatie hebt ingeschakeld in overeenstemming met de stappen die worden beschreven in de handleiding *aan* de slag.</span><span class="sxs-lookup"><span data-stu-id="58602-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="58602-106">Zorg ervoor dat het desbetreffende gebruikersaccount geen extern account is in de Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="58602-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="58602-107">Externe gebruikers kunnen zich niet aanmelden bij het beheerde domein, aangezien Azure AD Domain Services geen referenties hebben voor dergelijke gebruikersaccounts.</span><span class="sxs-lookup"><span data-stu-id="58602-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="58602-108">Als het desbetreffende gebruikersaccount een gebruikersaccount van de Cloud is, moet u ervoor zorgen dat gebruikers hun wachtwoord wijzigen nadat u Azure AD Domain Services hebt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="58602-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="58602-109">Met deze stap worden de referenties voor de referenties van Azure AD Domain Services gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="58602-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="58602-110">Als de desbetreffende gebruikersaccounts worden gesynchroniseerd vanuit een on-premises adreslijst, controleert u of de aanbevolen versie van Azure AD Connect is geconfigureerd om een volledige synchronisatie uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="58602-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="58602-111">Als het probleem zich blijft voordoen nadat u stap 4 hebt bevestigd, voert u de volgende opdrachten uit op uw synchronisatie computer:</span><span class="sxs-lookup"><span data-stu-id="58602-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="58602-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="58602-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>