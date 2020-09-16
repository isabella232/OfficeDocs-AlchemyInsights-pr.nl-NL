---
title: Meld u aan bij Windows 10 zonder een wachtwoord te gebruiken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719948"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="2fdcc-102">Meld u aan bij Windows 10 zonder een wachtwoord te gebruiken</span><span class="sxs-lookup"><span data-stu-id="2fdcc-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="2fdcc-103">Als u wilt voorkomen dat u een wachtwoord typt bij het opstarten van Windows, kunt u het beste een van de veilige aanmeldingsopties van Windows hello gebruiken, zoals een pincode, gezichtsherkenning of vingerafdruk, indien beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="2fdcc-104">Als u de beveiligde aanmelding echt wilt uitschakelen, raadpleegt u de instructies bij automatisch aanmelden bij Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="2fdcc-105">**Beveiligings suggesties van Windows hello naar het accountwachtwoord**</span><span class="sxs-lookup"><span data-stu-id="2fdcc-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="2fdcc-106">Ga naar **instellingen > Accounts > aanmeldingsopties** (of Klik [hier](ms-settings:signinoptions?activationSource=GetHelp).)</span><span class="sxs-lookup"><span data-stu-id="2fdcc-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2fdcc-107">De beschikbare aanmeldingsopties worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="2fdcc-108">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="2fdcc-108">For example:</span></span>

![Aanmeldingsopties.](media/sign-in-options.png)

<span data-ttu-id="2fdcc-110">Klik of tik op een van de opties om deze te configureren.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="2fdcc-111">De volgende keer dat u Windows start of ontgrendelt, kunt u de nieuwe optie gebruiken in plaats van een wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="2fdcc-112">**Automatisch aanmelden bij Windows 10**</span><span class="sxs-lookup"><span data-stu-id="2fdcc-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="2fdcc-113">**Opmerking**: automatische aanmelding is handig, maar maakt een beveiligingsrisico, met name als uw PC toegankelijk is voor meerdere personen.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="2fdcc-114">Klik of tik op de knop **Start** op de taakbalk.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="2fdcc-115">Typ **netplwiz** en druk op ENTER om het venster gebruikers accounts te openen.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="2fdcc-116">Klik bij **gebruikers accounts**op het account waarmee u zich automatisch wilt aanmelden wanneer Windows wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="2fdcc-117">Schakel het selectievakje Gebruikers moeten een gebruikersnaam en wachtwoord invoeren om deze computer te gebruiken uit.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Gebruikers moeten de optie gebruikersnaam en wachtwoord invoeren.](media/users-must-enter-username.png)

5. <span data-ttu-id="2fdcc-119">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-119">Click **OK**.</span></span> <span data-ttu-id="2fdcc-120">U wordt gevraagd het wachtwoord in te voeren en te bevestigen van het account dat u hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="2fdcc-121">Klik op **OK** om de bewerking te voltooien.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-121">Click **OK** to finish.</span></span> <span data-ttu-id="2fdcc-122">De volgende keer dat Windows 10 wordt gestart, wordt u automatisch aangemeld bij het account dat u hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="2fdcc-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
