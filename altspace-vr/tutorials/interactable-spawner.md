---
title: Interactables Spawner 사용
description: Interactables spawner을 만들고, 사용 하 고, 사용자 지정 하 여 AltspaceVR 공간에 항목을 저장 하는 방법을 알아봅니다.
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

Interactables Spawner를 사용 하면 이벤트, 세계 또는 홈 공간에 interactable 항목을 삽입할 수 있습니다. 이 기능은 현재 [초기 액세스 프로그램](../world-building/early-access.md) 의 일부 이며 주 메뉴를 통해 옵트인 한 경우에만 사용할 수 있습니다.

> [!NOTE]
> 이 기능을 계속 해 서 실험 하는 동안 너무 많은 상호 중단을 생성 하면 사용자 환경이 나 이벤트의 성능에 영향을 줄 수 있습니다. 

## <a name="creating-an-interactable"></a>Interactable 만들기

개체를 interactable 개체로 변환 하려면 다음을 수행 합니다.

1. 개체를 공간에 넣습니다.
2. 그런 다음 개체 목록에서 항목을 찾고 옆의 **기어 아이콘** 을 선택 하 여 해당 설정을 엽니다.

![개체 목록이 강조 표시 된 세계 편집기 열기](images/interactables-spawner-img-01.png)

설정 페이지에서 새 확인란 **"object spawner"** 를 찾을 수 있습니다 .이 확인란을 사용 하 여 interactable 개체로 만들 수 있습니다.

1. 확인란을 선택 하 고 **확인** 을 선택 합니다.
2. 편집 모드에 있는 동안에는 공간에서 개체의 생성 위치를 이동할 수 있습니다.
3. 항목 상호 작용을 사용 하려면 **편집 모드를 종료** 합니다.

![AltspaceVR 앱에서 열린 아티팩트 업데이트 창](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>기타 사용자 지정

**"Object spawner"** 를 사용 하도록 설정한 후 해당 개체의 속성으로 돌아가서 생성 된 개체가 동작 하는 방식에 적용할 수 있는 추가 설정이 있습니다.

> [!NOTE]
> Interactable 개체 크기 조정: 개체를 처음으로 선택 하기 전에 전 세계에 표시 되는 개체의 크기를 나타내는 "Scale"과 비교 하 여 개체를 선택할 때 개체의 소수 자릿수를 설정 합니다.

키트 작성자는 AltspaceVR가 실행 되는 동안 키트의 변경 내용이 적용 되지 않을 수 있습니다. AltspaceVR를 다시 시작할 때까지 적용 되지 않습니다.

최근, **일반 설정** 탭 아래에는 **세계 키트 다시 로드** 라는 단추가 추가 되었습니다. 이 단추를 클릭 하면 (사용자만) 공간을 다시 로드 하 여 모든 키트를 다시 로드 합니다. 그러면 AltspaceVR에 있는 동안 업데이트 된 키트의 새 버전만 다운로드 됩니다.

![AltspaceVR 앱에서 일반 설정 패널 열기](images/interactables-spawner-img-03.png)