---
title: Nebyl nastaven nabízený certifikát Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716850"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="b7954-102">Nebyl nastaven nabízený certifikát Apple MDM</span><span class="sxs-lookup"><span data-stu-id="b7954-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="b7954-103">Pro vaše předplatné není nakonfigurovaný certifikát Apple MDM pro nabízené (označované také jako certifikát APNS (Apple Push Notification Service)).</span><span class="sxs-lookup"><span data-stu-id="b7954-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="b7954-104">Bez nakonfigurovaného účtu Apple MDM push nemůžete registrovat a spravovat zařízení s iOS a Mac OS.</span><span class="sxs-lookup"><span data-stu-id="b7954-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="b7954-105">Po přidání certifikátu do Intune můžou uživatelé nainstalovat aplikaci Portál společnosti pro registraci zařízení s iOS.</span><span class="sxs-lookup"><span data-stu-id="b7954-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="b7954-106">Vyberte **"Souhlasím".**</span><span class="sxs-lookup"><span data-stu-id="b7954-106">Select **"I agree."**</span></span> <span data-ttu-id="b7954-107">poskytnutí oprávnění Microsoftu k posílání dat na Apple.</span><span class="sxs-lookup"><span data-stu-id="b7954-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="b7954-108">Vyberte **Stáhnout oddělení služeb zákazníkům** : žádost o podepsání certifikátu Intune požadovaná k vytvoření certifikátu Apple MDM push.</span><span class="sxs-lookup"><span data-stu-id="b7954-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="b7954-109">Soubor se používá k vyžádání certifikátu vztahu důvěryhodnosti na portálu Apple Push Certificates.</span><span class="sxs-lookup"><span data-stu-id="b7954-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="b7954-110">Vyberte **vytvořit certifikát MDM** pro přechod na portál Apple Push Certificates.</span><span class="sxs-lookup"><span data-stu-id="b7954-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="b7954-111">Přihlaste se pomocí Apple ID společnosti a pak vyberte **vytvořit certifikát**.</span><span class="sxs-lookup"><span data-stu-id="b7954-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="b7954-112">Vyberte **zvolit soubor**, přejděte do souboru žádosti o podpis certifikátu a pak zvolte **nahrát**.</span><span class="sxs-lookup"><span data-stu-id="b7954-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="b7954-113">Na stránce s potvrzením zvolte **Stáhnout** a Stáhněte si soubor Certificate (. pem) a uložte soubor místně.</span><span class="sxs-lookup"><span data-stu-id="b7954-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="b7954-114">**Poznámka**: certifikát je přidružený k Apple ID použitému k jeho vytvoření.</span><span class="sxs-lookup"><span data-stu-id="b7954-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="b7954-115">Nejvhodnějším postupem je použít pro úkoly správy společnost Apple ID společnosti a zkontrolovat, jestli je poštovní schránka monitorovaná více lidmi, nebo pomocí distribučního seznamu.</span><span class="sxs-lookup"><span data-stu-id="b7954-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="b7954-116">Nikdy nepoužívejte osobní ID Apple.</span><span class="sxs-lookup"><span data-stu-id="b7954-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="b7954-117">Pomocí stejného Apple ID prodlužte platnost certifikátu Apple Push každých 12 měsíců.</span><span class="sxs-lookup"><span data-stu-id="b7954-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="b7954-118">Zadejte Apple ID používané k vytvoření svého certifikátu Apple MDM push.</span><span class="sxs-lookup"><span data-stu-id="b7954-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="b7954-119">Pokud potřebujete certifikát prodloužit, nahrajte toto ID jako připomenutí.</span><span class="sxs-lookup"><span data-stu-id="b7954-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="b7954-120">Přejděte do souboru Certificate (. pem), zvolte **otevřít**a pak zvolte **nahrát**.</span><span class="sxs-lookup"><span data-stu-id="b7954-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="b7954-121">S certifikátem push může Intune zaregistrovat a spravovat zařízení Apple.</span><span class="sxs-lookup"><span data-stu-id="b7954-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>