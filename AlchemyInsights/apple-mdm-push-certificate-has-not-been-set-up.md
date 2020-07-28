---
title: Certifikát Apple MDM Push certificate nebyl nastaven.
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
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438852"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="9177c-102">Certifikát Apple MDM Push certificate nebyl nastaven.</span><span class="sxs-lookup"><span data-stu-id="9177c-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="9177c-103">Pro vaše předplatné nebyl nakonfigurován certifikát Apple MDM (označovaný také jako certifikát Služby nabízených oznámení Apple (APNS).</span><span class="sxs-lookup"><span data-stu-id="9177c-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="9177c-104">Bez nakonfigurovaného nabízeného certifikátu Apple MDM nemůžete zaregistrovat a spravovat zařízení se systémem iOS a Mac OS.</span><span class="sxs-lookup"><span data-stu-id="9177c-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="9177c-105">Po přidání certifikátu do Intune si uživatelé můžou nainstalovat aplikaci Portál společnosti a zaregistrovat svá iOS zařízení.</span><span class="sxs-lookup"><span data-stu-id="9177c-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="9177c-106">Vyberte **možnost Souhlasím.**</span><span class="sxs-lookup"><span data-stu-id="9177c-106">Select **"I agree."**</span></span> <span data-ttu-id="9177c-107">a udělí společnosti Microsoft oprávnění k odesílání dat společnosti Apple.</span><span class="sxs-lookup"><span data-stu-id="9177c-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="9177c-108">Vyberte **Stáhnout csr** žádost o podepisování certifikátu Intune, která je vyžadována k vytvoření nabízeného certifikátu Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="9177c-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="9177c-109">Soubor se používá k vyžádání certifikátu vztahu důvěryhodnosti z portálu Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="9177c-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="9177c-110">Výběrem **možnosti Vytvořit nabízený certifikát MDM přejděte** na portál Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="9177c-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="9177c-111">Přihlaste se pomocí firemního Apple ID a pak vyberte **Vytvořit certifikát**.</span><span class="sxs-lookup"><span data-stu-id="9177c-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="9177c-112">Vyberte **Vybrat soubor**, vyhledejte soubor žádosti o podpis certifikátu a pak zvolte **Nahrát**.</span><span class="sxs-lookup"><span data-stu-id="9177c-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="9177c-113">Na stránce Potvrzení zvolte **Stáhnout, chcete-li** stáhnout soubor certifikátu (.pem) a uložit soubor místně.</span><span class="sxs-lookup"><span data-stu-id="9177c-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="9177c-114">**Poznámka:** Certifikát je spojený s Apple ID použitým k jeho vytvoření.</span><span class="sxs-lookup"><span data-stu-id="9177c-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="9177c-115">Osvědčeným postupem je použití firemního Apple ID pro úkoly správy a ujistěte se, že poštovní schránka je monitorována více než jednou osobou nebo pomocí distribučního seznamu.</span><span class="sxs-lookup"><span data-stu-id="9177c-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="9177c-116">Nikdy nepoužívejte osobní Apple ID.</span><span class="sxs-lookup"><span data-stu-id="9177c-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="9177c-117">K obnovení apple push certifikátu každých 12 měsíců použijte stejné Apple ID.</span><span class="sxs-lookup"><span data-stu-id="9177c-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="9177c-118">Zadejte Apple ID použité k vytvoření nabízeného certifikátu Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="9177c-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="9177c-119">Toto ID zaznamenejte jako připomenutí, kdy potřebujete certifikát obnovit.</span><span class="sxs-lookup"><span data-stu-id="9177c-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="9177c-120">Přejděte do souboru certifikátu (.pem), zvolte **Otevřít**a pak zvolte **Nahrát**.</span><span class="sxs-lookup"><span data-stu-id="9177c-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="9177c-121">S nabízeným certifikátem může Intune zaregistrovat a spravovat zařízení Apple.</span><span class="sxs-lookup"><span data-stu-id="9177c-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>