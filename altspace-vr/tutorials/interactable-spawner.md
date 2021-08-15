---
title: Interactables Spawner 사용
description: AltspaceVR 공간에 항목을 배치하도록 상호 작용 가능한 생성자를 만들고, 사용하고, 사용자 지정하는 방법을 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: spawner, 상호 작용, 사용자 지정
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127403"
---
# <a name="using-the-interactables-spawner"></a>Interactables Spawner 사용

Interactables Spawner를 사용하면 이벤트, 세계 또는 홈 공간에 상호 작용 가능한 항목을 배치할 수 있습니다. 이 기능은 현재 초기 [액세스 프로그램의](../world-building/early-access.md) 일부이며 주 메뉴를 통해 옵트인하지 않는 한 사용할 수 없습니다.

> [!NOTE]
> 이 기능을 계속 파일럿하는 동안 너무 많은 상호 작용 가능 파일을 생성하면 환경 또는 이벤트의 성능에 영향을 줄 수 있다는 점에 유의하세요. 

## <a name="creating-an-interactable"></a>상호 작용 가능한 만들기

개체를 상호 작용 가능한 개체로 전환하려면 다음을 수행합니다.

1. 개체를 공간에 배치합니다.
2. 그런 다음, 개체 목록에서 항목을 찾고 옆에 있는 **기어 아이콘을** 선택하여 해당 설정을 엽니다.

![개체 목록이 강조 표시된 채 열린 세계 편집기](images/interactables-spawner-img-01.png)

설정 페이지에서 상호 작용 가능한 개체로 만드는 데 사용되는 **새 "개체 생성자"** 확인란을 찾을 수 있습니다.

1. 확인란을 선택하고 **확인을** 선택합니다.
2. 편집 모드에서 공간에서 개체의 생성 위치를 이동할 수 있습니다.
3. 항목 상호 작용을 사용하도록 설정하려면 **편집 모드를 종료합니다.**

![AltspaceVR 앱에서 열린 아티팩트 창 업데이트](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>기타 사용자 지정

해당 개체의 속성으로 돌아갈 때 **"개체 생성자"를** 사용하도록 설정한 후에는 생성된 개체의 동작 방식에 적용할 수 있는 추가 설정이 있습니다.

> [!NOTE]
> 상호 작용 가능한 개체 배율: 개체를 처음 선택하기 전에 개체가 전 세계에 나타나는 방식의 배율인 "Scale"과 비교하여 개체의 크기를 설정합니다.

AltspaceVR을 실행하는 동안 키트에 대한 변경 내용은 AltspaceVR을 다시 시작할 때까지 적용되지 않는다는 것을 키트 작성자가 알 수 있습니다.

최근에 **Moderate 설정** 탭 아래에 Worlds Kit 다시 로드라는 단추를 **추가했습니다.** 이 단추를 클릭하면 (본인만) 공간을 다시 입력하고 모든 키트를 다시 로드합니다. 그러면 AltspaceVR에 있는 동안 업데이트된 새 버전의 키트만 다운로드됩니다.

![AltspaceVR 앱에서 열린 조정 설정 패널](images/interactables-spawner-img-03.png)