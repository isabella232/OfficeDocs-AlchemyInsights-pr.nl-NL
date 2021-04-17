---
title: Aanmelden bij Windows 10 zonder een wachtwoord te gebruiken
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830541"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="79d80-102">Aanmelden bij Windows 10 zonder een wachtwoord te gebruiken</span><span class="sxs-lookup"><span data-stu-id="79d80-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="79d80-103">Om te voorkomen dat u een wachtwoord moet typen bij het opstarten van Windows, raden we u aan een van de beveiligde aanmeldingsopties van Windows Hello te gebruiken, zoals een pincode, gezichtsherkenning of vingerafdruk, indien beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="79d80-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="79d80-104">Zie de instructies 'Automatisch aanmelden bij Windows 10' hieronder als u veilige aanmelding echt wilt uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="79d80-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="79d80-105">**Windows Hello-alternatieven voor het accountwachtwoord beveiligen**</span><span class="sxs-lookup"><span data-stu-id="79d80-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="79d80-106">Ga naar **Instellingen > Accounts > aanmeldingsopties** (of klik [hier).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="79d80-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="79d80-107">Beschikbare aanmeldingsopties worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="79d80-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="79d80-108">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="79d80-108">For example:</span></span>

![Aanmeldingsopties.](media/sign-in-options.png)

<span data-ttu-id="79d80-110">Klik of tik op een van de opties om deze te configureren.</span><span class="sxs-lookup"><span data-stu-id="79d80-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="79d80-111">De volgende keer dat u Windows start of ontgrendelt, kunt u de nieuwe optie gebruiken in plaats van een wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="79d80-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="79d80-112">**Automatisch aanmelden bij Windows 10**</span><span class="sxs-lookup"><span data-stu-id="79d80-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="79d80-113">**Opmerking:** Automatische aanmelding is handig, maar brengt een beveiligingsrisico met zich mee, vooral als uw pc toegankelijk is voor meerdere personen.</span><span class="sxs-lookup"><span data-stu-id="79d80-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="79d80-114">Klik of tik op de **knop Start** op de taakbalk.</span><span class="sxs-lookup"><span data-stu-id="79d80-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="79d80-115">Typ **netplwiz en** druk op enter om het venster Gebruikersaccounts te openen.</span><span class="sxs-lookup"><span data-stu-id="79d80-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="79d80-116">Klik **in Gebruikersaccounts** op het account waarop u zich automatisch wilt aanmelden wanneer Windows wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="79d80-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="79d80-117">Het selectievakje 'Gebruikers moeten een gebruikersnaam en wachtwoord invoeren om deze computer te gebruiken' uit.</span><span class="sxs-lookup"><span data-stu-id="79d80-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Gebruikers moeten een gebruikersnaam en wachtwoordoptie invoeren.](media/users-must-enter-username.png)

5. <span data-ttu-id="79d80-119">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="79d80-119">Click **OK**.</span></span> <span data-ttu-id="79d80-120">U wordt gevraagd het wachtwoord in te voeren en te bevestigen voor het account dat u hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="79d80-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="79d80-121">Klik **op OK** om te voltooien.</span><span class="sxs-lookup"><span data-stu-id="79d80-121">Click **OK** to finish.</span></span> <span data-ttu-id="79d80-122">De volgende keer dat Windows 10 wordt gestart, wordt deze automatisch aanmelden bij het account dat u hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="79d80-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
