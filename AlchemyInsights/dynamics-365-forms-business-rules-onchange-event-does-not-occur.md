---
title: Dynamics 365 formuláre obchodné pravidlá-obchodné pravidlo nie je paľba pre formulár
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769354"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Udalosť OnChange nenastane, ak sa pole zmení programovo

Udalosť *onChange* nenastane, ak sa pole zmení programovo pomocou *atribútu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metóda. Ak chcete obsluhy udalostí pre udalosť *onChange* spustiť po nastavíte hodnotu musíte použiť *formcontext. Data. entity atribút* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metóda vo vašom kóde.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
