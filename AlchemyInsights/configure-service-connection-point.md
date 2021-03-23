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
# <a name="configure-service-connection-point-scp"></a>Konfigurace spojovacího bodu služby (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Důvod:** Nelze číst objekt SCP a získat informace o tenantovi Azure AD.
- **Řešení:** Přečtěte si část [Konfigurace spojovacího bodu služby.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akční plán**

- Zkontrolujte, jestli zařízení přijalo objekt zásad skupiny pro řízené ověření.
- Ujistěte se, že objekt zásad skupiny vytvořil klíče registru.
- Ujistěte se, že máte vytvořené 2 klíče s ID adresáře a doménou onmicrosoft.

**Konfigurace nastavení registru na straně klienta pro SCP**

V následujícím příkladu můžete vytvořit objekt Zásady skupiny (GPO) k nasazení nastavení registru, které konfiguruje položku SCP v registru vašich zařízení.

1. Otevřete konzolu Zásady skupiny správy a vytvořte nový objekt zásad skupiny ve vaší doméně.
     - Zadejte název nově vytvořeného objektu zásad skupiny (například ClientSideSCP).

2. Upravte objekt zásad skupiny a vyhledejte následující cestu: **Konfigurace počítače > Předvolby > Nastavení systému Windows > Registru**.

3. Klikněte pravým tlačítkem myši **na Registr** a vyberte > **položka registru.**

4. Na kartě **Obecné** nakonfigurujte následující možnosti:
  
- **Akce:** Aktualizace
    
- **Podregistr**: HKEY_LOCAL_MACHINE
    
- **Cesta ke klíči:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Název hodnoty:** TenantId
    
- **Typ hodnoty:** REG_SZ
    
- **Údaj hodnoty:** Identifikátor GUID nebo ID adresáře instance Azure AD (Tuto hodnotu najdete na webu **Azure Portal > Azure Active Directory > Properties > Directory ID**)
 
- Klikněte na tlačítko **OK**.
 
5. Klikněte pravým tlačítkem myši **na Registr** a vyberte > **položka registru.**

6. Na kartě **Obecné** nakonfigurujte následující možnosti:
  
- **Akce:** Aktualizace
    
- **Podregistr**: HKEY_LOCAL_MACHINE
    
- **Cesta ke klíči:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Název hodnoty:** TenantName
    
- **Typ hodnoty:** REG_SZ
    
- **Údaj hodnoty:** Váš ověřený název domény, pokud používáte federované prostředí, jako je služba AD FS. Váš ověřený název domény nebo název onmicrosoft.com domény (například contoso.onmicrosoft).com, pokud používáte spravované prostředí

- Klikněte na tlačítko **OK**.

7. Zavřete editor nově vytvořeného objektu zásad skupiny.

8. Nově vytvořený objekt zásad skupiny propojete s požadovanou OU obsahující počítače připojené k doméně, které patří k vašemu řízenému základnímu souboru.

Další informace najdete v tématu [Řízené ověřování hybridního připojení k Azure AD – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









