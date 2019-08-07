---
title: Problémy s MZV
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250180"
---
# <a name="issues-with-mfa"></a>Problémy s MZV
Existuje pár vecí na kontrolu, ak užívatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)

1. Príslušného používateľa môže byť zablokovaný v portáli Azure Active Directory. Ak je tomu tak, overovacie pokusy, že konkrétny používateľ bude automaticky zamietnutý. [Postupujte podľa krokov v tomto článku a ich odblokovanie.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak nepomohlo, odblokovanie používateľa alebo používateľ nie je blokovaný môžete skúsiť obnoviť MFA pre používateľa a pôjdu cez proces registrovať znova. [Postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak je to prvýkrát, čo ste MZV zapnuté a používatelia schopní prihlásiť-prehliadače klientov ako je Outlook, Skype, atď, možno ADAL (Active Directory overenie knižnica) nie je povolená na odber služby O365. V tomto prípade budete musieť pripojiť k Exchange Online Powershell a spustite tento cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*