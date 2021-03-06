---
title: Obísť lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889097"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Ovládanie nastavení vstupnej haly a úrovne účasti v tímoch

Ak chcete povoliť všetkým, vrátane dial-in, externých a anonymných používateľov, **obísť lobby**, použite PowerShell na splnenie tejto úlohy. Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tento cmdlet v súčasnosti vyžaduje použitie Skype Business PowerShell modulu. Ak chcete nastaviť použitie tejto rutiny cmdlet, pozrite sa na [správu politík pomocou prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Po nastavení politiky ju musíte aplikovať na používateľov. alebo ak ste upravili globálnu politiku, automaticky sa bude vzťahovať na používateľov. Pri každej zmene politiky musíte počkať aspoň **4 hodiny až 24 hodín** , kým sa politiky prejavia. 

Nezabudnite si prezrieť dokumentáciu nižšie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Pochopenie tímov pre kontrolu politiky lobby

Tieto nastavenia kontrolujú, ktoré účastníci stretnutia čakajú vo vstupnej hale pred tým, ako sú prijatí na schôdzu, a úroveň účasti, ktorú sú povolené na schôdzi. PowerShell môžete použiť na aktualizáciu nastavenia politiky schôdzí, ktoré ešte neboli implementované (označené ako "pripravujeme") v tíme admin Center. Pozri nižšie pre príklad rutiny cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.

- [Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.

- [Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.

- [Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .

- [Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastala v **automatickom priznávanie ľudí** a **umožniť používateľom telefonického pripojenia, aby pri plánovaní novej schôdze obchádzali vstupnú halu** .

**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams.
