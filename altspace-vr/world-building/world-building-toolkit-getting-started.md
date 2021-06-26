---
title: 세계 개발 도구 키트 소개
description: 전 세계의 도구 키트와 함께 Unity 장면 템플릿을 사용 하 여 AltspaceVR 환경을 설정 하 고 업로드 하는 방법에 대해 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 도구 키트
ms.openlocfilehash: 3b41f02aec1077a37b95a6826c105e1cd31974e3
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923080"
---
# <a name="introducing-the-world-building-toolkit"></a>세계 개발 도구 키트 소개

> [!NOTE]
> 세계 개발 도구 키트는 microsoft에서 제공 하는 [Anthony Madden](https://twitter.com/chigamesstudio)에 의해 실행 되는 커뮤니티 프로젝트입니다. 관심이 있는 경우 [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world-빌딩 채널을 방문 하세요. 현재 Mac 평가판 베타를 제공 하 고 있습니다. [자세한 정보](https://altvr.com/altspacevr-mac)

업 로더를 사용 하 여 전 세계의 템플릿으로 Unity 장면을 사용할 수 있습니다. Minecraft에서 파티를 즐겨 사용 하거나 즐겨 사용 하는 haunted를 만들 수 있습니다. Unity로 가져올 수 있는 경우 이러한 방식으로 Altspace으로 가져올 수 있습니다. 다음은 몇 가지 [예](https://account.altvr.com/worlds/1046572460192825569)입니다.

![예제 세계](images/unity-uploader-img-01.png)

## <a name="setup"></a>설치 프로그램

1. [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world을 방문 하세요. 친구는 친구 들이 혼자 빌드할 수 있습니다.
2. 기본 사항에 대 한 [시작 하기 가이드](world-building-getting-started.md) 를 참조 하십시오.
3. [Unity 허브를 설치](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 하 고 **unity 2020.3.9** 를 설치 합니다. 이 버전을 정확 하 게 일치 하지 않으면 업 로더가 작동 하지 않습니다. 무료 Unity 계정이 없으면 무료 Unity 계정이 필요 하 고, 재미를 위해이 작업을 수행 하므로 **개인** 을 선택 합니다. 설치 하는 동안 **Android 빌드** 옵션을 선택 하 고 자동 업데이트를 사용 하지 않도록 설정 해야 합니다.
4. [최신 Unity 업 로더 다운로드](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. 웹 사이트에서 [템플릿을 만듭니다](https://account.altvr.com/space_templates/new) . **템플릿을 헬로 월드** 으로 이름을로 합니다.
6. [세계를 만들고](https://account.altvr.com/worlds/my) **헬로 월드** 이름을로 합니다. 템플릿으로 **헬로 월드 템플릿을** 선택 합니다.

![만든 세계 화면](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>장면 업로드

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Unity 허브를 열고 새 Unity 2020.3.9 프로젝트를 만듭니다.
2. 프로젝트를 연 상태에서 다운로드 한 파일을 두 번 클릭 하 여 업 로더를 가져옵니다 (Unity 패키지). 이제 **AltspaceVR** 라는 새 탭이 표시 됩니다. Altspace와 함께 사용 하려는 모든 Unity 프로젝트에 대 한 패키지를 가져와야 합니다.
3. **메뉴 > AltspaceVR > 빌드 설정** 열기
4. Altspace 계정 자격 증명으로 로그인 합니다.
5. **템플릿 로드** 를 선택한 다음 **헬로 월드 템플릿** 을 선택 합니다.
6. 장면에 큐브를 추가 하 고 저장 합니다.
7. **Windows 용 빌드** 를 선택 하 고 **Android 용 빌드** 를 선택 취소 합니다.
8. **업로드** 를 선택합니다. 약 1 분 후 **업로드가** 완료 된 것을 볼 수 있습니다.
9. Altspace를 시작 하 고 **내 세계 > 메뉴 >** 를 입력 하 여 **헬로 월드** 를 조인 합니다.
10. **메뉴 > 설정 > 중간 > 공간 다시** 설정에서 전 세계를 다시 설정 합니다.
11. 큐브가 표시 되어야 합니다. 위의 비디오에서 빨리이 작업을 수행 하는 경우 10 초 내에 변경 내용을 볼 수 있습니다.

## <a name="whats-supported"></a>지원되는 내용

* 예: 모델, 충돌, 애니메이션, 파티클 효과, 오디오, skyboxes 등
* 아니요: 스크립트 보안을 위해 스크립트가 포함 된 업로드가 거부 됩니다.
* 예: 동적 전 세계 조명 등의 화려한 사물
* 다른 플랫폼에 대 한 장면을 개별적으로 또는 함께 업로드
* 업 [로더를 사용](https://account.altvr.com/worlds/featured)하 여 많은 기능을 빌드 했습니다.

## <a name="tips"></a>팁

* [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr)에 참여 합니다.
* 왼쪽의 템플릿 페이지에서 플랫폼별 최신 업로드를 표시 합니다. 성공적으로 완료 되 면 **1-2 분 전에** 표시 됩니다. Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![업로드가 강조 표시 된 템플릿 패널 열기](images/unity-uploader-img-03.png)

* 업데이트 시에는 전 세계에 있을 수 있습니다. 업 로더가 **업로드가 완료** 되 면 변경 내용을 볼 수 있도록 전 세계를 다시 설정할 수 있습니다.
* 간단한 장면을 사용 하 여 PC 전용으로 빌드하면 Altspace가 변경 되는 데 1 분 미만이 소요 됩니다.
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
    * 가장 일반적인 업로드 오류에 잘못 된 Unity 버전이 있습니다. 필요한 버전과 정확 하 게 일치 해야 합니다.
    * 업로드가 너무 클 수 있습니다. PC 장면을 100 < 유지 하세요. Small 및 build를 시작 합니다. 최적화, 최적화, 최적화.
    * 간단한 큐브로 새 프로젝트를 사용해 보세요.
    * 빌드 중에 강제 종료 하지 마세요. 장면을 손상 시킬 수 있습니다. 다시 업로드 합니다.

**속도가 느립니다.**
    * 나중에 Android를 반복 하는 동안에만 PC 용을 빌드하는 것이 좋습니다.
    * 사용 하지 않는 파일을 제거해 보세요. 어떤 이유로 Unity가 overzealous를 가져오는 경우도 있습니다.

**내 Altspace 자격 증명을 사용 하 여 로그인 할 수 없습니다.**
    * 전자 메일은 대/소문자를 구분 합니다.
    * 새 프로젝트를 사용해 보세요.
    * Altspace 계정이 정상 상태 인지 확인 합니다.

## <a name="see-also"></a>참조

* [Unity 학습](https://unity3d.com/learn)
* [Unity 포럼](https://forum.unity.com)
