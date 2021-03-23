---
title: Konfigurace spojovacího bodu služby (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035098"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="433d3-102">Konfigurace spojovacího bodu služby (SCP)</span><span class="sxs-lookup"><span data-stu-id="433d3-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="433d3-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="433d3-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="433d3-104">**Důvod:** Nelze číst objekt SCP a získat informace o tenantovi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="433d3-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="433d3-105">**Řešení:** Přečtěte si část [Konfigurace spojovacího bodu služby.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="433d3-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="433d3-106">**Akční plán**</span><span class="sxs-lookup"><span data-stu-id="433d3-106">**Action plan**</span></span>

- <span data-ttu-id="433d3-107">Zkontrolujte, jestli zařízení přijalo objekt zásad skupiny pro řízené ověření.</span><span class="sxs-lookup"><span data-stu-id="433d3-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="433d3-108">Ujistěte se, že objekt zásad skupiny vytvořil klíče registru.</span><span class="sxs-lookup"><span data-stu-id="433d3-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="433d3-109">Ujistěte se, že máte vytvořené 2 klíče s ID adresáře a doménou onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="433d3-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="433d3-110">**Konfigurace nastavení registru na straně klienta pro SCP**</span><span class="sxs-lookup"><span data-stu-id="433d3-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="433d3-111">V následujícím příkladu můžete vytvořit objekt Zásady skupiny (GPO) k nasazení nastavení registru, které konfiguruje položku SCP v registru vašich zařízení.</span><span class="sxs-lookup"><span data-stu-id="433d3-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="433d3-112">Otevřete konzolu Zásady skupiny správy a vytvořte nový objekt zásad skupiny ve vaší doméně.</span><span class="sxs-lookup"><span data-stu-id="433d3-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="433d3-113">Zadejte název nově vytvořeného objektu zásad skupiny (například ClientSideSCP).</span><span class="sxs-lookup"><span data-stu-id="433d3-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="433d3-114">Upravte objekt zásad skupiny a vyhledejte následující cestu: **Konfigurace počítače > Předvolby > Nastavení systému Windows > Registru**.</span><span class="sxs-lookup"><span data-stu-id="433d3-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="433d3-115">Klikněte pravým tlačítkem myši **na Registr** a vyberte > **položka registru.**</span><span class="sxs-lookup"><span data-stu-id="433d3-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="433d3-116">Na kartě **Obecné** nakonfigurujte následující možnosti:</span><span class="sxs-lookup"><span data-stu-id="433d3-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="433d3-117">**Akce:** Aktualizace</span><span class="sxs-lookup"><span data-stu-id="433d3-117">**Action**: Update</span></span>
    
- <span data-ttu-id="433d3-118">**Podregistr**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="433d3-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="433d3-119">**Cesta ke klíči:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="433d3-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="433d3-120">**Název hodnoty:** TenantId</span><span class="sxs-lookup"><span data-stu-id="433d3-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="433d3-121">**Typ hodnoty:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="433d3-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="433d3-122">**Údaj hodnoty:** Identifikátor GUID nebo ID adresáře instance Azure AD (Tuto hodnotu najdete na webu **Azure Portal > Azure Active Directory > Properties > Directory ID**)</span><span class="sxs-lookup"><span data-stu-id="433d3-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="433d3-123">Klikněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="433d3-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="433d3-124">Klikněte pravým tlačítkem myši **na Registr** a vyberte > **položka registru.**</span><span class="sxs-lookup"><span data-stu-id="433d3-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="433d3-125">Na kartě **Obecné** nakonfigurujte následující možnosti:</span><span class="sxs-lookup"><span data-stu-id="433d3-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="433d3-126">**Akce:** Aktualizace</span><span class="sxs-lookup"><span data-stu-id="433d3-126">**Action**: Update</span></span>
    
- <span data-ttu-id="433d3-127">**Podregistr**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="433d3-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="433d3-128">**Cesta ke klíči:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="433d3-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="433d3-129">**Název hodnoty:** TenantName</span><span class="sxs-lookup"><span data-stu-id="433d3-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="433d3-130">**Typ hodnoty:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="433d3-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="433d3-131">**Údaj hodnoty:** Váš ověřený název domény, pokud používáte federované prostředí, jako je služba AD FS.</span><span class="sxs-lookup"><span data-stu-id="433d3-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="433d3-132">Váš ověřený název domény nebo název onmicrosoft.com domény (například contoso.onmicrosoft).com, pokud používáte spravované prostředí</span><span class="sxs-lookup"><span data-stu-id="433d3-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="433d3-133">Klikněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="433d3-133">Click **OK**.</span></span>

7. <span data-ttu-id="433d3-134">Zavřete editor nově vytvořeného objektu zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="433d3-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="433d3-135">Nově vytvořený objekt zásad skupiny propojete s požadovanou OU obsahující počítače připojené k doméně, které patří k vašemu řízenému základnímu souboru.</span><span class="sxs-lookup"><span data-stu-id="433d3-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="433d3-136">Další informace najdete v tématu [Řízené ověřování hybridního připojení k Azure AD – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="433d3-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









