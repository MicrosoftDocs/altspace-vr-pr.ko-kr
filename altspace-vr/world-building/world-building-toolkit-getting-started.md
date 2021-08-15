---
title: 세계 빌드 Toolkit 소개
description: World Building Toolkit Unity 장면 템플릿을 사용하여 AltspaceVR 세계를 설치하고 업로드하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 툴킷
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125409"
---
# <a name="introducing-the-world-building-toolkit"></a>세계 빌드 Toolkit 소개

> [!NOTE]
> World Building Toolkit 놀라운 [친구인 여하우가](https://twitter.com/chigamesstudio)진행하는 커뮤니티 프로젝트로, 지원을 받고 있습니다. 관심이 있는 경우 [공식 AltspaceVR Discord에](https://discordapp.com/invite/altspacevr) 조인하고 #world 빌드 채널을 방문하세요. 현재 Mac 평가판 베타가 있습니다. [자세한 내용](https://altvr.com/altspacevr-mac)

업로더를 사용하면 Unity 장면을 전 세계에 대한 템플릿으로 사용할 수 있습니다. Minecraft 즐겨찾는 집이나 를 위해 찾은 집도 가져올 수 있습니다. Unity로 가져올 수 있는 경우 이러한 방식으로 Altspace로 가져올 수 있습니다. 다음은 몇 가지 [예제 Worlds 입니다.](https://account.altvr.com/worlds/1046572460192825569)

![예제 세계](images/unity-uploader-img-01.png)

## <a name="setup"></a>설치 프로그램

1. 공식 [AltspaceVR Discord에](https://discordapp.com/invite/altspacevr) 조인하고 #world 빌드 채널을 방문합니다. 친구만 세계를 빌드할 수 있습니다.
2. 기본 사항의 [세계 빌드 시작 가이드를](world-building-getting-started.md) 참조하세요.
3. [Unity Hub를 설치하고](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) **Unity 2020.3.9를** 설치합니다. 이 버전과 정확하게 일치하지 않으면 업로더가 작동하지 않습니다. Unity 계정이 없는 경우 무료 Unity 계정이 필요하며, 이 작업을 수행하므로 **개인을** 선택합니다. 설치하는 동안 **Android 빌드** 옵션을 확인하고 자동 업데이트를 사용하지 않도록 설정해야 합니다.
4. [최신 Unity 업로더 다운로드](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. 웹 사이트에서 [템플릿을 만듭니다.](https://account.altvr.com/space_templates/new) 이름을 **템플릿 Hello World** 지정합니다.
6. [World를 만들고](https://account.altvr.com/worlds/my) 이름을 **로 Hello World.** **템플릿으로 Hello World** 템플릿을 선택합니다.

![만든 세계 화면](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>장면 업로드

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Unity Hub를 열고 새 Unity 2020.3.9 프로젝트를 만듭니다.
2. 프로젝트를 연 후 다운로드한 파일(Unity 패키지)을 두 번 클릭하여 업로더를 가져옵니다. 이제 **AltspaceVR이라는** 새 탭이 표시됩니다. Altspace와 함께 사용하려는 모든 Unity 프로젝트에 대한 패키지를 가져와야 합니다.
3. **메뉴 > AltspaceVR > 빌드 설정**
4. Altspace 계정 자격 증명으로 로그인
5. **템플릿 로드를** 선택한 다음, **Hello World 템플릿을** 선택합니다.
6. 장면에 큐브를 추가하고 저장합니다.
7. **Windows 빌드를** 확인하고 **Android용 빌드를 선택 취소합니다.**
8. **업로드** 를 선택합니다. 약 1분 후에 **완료된 업로드** 표시됩니다.
9. **Altspace를** 시작하고 Menu > **Worlds > My Worlds에서 를** 입력하여 Hello World 조인
10. 메뉴 > 설정 > **보통 > 다시 설정 공간에서** 세계 다시 설정
11. 큐브가 표시됩니다. 위의 비디오에서처럼 빠르게 수행하는 경우 10초 이내에 변경 내용을 볼 수 있습니다.

## <a name="whats-supported"></a>지원되는 내용

* 예: 모델, 충돌, 애니메이션, 파티클 효과, 오디오, skyboxes 등
* 아니요: 스크립트. 보안을 위해 스크립트를 포함하는 업로드는 거부됩니다.
* 아마도 동적 글로벌 조명과 같은 멋진 것일 수 있습니다.
* 서로 다른 플랫폼에 대해 개별적으로 또는 함께 장면 업로드
* [업로더를](https://account.altvr.com/worlds/featured)사용하여 빌드된 주요 세계 를 참조하세요.

## <a name="tips"></a>팁

* 공식 [AltspaceVR Discord](https://discordapp.com/invite/altspacevr)에 조인합니다.
* 왼쪽의 템플릿 페이지에는 플랫폼별 최신 업로드가 표시됩니다. 성공하면 **1-2분 전이 표시됩니다.** Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![업로드가 강조 표시된 템플릿 패널 열기](images/unity-uploader-img-03.png)

* 업데이트할 때 세계일 수 있습니다. 업로더가 **업로드 완료라고** 말하는 순간 전 세계를 다시 설정하여 변경 내용을 확인할 수 있습니다.
* 간단한 장면으로 PC 전용 빌드는 Altspace의 변경이 표시되는 데 1분 미만이 소요됩니다.
* 방해를 피하기 위해 세계를 프라이빗 및 비공개로 설정합니다.
* 사용자가 기본적으로 생성되는 위치를 볼 수 있도록 큐브를 원점 에 배치합니다. 업로드할 때 큐브를 숨깁니다.

## <a name="troubleshooting"></a>문제 해결

**내가 넘어지거나 어떤 것에도 원격으로 전송할 수 없습니다.** 개체에 충돌을 추가하여 개체에 원격으로 전송해야 합니다.

**아무것도 변경되지 않습니다.**
    * Unity에서 장면을 저장했나요?
    * 테스트할 플랫폼을 선택했나요?
    * 올바른 세계에 있나요? 업로더 및 세계 양식에서 올바른 템플릿을 선택했나요?
    * 템플릿 페이지 통계를 확인했나요?

**업로드 실패 또는 시간 부족**
    * 가장 일반적인 업로드 오류는 잘못된 Unity 버전이 있는 것입니다. 필요한 버전과 정확히 일치해야 합니다.
    * 업로드가 너무 클 수 있습니다. PC 장면을 100MB < 유지해 보세요. 작게 시작하고 빌드합니다. 최적화, 최적화, 최적화.
    * 간단한 큐브가 있는 새 프로젝트를 사용해 보세요.
    * 빌드 중에 강제로 종료하지 마세요. 장면을 손상할 수 있습니다. 다시 업로드해 보세요.

**느린 프로세스입니다.**
    * PC용으로 빌드하는 동안에만 빌드하고 나중에 Android용으로 빌드하는 것이 좋습니다.
    * 사용하지 않는 파일을 제거해 보세요. 어떤 이유로든 Unity는 때때로 지나치게 됩니다.

**내 Altspace 자격 증명으로 로그인할 수 없습니다.**
    * 전자 메일은 대/소문자를 구분합니다.
    * 새 프로젝트를 사용해 보세요.
    * Altspace 계정이 양호한지 확인합니다.

## <a name="see-also"></a>추가 정보

* [Unity Learn](https://unity3d.com/learn)
* [Unity 포럼](https://forum.unity.com)
