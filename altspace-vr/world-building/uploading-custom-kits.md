---
title: 사용자 지정 키트 업로드
description: AltspaceVR에서 사용자 지정 키트를 설정, 생성 및 업로드하는 방법과 문제 해결 도움말을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 키트, 업로드, 문제 해결
ms.openlocfilehash: 9a90bff2360d854dc398a35501f07cddcbce5c6c66ef8230f2e412a022f8aed0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125529"
---
# <a name="uploading-custom-kits"></a>사용자 지정 키트 업로드

World Editor에는 세계로 생성할 수 있는 Artifacts 포함된 키트가 있습니다. 예를 [들어, Treefire Kit에는](https://account.altvr.com/kits/993516233267609824) 다양한 유형의 트리가 있습니다. 각 트리 유형은 아티팩트입니다. 사용자 고유의 키트를 만들려면 Unity AssetBundles를 만들고 각 아티팩트용 Unity 프리팹이 포함된 .zip 파일을 업로드하고 웹 사이트에 각 아티팩트를 등록해야 합니다. 다행히 커뮤니티 기반 Unity 업로더는 대부분의 워크플로를 자동화합니다. 업로드된 후에는 세계의 사용자 고유의 키트에서 개체를 생성할 수 있으며 다른 사용자가 자동으로 볼 수 있습니다. 나중에 추천을 받아 친구나 전체 Community 키트를 공유할 수 있습니다.

## <a name="prerequisites"></a>사전 요구 사항

1. [Unity Hub 및 Unity 설치](world-building-toolkit-getting-started.md)
2. 최신 버전의 Unity [업로더](https://altvr.com/download-latest-unity-uploader/) 다운로드

## <a name="setup"></a>설정 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. [Worlds > Kits](https://account.altvr.com/kits) 웹 사이트에서 키트 만들기
2. 브라우저의 주소 표시줄에서 클립보드로 키트 ID를 복사합니다(이 단계는 업로더 버전 0.9 이상에서 더 쉬울 수 있음).
3. 새 Unity Project 만들기
4. 패키지를 두 번 클릭하여 Unity 업로더 가져오기

![가져온 Unity 업로더 패키지](images/custom-kits-img-01.png)

5. Altspace 이메일 및 암호를 사용하여 업로더에 로그인합니다.

![Unity의 AltspaceVR 로그인 인터페이스](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>키트 생성 및 업로드

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. 키트 **폴더 이름을** 접두사 및 테마로 입력하고(예: **1137484494681408069_pirates)** 키트 자산 이름을 접두사로 키트 **ID로** 채웁니다. 모든 자산에는 이 접두사 가 있어야 합니다.

![Kit 폴더 이름이 있는 Unity의 AltspaceVR 인터페이스](images/custom-kits-img-03.png)

2. 각 아티팩트 또는 Artifacts 집합에 대해 다음을 수행합니다.
* 원본 Prefab을 계층 탭으로 끌어서
* 세트에 포함할 5가지 유형의 자를 선택합니다.
* 키트 **자산 이름을** **로 업데이트합니다.**
* **GameObject를 키트 프리팹으로 변환을** 선택합니다.
* Assets/Prefabs 폴더에 새 프리팹 및 스크린샷이 생성되었는지 확인합니다.

![아티팩트가 선택된 Unity의 AltspaceVR 인터페이스](images/custom-kits-img-04.png)

> [!NOTE]
> 생성된 Prefab을 수정하려면 계층 구조로 다시 끌어서 변경한 다음 검사기 탭에서 **적용** 을 클릭하여 Prefab을 업데이트합니다. 

3. 준비가 되면 업로더 탭 아래로 스크롤하여 자산 번들이 있는 zip 파일 생성을 준비해 보겠습니다.
4. 더 빠른 반복을 위해 **Android용 빌드 키트를 선택 취소합니다.** 나중에 키트를 공유/기능화하려는 경우 Android용 버전을 빌드하고 업로드해야 합니다. 
5. **로드 키트 프리팹 디렉터리** 선택
6. 키트 폴더 이름과 일치하는 옆에 있는 **빌드를** 선택합니다. 동일한 Unity 프로젝트에서 여러 키트를 생성하는 것이 일반적입니다. 키트의 크기에 따라 시간이 걸릴 수 있습니다. 완료되면 zip 파일이 포함된 폴더가 자동으로 열립니다. 
7. 웹 사이트로 이동하여 이전에 만든 키트를 편집하고, 생성한 zip 파일을 업로드합니다. 이 업로드는 파일 크기에 따라 시간이 걸릴 수 있습니다.
    * 성공하면 왼쪽의 "업로드" 아래에 파일 크기 및 PC 및 Android용 및 마지막으로 업데이트된 시기가 표시됩니다.
    * 실패하면 스크립트가 없는지 확인하고 스크립트를 지원하지 않습니다. 보안에 대한 스크립트를 확인하고 다시 시도합니다.

축하합니다! 사용자 고유의 키트를 사용하여 Worlds를 빌드할 준비가 완료되었습니다.

## <a name="troubleshooting"></a>문제 해결 

**제한이 있나요?**
아직 하드 제한은 없지만 아티팩트를 하나만 사용하더라도 사용자는 전체 키트에 대한 플랫폼용 AssetBundle을 다운로드해야 합니다. 플랫폼별 다운로드를 5MB 이하로 유지해 보세요. 이 작업을 수행하는 한 가지 방법은 작은 키트로 분할하는 것입니다. 예를 들어 200개의 props는 절반으로 분할되어야 합니다. 

**"분할 눈"이 보이나요?**
최신 업로더를 다시 사용하여 올바른 렌더링 설정 얻기

**업데이트/변경 내용이 반영되지 않나요?**
    * 키트 페이지에서 업데이트된 시간 확인
    * World를 다시 시작해도 작동하지 않습니다. 클라이언트를 다시 시작합니다. 업데이트하는 데 몇 분 정도 걸릴 수 있습니다.
    * 폴더 이름 또는 프리팹 이름에 공백이 없는지 **확인합니다(예: 'party_favors'과 'party favors').**

**스크립트가 있다고 계속 말하지만,** 저는 그렇지 않습니다. AssetBundle 브라우저에 파일이 자동으로 포함되기도 합니다. 가져오는 모델을 격리해 보세요. 예를 들어 이미 다른 Prefab의 일부인 경우 끌어서 두지 마세요.

**파티클 시스템 및 애니메이션은 어떤가요?**
이를 위해 메시 렌더링 및 충돌을 사용하지 않도록 설정하여 원점 위치에 있는 1x1x1 큐브 아래에 배치합니다. Particle Systems는 루핑을 사용하도록 설정해야 하며, Altspace에서 크기를 적절하게 조정하려면 **크기 조정을** **계층** 구조로 설정해야 합니다. 모든 애니메이션에 대한 프리팹을 생성한 후 각 애니메이션에 대한 충돌 개체에서 **충돌을** 사용하지 않도록 설정합니다.

**Artifacts 어둡게** 모델의 재질 셰이더를 **모바일/꼭짓점 조명 전용 방향등으로** 설정했나요?

**아티팩트에서 올바른 방법이 아님** **모델** 및 **충돌체를** 회전하고 Prefab을 업데이트합니다. 부모를 회전해도 아무 것도 수행되지 않으며 무시됩니다. **회전 재정의** 필드를 사용하여 이 작업을 쉽게 수행할 수 있습니다.

**이러한 Artifacts SDK의 **CreateFromLibrary** 함수와 함께 사용할 수 있나요?**
예