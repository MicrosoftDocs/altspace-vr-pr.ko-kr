---
title: AltspaceVR 오디오에 대한 질문과 대답
description: 오디오 관련 문제에 대한 문제 해결 및 지원
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr, 오디오, 문제 해결, 지원
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311909"
---
# <a name="frequently-asked-questions-about-audio"></a>오디오에 대한 질문과 대답

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>VR 헤드셋에 기본 제공 마이크가 있나요?

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus Quest/HtC Vive, Oculus Quest/Quest 2, Windows Mixed Reality 및 HTC Vive

예, 이러한 VR 헤드셋에는 기본 제공 마이크가 있습니다.

### <a name="windows"></a>Windows

Windows 함께 사용되는 헤드셋의 경우 헤드셋을 연결하는 동안 **녹음 디바이스** 아래에 나열된 마이크를 찾을 수 있어야 합니다.

### <a name="further-troubleshooting"></a>추가 문제 해결

* [AltspaceVR 지원 - 다른 사용자가 내 말을 들어도 안 돼요.](#what-do-i-do-if-other-users-cant-hear-me)
* [AltspaceVR 지원 - Oculus Quest에 대한 권한 관리](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>PTT(Push-to-Talk) 단추가 있나요?

압정 단추가 없습니다.  보기의 왼쪽 아래를 보면 음성을 토글하는 데 사용할 수 있는 마이크 아이콘이 있습니다. 또는 바로 가기 키인 스페이스바를 사용하여 마이크를 음소거/음소거 해제할 수 있습니다.

대화할 때 아이콘이 깜박이면 마이크가 작동합니다.
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>내 오디오가 고가용성인 경우 어떻게 해야 합니까?

일부 사용자는 다른 아바타가 말하는 경우 오디오가 퇴사하거나 정기적인 드롭아웃으로 인해 발생한다는 것을 알아차렸습니다. 다른 경우에는 다른 사용자가 자신의 오디오가 음해 또는 로봇을 통해 들어오고 있음을 알릴 수 있습니다.

가장 먼저 시도해야 할 것은 항상 현재 있는 공간을 다시 표시하거나, 실패할 경우 AltspaceVR을 다시 시작하는 것입니다. 오디오 문제는 일반적이지 않지만 문제가 발생하는 경우 쉽게 해결할 수 있는 경우가 많습니다. 

이 작업이 실패하면 다음을 조사할 수 있습니다.

#### <a name="cpu-performance-for-desktop-users"></a>데스크톱 사용자에 대한 CPU 성능

AltspaceVR을 실행하는 데 권장되는 하드웨어에 대한 [권장 시스템 사양을](../getting-started/system-requirements.md) 검토합니다. i3 이하 CPU는 비디오의 프레임 속도뿐만 아니라 드롭아웃 및 품질 저하와 같은 오디오 문제에 영향을 줄 수 있는 문제를 야기한다는 것을 발견했습니다.

#### <a name="internet-bandwidth-and-network-connection"></a>인터넷 대역폭 및 네트워크 연결

느린 인터넷 연결(5mbps 미만) 또는 WiFi의 사용자는 드롭아웃과 같은 오디오 문제가 있을 수 있습니다. 컴퓨터에 이더넷 케이블을 연결하고 연결 속도를 5mbps보다 빠르게 하는 것이 좋습니다. 백그라운드에서 인터넷 연결을 사용할 수 있는 모든 프로그램을 종료할 수 있습니다.

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>다른 사용자가 내 말을 들어도 안 되는 경우 어떻게 해야 합니까?

먼저 AltspaceVR이 마이크에서 오디오를 감지하는지 확인합니다. 대화할 때 보기 왼쪽 아래의 마이크 아이콘이 깜박인지 여부를 확인하여 이를 확인할 수 있습니다. 대화할 때 아이콘이 깜박이면 마이크가 작동합니다. 아이콘이 빨간색이면 음소거됩니다. 아이콘을 선택하여 자신을 음소거하거나 음소거 해제합니다.

음소거 후 마이크 아이콘이 깜박이지 않으면 AltspaceVR에서 마이크 설정을 조정하고 메뉴/설정/오디오/오디오 입력 선택으로 이동해야 할 수 있습니다. 그런 다음 화살표 단추를 사용하여 사용하려는 마이크를 선택합니다.
 
### <a name="oculus-questquest-2"></a>Oculus Quest/Quest 2

AltspaceVR을 설치할 때 마이크 오디오를 사용할 수 있는 권한을 부여해야 합니다. 수행할 수 있는 또 다른 확인은 메뉴/설정/오디오/오디오 입력 선택을 살펴보고, Quest/Quest2의 기본 마이크인 Android 오디오 입력으로 설정되어 있는지 확인하는 것입니다.
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality, Oculus Oculus 조정/스모크 S, HTC Vive 또는 2D 모드

AltspaceVR: 메뉴/설정/오디오/오디오 입력 선택에서 올바른 마이크 설정이 있는지 확인합니다. 그런 다음 화살표 단추를 사용하여 사용하려는 마이크를 선택합니다.

AltspaceVR을 시작하기 전에 적절한 마이크가 Windows 기본 녹음 디바이스로 설정되어 있는지 확인합니다. AltspaceVR에 다른 마이크가 연결되어 있으면 해당 디바이스를 사용하려고 할 수 있는 경우 OculusSpace/표시 S 및 HTC Vive에는 모두 기본 제공 마이크가 있습니다.
 
Windows 기본 기록 디바이스를 변경하려면 다음을 수행합니다.

* Windows 스피커 아이콘을 마우스 오른쪽 단추로 클릭하고 **소리 설정 열기를** 선택합니다.
* **입력/입력 디바이스 선택** 드롭다운으로 이동합니다.
* 드롭다운 메뉴에서 사용하려는 마이크를 선택합니다. 
    * HTC Vive 마이크에는 **마이크 - USB 오디오 디바이스** 레이블이 지정됩니다.
    * Oculus Microphone 마이크에는 **헤드셋 마이크(Oculus 가상 오디오 디바이스)** 레이블이 지정됩니다.
* AltspaceVR을 다시 시작한 후 마이크가 선택됩니다.
 
이러한 단계를 수행한 후에도 여전히 문제가 있는 경우 영향을 줄 수 있는 것은 다음과 같습니다.

* 30초 이상 Alt-Tab 경우 AltspaceVR에서 자동으로 음소거됩니다. **AltspaceVR이 유휴 상태일 때 메뉴 -> 설정 -> 오디오 -> 음소거에서** 이 옵션을 사용하지 않도록 설정할 수 있습니다.
* AltspaceVR 오디오 시스템에는 아래일 수 있는 볼륨 임계값이 있습니다. 마이크 수준을 최대로 설정하고, 마이크를 사용자의 입에 더 가깝게 설정하고, 일반 볼륨에서 말합니다.
* VR을 종료하고 헤드셋의 USB 코드를 대체 USB 3.0 포트에 연결해 보세요. 이 경험에서는 일부 USB 3.0 포트로 인해 문제가 발생합니다.

AltspaceVR은 게임 중의 소리 설정 변경 내용을 인식하지 못할 수 있으므로 위의 마이크 변경 내용을 적용하려면 AltspaceVR을 다시 시작해야 할 수 있습니다.  게임을 다시 시작하면 마이크 아이콘을 보고 대화할 때 깜박이는지 확인합니다. 아이콘이 깜박이면 마이크가 작동합니다.

## <a name="support"></a>Support(지원)

AltspaceVR 팀에 대한 질문 또는 피드백 

> [!div class="nextstepaction"]
> [지원 요청을 보내려면 여기를 클릭하세요.](https://help.altvr.com/hc/requests/new)