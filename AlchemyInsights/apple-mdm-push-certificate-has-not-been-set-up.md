---
title: Apple MDM Push Certificate is niet ingesteld
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
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439014"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="b1889-102">Apple MDM Push Certificate is niet ingesteld</span><span class="sxs-lookup"><span data-stu-id="b1889-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="b1889-103">Een Apple MDM Push Certificate (ook wel bekend als een Apple Push Notification Service (APNS) certificaat) is niet geconfigureerd voor uw abonnement.</span><span class="sxs-lookup"><span data-stu-id="b1889-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="b1889-104">Zonder een Apple MDM Push Certificate geconfigureerd, u iOS- en Mac OS-apparaten niet inschrijven en beheren.</span><span class="sxs-lookup"><span data-stu-id="b1889-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="b1889-105">Nadat u het certificaat aan Intune hebt toegevoegd, kunnen gebruikers de Bedrijfsportal-app installeren om hun iOS-apparaten in te schrijven.</span><span class="sxs-lookup"><span data-stu-id="b1889-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="b1889-106">Selecteer **'Ik ga akkoord'.**</span><span class="sxs-lookup"><span data-stu-id="b1889-106">Select **"I agree."**</span></span> <span data-ttu-id="b1889-107">om Microsoft toestemming te geven om gegevens naar Apple te verzenden.</span><span class="sxs-lookup"><span data-stu-id="b1889-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="b1889-108">Selecteer **Uw csr downloaden** van het intune-certificaatondertekeningsverzoek dat nodig is om een Apple MDM-pushcertificaat te maken.</span><span class="sxs-lookup"><span data-stu-id="b1889-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="b1889-109">Het bestand wordt gebruikt om een vertrouwensrelatiecertificaat aan te vragen bij de Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="b1889-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="b1889-110">Selecteer **Uw MDM-pushcertificaat maken** om naar de Apple Push Certificates Portal te gaan.</span><span class="sxs-lookup"><span data-stu-id="b1889-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="b1889-111">Meld u aan bij uw bedrijf Apple ID en selecteer **Vervolgens Een certificaat maken**.</span><span class="sxs-lookup"><span data-stu-id="b1889-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="b1889-112">Selecteer **Bestand kiezen,** blader naar het aanvraagbestand voor certificaatondertekenen en kies **Upload**.</span><span class="sxs-lookup"><span data-stu-id="b1889-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="b1889-113">Kies op de pagina Bevestiging **download** om het certificaatbestand (.pem) te downloaden en sla het bestand lokaal op.</span><span class="sxs-lookup"><span data-stu-id="b1889-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="b1889-114">**Opmerking**: Het certificaat is gekoppeld aan de Apple ID die wordt gebruikt om het te maken.</span><span class="sxs-lookup"><span data-stu-id="b1889-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="b1889-115">Gebruik als aanbevolen praktijk een Apple ID voor beheertaken en zorg ervoor dat het postvak door meer dan één persoon wordt gecontroleerd of door een distributielijst te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="b1889-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="b1889-116">Gebruik nooit een persoonlijke Apple ID.</span><span class="sxs-lookup"><span data-stu-id="b1889-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="b1889-117">Gebruik dezelfde Apple ID om het Apple Push-certificaat elke 12 maanden te verlengen.</span><span class="sxs-lookup"><span data-stu-id="b1889-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="b1889-118">Voer de Apple ID in die wordt gebruikt om uw Apple MDM-pushcertificaat te maken.</span><span class="sxs-lookup"><span data-stu-id="b1889-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="b1889-119">Neem deze id op als een herinnering voor wanneer u het certificaat moet verlengen.</span><span class="sxs-lookup"><span data-stu-id="b1889-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="b1889-120">Ga naar het certificaatbestand (.pem), kies **Openen**en kies **vervolgens Uploaden**.</span><span class="sxs-lookup"><span data-stu-id="b1889-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="b1889-121">Met het pushcertificaat kan Intune Apple-apparaten inschrijven en beheren.</span><span class="sxs-lookup"><span data-stu-id="b1889-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>