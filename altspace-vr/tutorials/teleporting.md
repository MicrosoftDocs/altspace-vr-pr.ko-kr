---
title: 원격 통신기 사용
description: AltspaceVR에서 원격 통신기를 사용하여 한 이벤트 또는 세계에서 다른 이벤트 또는 세계로 이동하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 텔 레 포터
ms.openlocfilehash: 79c5b09e1643a70939ba1e967a948ac6c80c2b615bce9eef598d0e07b7722ea3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126191"
---
# <a name="using-the-teleporter"></a>원격 통신기 사용

이벤트 또는 세계에서 다른 이벤트로 이동하는 것은 여러분과 커뮤니티에서 AltspaceVR이 제공해야 하는 모든 것을 살펴볼 수 있는 좋은 방법입니다.

## <a name="the-short-version"></a>짧은 버전

![편집기 패널에서 원격 보고 대상 설정으로 단계 전송](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>약간 더 긴 버전

먼저 생성했거나 Terraformer 역할이 부여된 이벤트 또는 세계의 홈스페이스에 있는지 확인합니다. 2D 모드에 있고 UI의 오른쪽 아래에 세계 편집기 단추가 표시되지 않는 경우 마우스 단추를 마우스 오른쪽 단추로 클릭하여 켜기/끄기를 전환합니다. 여전히 세계 편집기 단추가 표시되지 않으면 다른 사람의 공간에 있을 수 있습니다. 이 경우 호스트에 Terraformer 역할을 제공하도록 요청합니다.

또한 다음을 수행할 수 있습니다. 
1. 먼저 이벤트 또는 세계 만들기
2. Teleporter를 생성하려는 위치로 이동하여 이벤트/세계는 Teleporter 대상 패널에 채워지고 더 빠르고 쉽게 연결할 수 있도록 합니다.

2D 모드에서 Teleporters를 탐색하는 데 도움이 되는 또 다른 트릭은 Ctrl + 스페이스바를 사용하는 것입니다. 명령 프롬프트가 표시되고 back -을 입력하면 마지막 공간으로 돌아갈 수 있습니다. 

이제 Teleporter를 생성하려는 위치로 이동하여 세계 편집기/편집기 패널/기본 사항/Teleporter를 선택합니다.

그러면 Teleporter 대상 패널이 표시됩니다. 선택할 세 가지 범주가 표시됩니다.

* **MY SPACES** - 만든 세계 목록입니다.
* **최근** - 최근 이벤트 목록입니다. 이벤트로 이동하려는 경우 이 옵션을 사용합니다. 이 옵션은 이벤트로 이동하는 유일한 옵션이며, 나머지 2개는 세계 사이를 이동하도록 허용합니다. 참고: Imported Worlds가 있는 Front Row 이벤트를 연결하는 경우 실제 이벤트가 아닌 Imported World에서 Teleporters를 생성하고 설정해야 하는 경우 아래 고급을 참조하세요.
* **추천** - 이동하도록 Teleporter를 설정할 수 있는 추천 세계 목록입니다.

사용하려는 이벤트 또는 세계를 선택하면 Teleporter가 생성되고 이벤트 또는 세계 이름의 레이블 텍스트가 약간 뒤에 배치됩니다. 따라서 개체 표시 섹션에서 기어 아이콘을 선택하여 레이블 이름을 변경할 수 있습니다.

커서를 사용하여 Teleporter를 선택하거나(잘못 클릭된 경우 해당 위치에 이동할 수 있는지 묻는 메시지가 표시될 수 있습니다.) 바로 Teleporter로 아바타를 이동하고, 미리 보고, 대상으로 이동할 수 있습니다. 안녕하세요!

## <a name="advanced-features"></a>고급 기능

사용자 지정 세계와 함께 Front Row를 사용하여 회의, 회의 또는 대규모 이벤트를 만드는 경우(예: Foundation World, Unity Uploader Space Template, Re-Import World) 실제 이벤트가 아닌 Foundation World에서 Teleporter를 설정해야 합니다. Foundation World에서 올바른 이벤트(최근 목록에 있어야 합니다)로 이동하도록 Teleporter를 설정하고 이벤트에서 World를 Re-Import 모든 프런트 행 이벤트 공간에 Teleporters가 표시되도록 합니다.

## <a name="faqs"></a>FAQ

**오류: '죄송합니다. 하지만 그 안에는 사용할 수 없습니다.'**

이벤트에는 그룹이 연결되어 있을 수 있으므로 그룹의 사용자 이름만 해당 Teleporter에 연결하여 해당 프라이빗 그룹 이벤트에 연결할 수 있습니다.

**한 공간에서 사용할 수 있는 원격 통신기는 몇 개입니까?**

원격 통신기는 애니메이션 효과가 적용된 파티클 효과와 함께 투명한 질감을 사용하므로 성능에 영향을 줄 수 있으므로 동일한 스폿/겹침에 너무 많은 텍스처를 두지 않는 것이 가장 좋습니다. 동일한 영역에 4개 이상 또는 모두 공간에 분산된 경우 10개 이상을 갖지 않도록 합니다.