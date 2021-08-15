---
title: 최신 Unity 버전으로 콘텐츠 업데이트
description: 콘텐츠를 최신 버전의 Unity로 업데이트하는 방법을 알아봅니다.
ms.date: 06/4/2021
ms.topic: article
keywords: 키트, 세계, unity, 업데이트, 셰이더, 업로더, 문제 해결
ms.openlocfilehash: a10e64b4dc19e256dcae9d61620de0140db60ccc0bf2a10dc864313f139bbd10
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126764"
---
# <a name="updating-content-to-the-latest-unity-version"></a>최신 Unity 버전으로 콘텐츠 업데이트

## <a name="moving-to-unity-202039"></a>Unity 2020.3.9로 이동

오늘부터 AltspaceVR은 최신 버전의 Unity(2020.3.9)로 업그레이드되었습니다. 이 업데이트는 몇 가지 성능 향상 외에도 통합하게 되어 기쁩니다. 이 변경 내용은 모든 기존 콘텐츠와 호환되어야 합니다. 그렇지 않은 경우 지원 담당자에게 문의하세요 altvr.com/support

2020.3.9로의 이 이동은 사용자 생성 콘텐츠에 영향을 미치지 않았지만, 몇 주 후에 사용자가 콘텐츠를 업데이트해야 하는 AltspaceVR의 [스테레오 렌더링 모드를]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)변경합니다. [Single Pass Instancing으로](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 업그레이드하면 전 세계에서 성능이 크게 향상될 수 있습니다. 이 새 빌드는 더 이상 2019.4 및 이전 버전 콘텐츠와의 호환성을 지원하지 않습니다. 주요 변경 내용을 방지하기 위해 가능한 한 빨리 모든 작성자 소유 콘텐츠를 업데이트해야 합니다. 아래 가이드에 따라 콘텐츠를 업데이트하고 Unity 2020.3.9에서 Single Pass Instancing으로 원활하게 전환할 수 있습니다.

> [!NOTE]
> 다른 사람이 소유하고 사용자와 공유한 콘텐츠를 정기적으로 사용하는 경우 world/kit 소유자에게 문의하여 콘텐츠를 업데이트할 계획인지 확인합니다.

> 콘텐츠 작성자이며 질문이 있거나 도움이 필요한 경우 지원 팀에 문의하세요. altvr.com/support

## <a name="testing-your-spi-content"></a>SPI 콘텐츠 테스트

다음 미리 보기 버전의 AltspaceVR을 사용하여 VR에서 새로 업데이트된 콘텐츠를 테스트합니다. 미리 보기 버전은 테스트 목적으로만 사용되며 플랫폼의 일반적인 용도로 사용하면 안 됩니다.

* [Windows Mixed Reality 대한 AltspaceVR SPI 미리 보기](https://aka.ms/AvrSpiMr)
* [AltspaceVR SPI Preview for SteamVR](https://aka.ms/AvrSpiSteam)
* [Oculus 표시를 위한 AltspaceVR SPI 미리 보기](https://aka.ms/AvrSpiRift)

> 참고: PC VR 미리 보기만 제공되었습니다. 단일 패스 인스턴스 렌더링은 Android에서 사용할 수 없으며 Mac과 같은 비 VR 플랫폼에서는 필요하지 않습니다. 따라서 일반 릴리스 버전을 사용하여 이러한 디바이스를 테스트할 수 있습니다.


## <a name="storecompatibilitycheck"></a>저장소 호환성 검사

Unity 2020.3.9로 업그레이드하면 헤드셋 및 스토어 빌드 호환성에도 영향을 줍니다. 이제 헤드셋과 호환되는 스토어에서 AltspaceVR을 다운로드해야 합니다. 예를 들어 WinMR 또는 Oculus 헤드셋의 경우 각각 Windows Store 또는 Oculus Store에서 AltspaceVR을 다운로드합니다. Windows Mixed Reality 사용자는 Windows Store에서 AltspaceVR, Steam의 SteamVR 사용자 및 Oculus Store에서 Oculus 표시 사용자를 다운로드해야 합니다.

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR 업로더 v0.9.0 업그레이드 가이드 

업로더 0.9는 이전 버전의 업로더와 다르게 패키지됩니다. 이 패키징 변경과 동시에 새 업로더에는 새 버전의 Unity가 필요합니다. 이 가이드는 관련된 모든 사용자에 대해 이 업그레이드 프로세스를 더 원활하고 안전하게 만들기 위한 것입니다.

1. **프로젝트 백업** - 전체 프로젝트 디렉터리 복사본을 만들고 안전한 곳에 배치합니다. 이 업그레이드는 파괴적 업그레이드이므로 완료한 후에는 Unity 2019.4용 번들을 만들거나 업로드할 수 없습니다. 이 업그레이드 중에 문제가 발생하는 경우 다시 사용할 프로젝트의 클린 복사본이 필요합니다. 또한 AltspaceVR이 Unity 2020.3.9로 공식적으로 업그레이드하기 전에 라이브 키트 또는 템플릿을 업데이트하는 데 필요합니다.

2. **REMOVE OLD UPLOADER** - Unity를 닫은 후 다음 파일/폴더를 삭제하고 해당하는 .meta 파일입니다.

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **엔진 버전 다운로드** - Unity Hub를 열고 Unity 2020.3.9를 설치합니다(또는 [여기를 클릭하여](https://unity3d.com/ru/unity/whats-new/2020.3.9) 직접 설치).

4. **프로젝트 업그레이드** - Unity 2020.3.9에서 정리된 프로젝트를 열고 Unity에서 프로젝트를 업그레이드하도록 허용합니다.

5. (PC만 해당) **MIXED REALITY FEATURE TOOL 다운로드** - 지침에 따라 업로더 패키지의 설치를 관리하는 데 사용할 [Mixed Reality 기능 도구를](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)다운로드합니다.

6. **UPLOADER 설치** - MR 기능 도구를 사용하여 Unity 프로젝트를 선택하고 AltspaceVR 업로더 기능을 추가합니다(AltspaceVR 제목 아래). 도구의 지침을 따릅니다.

macOS에서는 [레지스트리에서](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)최신 버전을 수동으로 다운로드하고 Unity 편집기 패키지 관리자 내에서 설치합니다(Windows > 패키지 관리자 > + > tarball에서 패키지 추가).

패키지 가져오기가 완료되면 AltspaceVR 메뉴 항목에서 친숙한 업로더 창을 사용할 수 있어야 합니다.

## <a name="troubleshooting-tips"></a>문제 해결 팁

1. WinMR 헤드셋에 컨트롤러 또는 입력 문제가 있는 경우 현재 상태 센서를 제대로 연결하기 위해 헤드에 있는지 확인합니다. 이는 알려진 문제이며 Microsoft는 이 문제를 해결하기 위해 적극적으로 노력하고 있습니다.

2. 헤드셋 및 스토어 빌드 호환성을 확인합니다. 예를 들어 WinMR 헤드셋을 사용하는 경우 Windows Store를 통해 AltspaceVR 빌드를 획득했는지 확인합니다.

3. 테스트 중에 콘텐츠가 VR 모드에서 한 눈에만 나타나는 경우 사용하는 사용자 지정 셰이더가 SPI 렌더링을 지원하지 않을 수 있습니다. 다른 셰이더를 선택하거나 [Unity의 SPI 업그레이드 가이드에](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 따라 셰이더를 수동으로 편집하고 지원을 추가해야 합니다.

4. WinMR의 경우 AltspaceVR에서 VR 모드에 액세스하려면 먼저 다음을 수행해야 합니다. 
    1. Microsoft Store Windows Mixed Reality OpenXR을 다운로드하여 설치합니다.
        1. Mixed Reality 포털 앱 열기
        2. 앱의 왼쪽 아래 모서리에서 "자세히 보기"를 선택합니다.
        3. 표시되는 메뉴에서 OpenXR 설정을 선택합니다. 이렇게 하면 런타임을 설치할 수 있는 위치에서 Windows Store가 시작됩니다. 이 메뉴 항목이 표시되지 않으면 OpenXR이 PC에 이미 설치되어 있을 수 있습니다.