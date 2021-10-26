---
title: Altspace 업 로더 소개
description: Altspace 업 로더를 사용 하 여 Unity 장면 템플릿을 사용 하 여 AltspaceVR 환경을 설정 하 고 업로드 하는 방법에 대해 알아봅니다.
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: 도구 키트, Altspace, 업 로더
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298819"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace 업 로더 소개

> [!NOTE]
> - 관심이 있는 경우 [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world-빌딩 채널을 방문 하세요.  
> - 이전 공간을 액세스 권한을 복원 하려는 경우 [업그레이드 가이드](upgrading-old-unity-projects.md)를 참조 하세요. 

업 로더를 사용 하 여 전 세계의 템플릿으로 Unity 장면을 사용할 수 있습니다. Minecraft에서 파티 또는 선호 하는 생성을 위해 haunted를 가져올 수 있습니다. Unity로 가져올 수 있는 경우 이러한 방식으로 Altspace으로 가져올 수 있습니다. 다음은 몇 가지 [예](https://account.altvr.com/worlds/1046572460192825569)입니다.

![예제 세계](images/unity-uploader-img-01.png)

## <a name="setup"></a>설치 프로그램

1. [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world-빌딩 채널을 방문 하세요. Friend를 사용 하는 경우에만 친구를 빌드할 수 있습니다.
2. 기본 사항에 대 한 [시작 하기 가이드](world-building-getting-started.md) 를 참조 하십시오.
3. [Unity Hub](https://unity3d.com/get-unity/download) 및 **Unity 2020.3.9** 를 설치 합니다. 이 버전을 정확 하 게 일치 하지 않으면 업 로더가 작동 하지 않습니다. 없는 경우 무료 Unity 계정이 필요 합니다. 설치 하는 동안 **개인** 버전 (재미를 위해이 작업을 수행 하 고 있으므로)을 선택 하 고 다음을 수행 해야 합니다.
    * **Android 빌드 지원** 모듈을 포함 합니다.
    * Windows에서 **Mac 빌드 지원 (Mono)** 모듈을 포함 합니다.
    * Mac에 **Windows 빌드 지원 (Mono)** 모듈을 포함 합니다.
4. [AltspaceVR 업 로더 다운로드](https://aka.ms/AvrUrpUploader)
5. 웹 사이트에서 [템플릿을 만듭니다](https://account.altvr.com/space_templates/new) . **템플릿을 헬로 월드** 으로 이름을로 합니다.
6. [세계를 만들고](https://account.altvr.com/worlds/my) **헬로 월드** 이름을로 합니다. 템플릿으로 **헬로 월드 템플릿을** 선택 합니다.

![만든 세계 화면](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>장면 업로드

> [!NOTE]
> 자세한 단계별 가이드는 [여기](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)에서 찾을 수 있습니다.

1. Unity 허브를 열고 새 Unity 2020.3.9 프로젝트를 만듭니다. 템플릿의 경우 **유니버설 렌더링 파이프라인** 을 선택 합니다.

    ![URP Unity 템플릿 선택](images/001-unity-templates.png)

1. Altspace 업 로더를 다운로드 한 폴더로 이동한 후 해당 폴더에서 새 Unity 프로젝트의 루트 폴더로 복사 하거나 이동 합니다.
1. Unity의 메뉴 모음에서 **창** 패키지 관리자를 선택  >  **합니다.**
1. 패키지 관리자 메뉴 모음에서 더하기 기호 드롭다운 ("+")을 선택 하 고 **tarball에서 패키지 추가** 를 선택 합니다.
1. Altspace 업 로더를 포함 하는 폴더로 이동한 후 업 로더를 선택 하 고 **열기** 를 클릭 합니다.  패키지가 로드 되 면 메뉴 모음에 **AltspaceVR** 나타납니다.

    ![메뉴 모음의 AltspaceVR](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Altspace에 사용 하려는 모든 Unity 프로젝트에 Altspace 업 로더 패키지를 가져와야 합니다.
1. 메뉴 모음에서 **AltspaceVR > 템플릿** 을 선택 합니다.
1. **ALTSPACE VR 템플릿** 대화 상자에서 altspace 계정 자격 증명으로 로그인 합니다. MSA 로그인은 곧 제공 될 예정입니다. Microsoft 계정를 사용 하 여 Altspace에 로그인 한 경우에는 웹 사이트에서 "암호 잊음" 옵션을 사용 하 여 암호를 만들어야 합니다.
1. **템플릿 선택** 드롭다운을 클릭 한 다음 **템플릿 헬로 월드** 을 선택 합니다.
1. 장면 선택: **unity 파일** 줄임표 단추 (세 개의 점)를 클릭 한 다음 프로젝트의 **자산**  >  **장면** 폴더로 이동한 다음 **SampleScene** 를 선택 하 여 엽니다.
1. **플랫폼용 빌드:** 에서 **Windows** 가 선택 되어 있는지 확인 합니다. 지금은 **Android** 및 **Mac** 의 다른 두 옵션을 선택 **하면 안 됩니다** . 사용자가 방문 하려면 모든 플랫폼에 대해 빌드 및 업로드 해야 합니다. "
1. **빌드 & 업로드** 단추를 선택 합니다. 이 프로세스는 1 ~ 2 분 정도 걸릴 수 있습니다.
1. Altspace를 시작한 다음 **주 메뉴** 를 선택 하 고 메뉴 모음에서 **내 세계** 를 선택 합니다.
1. **헬로 월드** 로 이동 하 여 엽니다.

    장면은 Unity 편집기에서 본 것과 비슷해야 합니다.

## <a name="whats-supported"></a>지원되는 내용

* 예: 모델, 충돌, 애니메이션, 파티클 효과, 오디오, skyboxes 등
* 아니요: 스크립트 보안을 위해 스크립트가 포함 된 업로드가 거부 됩니다.
* 예: 동적 전 세계 조명과 같은 멋진 사물입니다.
* 다른 플랫폼에 대해 개별적으로 또는 함께 장면을 업로드 합니다.
* [추천](https://account.altvr.com/worlds/featured)항목을 참조 하세요. 대부분은 업 로더를 사용 하 여 빌드 되었습니다.

## <a name="tips"></a>팁

* [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr)에 참여 합니다.
* 왼쪽의 템플릿 페이지에서 플랫폼별 최신 업로드를 표시 합니다. 성공적으로 완료 되 면 **1-2 분 전에** 표시 됩니다. 

![업로드가 강조 표시 된 템플릿 패널 열기](images/template-upload-list.png)

* 업데이트 시에는 전 세계에 있을 수 있습니다. 업 로더가 **업로드 완료** 되는 순간에 변경 내용을 볼 수 있도록 전 세계를 다시 설정할 수 있습니다.
* 간단한 장면을 사용 하 여 PC 전용으로 빌드하는 경우에는 Altspace의 변경을 확인 하는 데 1 분 미만이 소요 됩니다.
* 혼란을 피하기 위해 전 세계를 개인 또는 목록으로 설정 합니다.
* 사용자가 기본적으로 생성 하는 위치를 확인할 수 있도록 원본에 큐브를 추가 합니다. 업로드할 때 큐브를 숨깁니다.

## <a name="troubleshooting"></a>문제 해결

**거의 모든 항목으로 텔레포트 할 수 없습니다** . 이로 텔레포트 하려면 개체에 충돌을 추가 해야 합니다.

**변경 내용 없음**
    * 장면을 Unity에 저장 했습니까?
    * 테스트 중인 플랫폼을 선택 하셨습니까?
    * 올바른 세계에 있나요? 업 로더 및 세계 양식에서 적합 한 템플릿을 선택 했습니까?
    * 템플릿 페이지 통계를 확인 했나요?

**업로드 실패 또는 시간 초과**
    * 가장 일반적인 업로드 오류는 잘못 된 Unity 버전이 있는 경우에 발생 합니다. 필요한 버전과 정확 하 게 일치 해야 합니다.
    * 업로드가 너무 클 수 있습니다. PC 장면을 100 < 유지 하세요. Small 및 build를 시작 합니다. 최적화, 최적화, 최적화.
    * 간단한 큐브가 포함 된 새 프로젝트를 사용해 보세요.
    * 빌드 중에 강제 종료 하지 마세요. 장면을 손상 시킬 수 있습니다. 다시 업로드 해 보세요.

**속도가 느립니다.**
    * 나중에 Android를 반복 하는 동안에만 PC 용을 빌드하는 것이 좋습니다.
    * 사용 하지 않는 파일을 제거해 보세요. 어떤 이유로 든 Unity는 때때로 overzealous을 가져옵니다.

**내 Altspace 자격 증명을 사용 하 여 로그인 할 수 없습니다.**
    * 전자 메일은 대/소문자를 구분 합니다.
    * 새 프로젝트를 사용해 보세요.
    * Altspace 계정이 정상 상태 인지 확인 합니다.

## <a name="see-also"></a>추가 정보

* [Unity Learn](https://unity3d.com/learn)
* [Unity 포럼](https://forum.unity.com)  
