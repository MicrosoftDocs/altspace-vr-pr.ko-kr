---
title: Altspace Uploader 소개
description: Altspace Uploader와 함께 Unity 장면 템플릿을 사용하여 AltspaceVR 세계를 설정하고 업로드하는 방법을 알아봅니다.
ms.date: 10/29/2021
ms.author: v-vtieto
ms.topic: article
ms.openlocfilehash: 6d28b3efe75d589a0a09d4969add5d043a3116d0
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278965"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace Uploader 소개

> [!NOTE]
> - 관심이 있는 경우 [공식 AltspaceVR Discord에](https://discordapp.com/invite/altspacevr) 조인하고 #world 빌드 채널을 방문하세요.  
> - 이전 공간을 복원하려는 경우 [업그레이드 가이드](upgrading-old-unity-projects.md)를 참조하세요. 

업로더를 사용하면 Unity 장면을 전 세계에 대한 템플릿으로 사용할 수 있습니다. Minecraft 즐겨찾는 만들기 또는 를 위해 찾은 집으로 가져올 수 있습니다. Unity로 가져올 수 있는 경우 이러한 방식으로 Altspace로 가져올 수 있습니다. 다음은 몇 가지 [예제 Worlds 입니다.](https://account.altvr.com/worlds/1046572460192825569)

![예제 세계](images/unity-uploader-img-01.png)

## <a name="setup"></a>설치 프로그램

1. 공식 [AltspaceVR Discord에](https://discordapp.com/invite/altspacevr) 조인하고 #world 빌드 채널을 방문합니다. 친구만이 세계를 빌드하도록 허용하지 않습니다.
2. 기본 사항의 [세계 빌드 시작 가이드를](world-building-getting-started.md) 참조하세요.
3. [Unity Hub를 설치하고](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) [**2020.3.18f1을 설치합니다.**](https://unity3d.com/unity/whats-new/2020.3.18) 이 버전과 정확하게 일치하지 않으면 업로더가 작동하지 않습니다. Unity 계정이 없는 경우 무료 Unity 계정이 필요하고, 재미있는 작업을 수행하므로 **개인을** 선택해야 합니다. 설치하는 동안 **Android 빌드** 옵션을 확인하고 자동 업데이트를 사용하지 않도록 설정해야 합니다.
    * Android **빌드 지원** 모듈을 포함합니다.
    * Windows **Mac 빌드 지원(Mono)** 모듈을 포함합니다.
    * Mac에서는 Windows **빌드 지원(Mono)** 모듈을 포함합니다.
4. [최신 Unity 업로더 다운로드](https://altvr.com/download-latest-unity-uploader)
5. 웹 사이트에서 [템플릿을 만듭니다.](https://account.altvr.com/space_templates/new) 이름을 **템플릿 Hello World** 지정합니다.
6. [World를 만들고](https://account.altvr.com/worlds/my) 이름을 **로 Hello World.** **템플릿으로 Hello World** 템플릿을 선택합니다.

![만든 세계 화면](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>장면 업로드

> [!NOTE]
> 자세한 단계별 가이드는 [여기에서](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)찾을 수 있습니다.

1. Unity Hub를 열고 새 Unity 2020.3.9 프로젝트를 만듭니다. 템플릿에 대해 **유니버설 렌더링 파이프라인** 을 선택합니다.

    ![URP Unity 템플릿 선택](images/001-unity-templates.png)

1. Altspace Uploader를 다운로드한 폴더로 이동한 다음 해당 폴더에서 새 Unity 프로젝트의 루트 폴더로 복사하거나 이동합니다.
1. 메뉴 모음의 Unity에서 **창**  >  **패키지 관리자 선택합니다.**
1. 패키지 관리자 메뉴 모음에서 더하기 기호 드롭다운("+")을 선택한 다음 **tarball에서 패키지 추가를** 선택합니다.
1. Altspace Uploader가 포함된 폴더로 이동한 다음 업로더를 선택한 다음 **열기를** 클릭합니다.  패키지가 로드된 후 메뉴 모음에 **AltspaceVR이** 표시됩니다.

    ![메뉴 모음의 AltspaceVR](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Altspace 업로더 패키지를 Altspace와 함께 사용하려는 모든 Unity 프로젝트로 가져와야 합니다.
1. 메뉴 모음에서 **AltspaceVR > 템플릿을 선택합니다.**
1. **Altspace VR 템플릿** 대화 상자에서 Altspace 계정 자격 증명으로 로그인합니다. (MSA 로그인은 곧 제공될 예정입니다. Microsoft 계정 사용하여 Altspace에 로그인한 적이 있는 경우 웹 사이트의 "암호 잊음" 옵션을 사용하여 암호를 만들어야 합니다.)
1. 템플릿 **선택 드롭다운을** 클릭한 다음 템플릿 **Hello World** 선택합니다.
1. 장면을 선택합니다. **.unity 파일** 타원 선택 단추(점 세 개)를 클릭한 다음, 프로젝트의 **Assets**  >  **Scenes** 폴더로 이동한 다음, **SampleScene.unity를** 선택하여 엽니다.
1. **플랫폼용 빌드:** 에서 **Windows** 선택되어 있는지 확인합니다. 지금은 다른 두 옵션인 **Android** 및 **Mac** 을 **선택하지 않아야** 합니다. 사람들이 방문하도록 하려면 모든 플랫폼에 대해 빌드하고 업로드해야 합니다."
1. 빌드 **& 업로드** 단추를 선택합니다. 이 프로세스는 1~2분 정도 걸릴 수 있습니다.
1. Altspace를 시작하고 **주 메뉴** 를 선택한 다음, 메뉴 모음에서 **내 세계** 를 선택합니다.
1. **Hello World** 이동한 다음 엽니다.

    장면은 Unity 편집기에서 본 것과 비슷해야 합니다.

## <a name="whats-supported"></a>지원되는 내용

* 예: 모델, 충돌, 애니메이션, 파티클 효과, 오디오, skyboxes 등입니다.
* 아니요: 스크립트. 보안을 위해 스크립트를 포함하는 업로드가 거부됩니다.
* 아마도 동적 글로벌 조명과 같은 멋진 것일 수 있습니다.
* 서로 다른 플랫폼에 대한 장면을 개별적으로 또는 함께 업로드.
* [추천 세계 를 참조하세요.](https://account.altvr.com/worlds/featured) 많은 것이 업로더를 사용하여 빌드되었습니다.

## <a name="tips"></a>팁

* 공식 [AltspaceVR Discord](https://discordapp.com/invite/altspacevr)에 조인합니다.
* 왼쪽의 템플릿 페이지에는 플랫폼별 최신 업로드가 표시됩니다. 성공하면 **1-2분 전이 표시됩니다.** 

![업로드가 강조 표시된 템플릿 패널 열기](images/template-upload-list.png)

* 업데이트할 때 세계일 수 있습니다. 업로더가 **업로드 완료라고** 말하는 순간 전 세계를 다시 설정하여 변경 내용을 확인할 수 있습니다.
* 간단한 장면으로 PC 전용으로 빌드하는 경우 Altspace의 변경이 표시되는 데 1분 미만이 소요됩니다.
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
    * 가장 일반적인 업로드 오류는 잘못된 Unity 버전으로 인한 것입니다. 필요한 버전과 정확히 일치해야 합니다.
    * 업로드가 너무 클 수 있습니다. PC 장면을 100MB < 유지해 보세요. 작게 시작하고 빌드합니다. 최적화, 최적화, 최적화.
    * 간단한 큐브가 포함된 새 프로젝트를 사용해 보세요.
    * 빌드 중에 강제로 종료하지 마세요. 장면을 손상할 수 있습니다. 다시 업로드해 보세요.

**느린 프로세스입니다.**
    * PC용으로 빌드하는 동안에만 빌드하고 나중에 Android용으로 빌드하는 것이 좋습니다.
    * 사용하지 않는 파일을 제거해 보세요. 어떤 이유로든 Unity는 때때로 지나치게 됩니다.

**내 Altspace 자격 증명으로 로그인할 수 없습니다.**
    * 전자 메일은 대/소문자를 구분합니다.
    * 새 프로젝트를 사용해 보세요.
    * Altspace 계정이 양호한지 확인합니다.

## <a name="see-also"></a>참고 항목

* [Unity Learn](https://unity3d.com/learn)
* [Unity 포럼](https://forum.unity.com)  
