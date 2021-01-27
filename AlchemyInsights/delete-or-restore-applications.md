---
title: Toepassingen verwijderen of herstellen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014796"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="23e4b-102">Toepassingen verwijderen of herstellen</span><span class="sxs-lookup"><span data-stu-id="23e4b-102">Delete or restore applications</span></span>

<span data-ttu-id="23e4b-103">**Een toepassing verwijderen uit een Azure AD-Tenant**:</span><span class="sxs-lookup"><span data-stu-id="23e4b-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="23e4b-104">Selecteer **Enterprise toepassingen** in de **Azure AD-Portal**.</span><span class="sxs-lookup"><span data-stu-id="23e4b-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="23e4b-105">Zoek en selecteer de toepassing die u wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="23e4b-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="23e4b-106">Selecteer in de sectie **beheren** van het linkerdeelvenster **Eigenschappen**.</span><span class="sxs-lookup"><span data-stu-id="23e4b-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="23e4b-107">Selecteer **verwijderen** en selecteer vervolgens **Ja** om te bevestigen dat u de app wilt verwijderen uit uw Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="23e4b-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="23e4b-108">Zie voor meer informatie over het verwijderen van een app [: een toepassing verwijderen uit uw Azure Active Directory (Azure AD)-Tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="23e4b-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="23e4b-109">In PowerShell worden toepassings proxy configuraties uit een bepaalde toepassing in azure Active Directory verwijderd uit PowerShell en [kan de toepassing](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) helemaal verwijderen, indien opgegeven.</span><span class="sxs-lookup"><span data-stu-id="23e4b-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="23e4b-110">U kunt **een verwijderde toepassing herstellen** met PowerShell.</span><span class="sxs-lookup"><span data-stu-id="23e4b-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="23e4b-111">Wanneer de toepassing die u wilt herstellen is vastgesteld, kunt u deze herstellen met [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="23e4b-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
