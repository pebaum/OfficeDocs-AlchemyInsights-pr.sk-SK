---
title: Odvolanie alebo nahradenie e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096622"
---
# <a name="recall-or-replace-an-email-message"></a>Odvolanie alebo nahradenie e-mailovej správy

- Môžete **len recall správy, ktoré odosielajú ľudí vo vašej organizácii**. Ak bola odoslaná na adresu služby Gmail, napríklad, nemôžem spomenúť to.
- Môžete **len recall správy odoslané z programu Outlook 2016 pre PC**. Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, si nemôžete spomenúť.
- Ak ste správcom, môžete **recall správy v mene používateľov pomocou prostredia PowerShell**. Nemôže odvolať správy z admin center. Prejdite na "Vyhľadať a odstrániť e-mailových správ v organizácii" pre viac informácií.

***Odvolanie alebo nahradenie e-mailovej správy, ktoré ste odoslali***
1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Sent Items.
2. Otvorte správu, ktorú chcete vyvolať. Musí dvojitým kliknutím otvorte správu. Označte príslušnú správu, takže sa zobrazí v table na čítanie nedovolí odvolať správu.
3. Na karte správy vyberte **akcie** > **Odvolanie tejto správy**.
4. Vyberte **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť novú správu**, potom vyberte **OK**.
5. Ak posielate správu náhradné, napísať správu, potom vyberte **Odoslať**.
6. Úspech či neúspech odvolanie správy závisí od príjemcov nastavenia v programe Outlook. 

Pre viac informácií, vrátane toho, ako skontrolovať na odvolanie, [odvolanie](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)alebo nahradenie e-mailovej správy, ktoré ste odoslali.

***Vyhľadať a odstrániť e-mailových správ v organizácii*** Vyhľadať a odstrániť e-mailových správ v organizácii, je to najjednoduchšie, ak ste globálny admin. Ak nie ste globálne admin, váš účet musí pripočítať skupiny rolí správcu eDiscovery, alebo súlad vyhľadávanie rola. Ak chcete odstrániť správy, musíte pripojiť sa k skupine rolí Správa organizácie alebo Hľadať a očistenie rola. Povolenia na tieto roly priradené [centrum zabezpečenia & súladu](https://protection.office.com/).

1. [Vytvoriť obsah vyhľadávať](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) správy odstrániť.
2. [Pripojiť bezpečnostné & centrum súladu PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ak používate MFA, pozrite si [pripojiť k Office 365 zabezpečenia & súlad centrum PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 