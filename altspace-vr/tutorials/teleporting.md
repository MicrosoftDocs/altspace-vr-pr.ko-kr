---
title: Teleporter 사용
description: AltspaceVR의 teleporter를 사용 하 여 한 이벤트에서 다른 이벤트로 이동 하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: teleporter
ms.openlocfilehash: afc199e958824bb5f0a9ff6d74865cbcd3f16868
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213417"
---
# <a name="using-the-teleporter"></a>Teleporter 사용

한 이벤트에서 다른 이벤트로 이동 하는 것은 사용자와 커뮤니티에서 AltspaceVR가 제공 해야 하는 모든 것을 탐색할 수 있는 좋은 방법입니다.

## <a name="the-short-version"></a>짧은 버전

![Teleportation 대상을 설정 하기 위해 편집기 패널에서 단계 Teleporting](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>약간 더 긴 버전

먼저 Homespace에서 사용자가 만들었거나 Terraformer 역할을 제공 받은 이벤트 또는 세계에 있는지 확인 합니다. 2D 모드에 있고 UI의 오른쪽 아래에 있는 세계 편집기 단추를 표시 하지 않는 경우 마우스 단추를 마우스 오른쪽 단추로 클릭 하 여 설정/해제를 설정/해제 합니다. 여전히 전 세계 편집기 단추가 표시 되지 않으면 다른 사람의 공간에 있을 수 있습니다. 이 경우 호스트에 요청 하 여 Terraformer 역할을 제공 합니다.

또한 다음 작업을 수행 하는 데 도움이 됩니다. 
1. 먼저 이벤트 또는 전 세계 만들기
2. Teleporter를 생성 하려는 위치로 이동 하 여 이벤트/작업을 Teleporter 대상 패널에 채우고 더 빠르고 쉽게 연결할 수 있도록 합니다.

2D 모드에서 Teleporters를 사용 하 여 탐색 하는 또 다른 트릭은 Ctrl + 스페이스바를 사용 하는 것입니다. 명령 프롬프트를 표시 하 고 다음을 입력할 수 있습니다. 뒤로-이전에 사용 했던 공간으로 돌아갑니다. 

이제 Teleporter을 생성 하려는 위치로 이동 하 고 세계 편집기/편집기 패널/기본 사항/Teleporter을 선택 합니다.

그러면 Teleporter 대상 패널이 표시 됩니다. 선택할 수 있는 세 가지 범주가 표시 됩니다.

* **내 공백** -사용자가 만든 세계 목록입니다.
* **최근** -최근 발생 한 이벤트의 목록입니다. 이벤트로 이동 하려는 경우이 옵션을 사용 합니다 .이 옵션을 사용 하면 이벤트로 이동 하 여 다른 2를 사용 하는 경우에만이 옵션을 사용할 수 있습니다. 참고: 가져온 프런트 행 이벤트를 연결 하는 경우 아래의 고급을 참조 하세요. 실제 이벤트가 아닌 가져온 환경에서 Teleporters를 생성 하 고 설정 해야 합니다.
* **추천** -Teleporter 이동 하도록 설정할 수 있는 주요 세계 목록입니다.

사용 하려는 이벤트를 선택 합니다. 그러면 Teleporter가 생성 되 고 이벤트 또는 세계 이름의 텍스트 레이블이 약간 뒤에 표시 됩니다. 따라서 현재 개체 섹션에서 기어 아이콘을 선택 하 여 레이블 이름을 변경할 수 있습니다.

커서를 사용 하 여 Teleporter를 선택 하거나 (마우스 단추를 클릭 하지 않은 경우) 아바타를 Teleporter 및 presto로 이동 하 여 대상으로 이동 하 게 할 수 있습니다. 안녕하세요.

## <a name="advanced-features"></a>고급 기능

사용자 지정 전 세계의 Front 행을 사용 하 여 회의, summit 이상의 이벤트를 만드는 경우 (예: 기초 세계, Unity 업 로더 공간 템플릿, Re-Import 세계) 실제 이벤트가 아니라 기초 세계에서 Teleporter를 설정 해야 합니다. Teleporter를 올바른 이벤트 (최신 목록에서 가져와야 함)로 이동 하도록 설정 하 고, 이벤트에서 세계를 Re-Import 하 여 모든 Front Row 이벤트 공간에 Teleporters를 표시 해야 합니다.

## <a name="faqs"></a>FAQ

**오류: ' 죄송 합니다. 죄송 합니다. 죄송 합니다.**

이벤트에는 연결 된 그룹이 있을 수 있으므로 그룹의 사용자만이 해당 Teleporter로 이동 하 여 해당 개인 그룹 이벤트에 액세스할 수 있습니다.

**한 공간에서 사용할 수 있는 teleporters는 몇 개입니까?**

Teleporters는 애니메이션 파티클 효과와 함께 투명 한 질감을 사용 하 고 있으므로 성능에 영향을 줄 수 있으므로 동일한 지점에 너무 많이 포함 하지 않는 것이 좋습니다. 동일한 영역에 4 개 이상의를 포함 하지 않도록 하거나, 모두 공간에 분산 된 경우 10 개 이상으로 시도 하지 마십시오.