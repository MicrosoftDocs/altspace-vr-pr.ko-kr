---
title: 전역 역할 부여
description: 역할 및 기능 시스템에 대해 알아보고 AltspaceVR 환경에서 사용자 역할을 제공 하는 방법에 대 한 단계별 지침을 확인 하세요.
ms.date: 03/11/2021
ms.topic: article
keywords: 역할
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212790"
---
# <a name="granting-world-roles"></a>전역 역할 부여

Altspace에는 역할 및 기능 시스템이 있습니다. 각 사용자는 여러 역할을 가질 수 있으며 해당 역할은 어디에 있는지에 따라 다를 수 있습니다. 각 역할은 하나 이상의 기능을 제공 합니다. 예를 들어 사용자 고유의 이벤트에 있는 경우 **발표자** 및 **중재자** 역할을 자동으로 받게 됩니다. 이러한 두 가지 역할을 사용 하 여, 준비를 하 고, 색종이를 출시할 수 있습니다. 

1. 전 세계를 편집 하 고 아래로 스크롤하여 **VR** 섹션 (전 세계 [관리 방법](managing-worlds.md))으로 스크롤합니다.

![세계의 VR 섹션에서 역할 변경](images/granting-roles.png)

2. 이 세계의 특정 사용자 에게만 특정 역할을 부여 하려면 **역할** 필드를 편집 합니다. 예를 들어 **발표자**  +  **중재자** **를 제공** 하 고 calen을 제공 하려는 경우 다음을 추가 하 고 **저장** 을 선택 합니다. 형식은 각 줄에서 **{role}, {username 또는 email}** 입니다. 사용자 이름은 대/소문자를 구분 하지 않습니다. 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. **편집** 을 다시 선택 하면 역할 필드 위에 다음이 표시 됩니다. 데이터베이스에서 업데이트 된 것을 알 수 있습니다.

```
Presenters: jimmy
Moderators: jimmy,calen
```

* 이 변경 내용이 Altspace에 적용 되려면 전 세계를 다시 설정 하 여 모든 사용자가 다시 참가 하도록 해야 합니다. 아래에는 역할의 전체 목록이 있습니다.

4. 전 세계에 참가 하는 모든 역할에 역할을 부여 하려면 **컨텍스트 역할** 필드를 편집 합니다. 예를 들어 사용자가 폰를 사용 하 여 서로를 대상으로 하는 동안 서로를 들 여 받을 수 있도록 하려면 다음을 추가 합니다.

```
pilot,megaphone_only
```

**업데이트** 를 선택한 후 전 세계를 다시 설정 합니다. 이는이 세계에만 영향을 줍니다. 역할을 전체 Universe에 부여 하려면 Universe에서 동일한 필드를 편집 합니다. 

## <a name="roles"></a>역할 

* 스테이지에 있을 수 있는 것과 같은 **발표자** 기능
* **중재자** -decorum 유지 관리 **와 같은 기능**
* **Terraformer** -전 세계 편집기를 사용할 수 있습니다.
* **파일럿** -즉석 모드를 전환 하 고 6DOF 비행 도구를 생성 하는 기능
* **Megaphone_only** -전 세계 어디에서 든 사용자의 귀를 이야기 하는 기능
* **Showcase_new_sdk** -MRE sdk 앱을 생성 하는 기능

## <a name="troubleshooting"></a>문제 해결

**역할을 삭제할 수 있나요?**
이제는 폼에서 제공 되지 않으므로 help.altvr.com에서 파일 a를 지원 요청 합니다.

**다른 지역에서 가져올 때 역할이 복사 되나요?**
아니요. 역할은 복사 되지 않습니다.