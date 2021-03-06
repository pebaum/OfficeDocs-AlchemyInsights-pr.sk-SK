---
title: Pracovný postup sa nespúšťa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766112"
---
# <a name="workflow-is-not-starting"></a>Pracovný postup sa nespúšťa

- SharePoint 2010 a SharePoint 2013 toky činností sa nespúšťa.

    - Ak váš pracovný postup nie je začína, môže existovať dočasný problém služby, kde používatelia môžu vyskytnúť občasné oneskorenie s workflow pokrok. Ak chcete zistiť, či je vaša organizácia ovplyvnená, skontrolujte [stav služby](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .

    - Ak uplynulo viac ako 24 hodín, pretože ste prvýkrát videli tento problém, prihláste sa prosím lístok podpory. V mnohých prípadoch už pracujeme na riešení. Prosím, dajte nám aspoň 24 hodín na dokončenie riešenia.

- SharePoint 2010 pracovné postupy oneskorené na začiatku.

    - To nastane, ak pracovný postup sa spúšťa vo veľkých dávkach. (napríklad pri pridaní viacerých položiek naraz).

    - Pracovné postupy nie sú určené na spustenie v reálnom čase, takže oneskorenie je podľa-Design správanie.

   -  Ak je pracovný postup zložitý Extensible Object Markup Language (XMOL), kompilácia môže byť pomalé. Pozrite si [Tento](https://support.microsoft.com//kb/3043697) článok.

    - Pracovný postup by ste mali zjednodušiť alebo ho môžete prepracovať pomocou typu platformy Microsoft SharePoint 2013 workflow.

    - Ak sa História pracovného postupu rozrástla veľké, možno budete chcieť vymazať položky alebo vytvoriť nový zoznam histórie.

        Ďalšie informácie: [Vymazanie histórie pracovného postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Súvisiace témy
Chcete vyskúšať službu Microsoft flow v SharePointe Online?
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


