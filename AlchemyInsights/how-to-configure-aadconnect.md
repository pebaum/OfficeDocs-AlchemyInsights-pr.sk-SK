---
title: 646 konfigurovaní AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779526"
---
# <a name="configure-sync-features"></a>Konfigurácia funkcie synchronizácie.

Azure AD pripojiť obsahuje niekoľko funkcií, ktoré sú predvolene povolené, alebo že môžete aktivovať neskôr. Niektoré funkcie vyžadujú dodatočné konfigurácia v osobitných prostrediach.
  
- [Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limity objekty sú synchronizované s azúrovo reklamy. Predvolené, všetci používatelia, kontakty, skupiny aj Windows 10 sú synchronizované počítačové kontá. Môžete zahrnúť alebo vylúčiť objekty založené na domény, organizačné jednotky, alebo iné atribúty. 
    
- [Heslo hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla zo služby Active Directory lokálne Azure AD. To umožňuje správu hesiel na jednom mieste, ale používať rovnaké heslo lokálne a cloud prostredí. Pretože Active Directory autoritatívny zdroj, môžete použiť svoje vlastné politiky hesla. 
    
- [Samoobslužné heslo reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje užívateľom obnoviť svoje heslá v cloude pri neustálom uplatňovaní lokálne heslo politika. 
    
- [Zariadenie writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje registrovaných zariadení v Azure AD sa zapíše späť do služby Active Directory lokálne, takže môžu byť použité pre podmienený prístup. 
    
- [Zabránenie náhodnému odstráni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je predvolene zabrániť príliš veľa simultánnych objektov odstránenia (viac ako 500 objekty na synchronizácie). Môžete zmeniť toto nastavenie, aby vyhovovali potrebám vašej organizácie. 
    
- [Automatické aktualizácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) zapnutá predvolene expresné elektroinštalácií a pomáha zabezpečiť vašu verziu Azure AD pripojenie je vždy aktuálny. 
    
