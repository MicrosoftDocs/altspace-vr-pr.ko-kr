---
title: 레코딩 및 라이브 스트리밍
description: 사용자와의 판촉 및 공유를 위해 PC에서 AltspaceVR 이벤트를 기록 하 고 라이브 스트리밍하는 방법에 대해 알아봅니다.
author: qianw211
ms.author: v-qianwen
ms.date: 11/1/2021
ms.topic: article
keywords: 스트리밍, 기록, 비디오, 오디오, youtube, obs, 라이브
ms.openlocfilehash: e82960097103df25c50f0b03b76d21e10b1cbbd6
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278982"
---
# <a name="recording-and-live-streaming"></a>레코딩 및 라이브 스트리밍

전 세계의 사람들을 보여 주기 위해 AltspaceVR 환경을 기록 하 고 라이브 스트리밍하는 것은 일반적으로 이벤트, AltspaceVR 및 VR의 수준을 올리는 좋은 방법입니다. 시작 하는 방법을 보려면 아래를 확인 하세요.

이 문서에서는 다음을 수행하는 방법을 알아봅니다.

* [PC에서 2D 모드로 AltspaceVR 기록](#recording-altspacevr-in-2d-mode-on-pc)
* [PC에서 2D 모드로 AltspaceVR에서 YouTube로 라이브 스트림](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>PC에서 2D 모드로 AltspaceVR 기록

### <a name="the-short-version"></a>짧은 버전

1. AltspaceVR 및 OBS (Open 브로드캐스터 소프트웨어)가 설치 되어 있어야 합니다. AltspaceVR를 2D 모드로 시작 하 고, OBS를 시작 하 고, AltspaceVR를 기록 하도록 OBS를 설정 하 고, 기록 합니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

1. [https://obsproject.com/](https://obsproject.com/)로 이동합니다.
2. **Windows** 를 선택 하 여 obs를 다운로드 합니다. 이 게시물은 **Obs v 26.1.1** 를 사용 합니다.
3. OBS 설치

### <a name="have-altspacevr-running-before-you-run-obs"></a>OBS를 실행 하기 전에 AltspaceVR를 실행 해야 합니다.

1. 웹 사이트에서 AltspaceVR 다운로드 및 설치: [altvr.com/get](https://altvr.com/getaltspacevr)
2. VR 비디오를 안정화 하 고 jerky 헤드 이동을 제거 하려면 2D 클라이언트를 사용 하거나, PC에서 헤드셋의 USB 케이블을 분리 하 여 2D 모드로 AltspaceVR를 시작 해야 합니다. Rift이 있는 경우 Ctrl + Alt + Del을 누르고, **서비스**, **OCULUS VR 런타임 서비스** 를 선택 하 고, 마우스 오른쪽 단추를 클릭 하 고, **중지** 를 선택 합니다. 이렇게 하면 AltspaceVR를 사용 하지 않도록 설정 하 고 2D 모드에서 시작 합니다. 이러한 단계를 반복 하 고 시작을 사용 하 여 VR 모드를 다시 가져옵니다.
3. OBS를 사용 하 여 게임 캡처를 사용 하 여 VR 모드로 사용자 환경을 기록할 수도 있습니다.

이제 OBS로 Alt-Tab 합니다.

1. **장면** 에서 **+** 새 장면을 선택 하 고 이름을로 선택 합니다.
2. 그런 다음 **원본** 에서: **+ > 게임 캡처 > 새로 만들기** 를 선택 합니다.
2. 텍스트를 ' AltspaceVR 캡처 '로 편집 하 고, 틱을 **표시** 하 고, **확인** 을 선택 합니다.
3. **원본** 에서 **AltspaceVR 캡처** 를 두 번 클릭 합니다.
4. **특정 창 캡처** 로 **모드** 변경
5. 창: [AltspaceVR.exe]: AltspaceVR
6. 창 일치 우선 순위: 제목 일치, 그렇지 않으면 동일한 실행 파일의 창 찾기
7. 아래로 스크롤하여 **커서 캡처**: untick
8. **확인** 을 선택합니다.
9. 이렇게 하면 AltspaceVR가 OBS에 표시 됩니다.

이제 OBS에서 다음 속성을 설정 하려면 **파일 > 설정** 로 이동 합니다.

|탭|설정|
|---|---|
| **일반** | 기본값 유지 |
| **STREAM** | 기본값 유지 |
| **출력** | 고급으로 전환 |
| **-스트리밍 탭** | 오디오 트랙 1 <br> 인코더: x264 <br> 출력 크기 조정: 읽으려고 <br> Rate 컨트롤: CBR <br> 비트 전송률: 6000 (6000의 경우, 60 fps의 경우 9000) <br> 키 프레임 간격 = 2 <br> CPU 사용량 사전 설정 = veryfast |
| **-기록 탭** | 유형: 표준 <br> 기록 경로: D:/Video (비디오 파일을 저장 하려는 위치로 이동) <br> 기록 형식: mp4 (기록 하는 동안 약간의 충돌이 발생 하면 mp4 대신 flv를 사용해 보세요. 충돌 하는 경우 비디오는 계속 flv로 사용할 수 있습니다.) <br> 오디오 트랙 1 <br> 인코더: stream encoder 사용 |
| **-오디오 탭** | 오디오 비트 전송률: 160 (모든 트랙의 경우) |
| **-재생 버퍼 탭** | 기본값 유지 |
| **오디오** | 샘플링 주기: 44.1 khz <br> 채널: 스테레오 <br> 바탕 화면 오디오: 기본값 <br> 데스크톱 오디오 2: 사용 안 함 <br> Mic/Aux Audio: 기본값 |
| **비디오** | 기본 (캔버스) 해상도: 1920 x 1080 <br> 출력 (크기 조정) 해상도: 1920 x 1080 <br> 다운 눈금 필터: 쌍입방 (Sharpened 크기 조정, 16 개 샘플) <br> 일반적인 FPS 값: 30 (또는 60) |
| **바로 가기 키** | 기본값 유지 |
| **고급** | 프로세스 우선 순위: 보통 | <br>

<br>이제 **적용** 을 선택 하 고 **확인** 을 선택 하 여 모든 obs 설정을 저장 합니다. 

1. AltspaceVR에 대 한 Alt-Tab 올바른 공간/세계/이벤트를 확인 하 고 카메라를 온라인으로 전환 합니다. 즉, 아바타는 비디오를 기록 하려고 합니다.
2. OBS로 Alt-Tab 하 고 준비가 되 면 **기록 시작** 을 클릭 합니다.

OBS가 계산을 시작 하 고 점이 빨간색 임을 나타내는 OBS의 오른쪽 아래에 표시 **됩니다. 즉** , 기록 하는 중입니다.

테스트 기록을 다음과 같이 설정 합니다. 
1. AltspaceVR의 메뉴 열기/닫기/롤오버를 사용 하 여 UI 소리를 만듭니다.
2. ' Sibilance, Sibilance ' 라고 unmuted 하거나 일반 볼륨에서 사용자에 게 연락 하기 위해 다른 사용자에 게 문의 하세요.
3. 오디오를 제대로 선택 했는지 확인 하기 위해이 작업을 수행 하는 **데스크톱 오디오** 및 **Mic/Aux** 수준을 확인 합니다.

일반적으로 녹음할 때 Mic/Aux를 음소거 합니다. 계속 해 서 Mic/Aux의 스피커 아이콘을 선택 하면 X로 빨간색으로 바뀝니다.

* 마이크 오디오 수준을 다른 사용자의 오디오와 일치 시키는 것이 매우 어렵기 때문에 이벤트를 기록 하는 동안 Mic는 음소거를 사용 하는 것이 좋습니다.
* 오디오의 또 다른 문제는 OBS를 설정 하는 방법입니다. 컴퓨터에서 모든 오디오를 캡처하여 YouTube를 시청 하거나 PC에서 알림 소리를 가져오는 경우 해당 오디오를 기록 합니다.
* AltspaceVR에서 오디오만 기록 하려면 **열린 볼륨 믹서** 로 이동 하 고 (Windows 오른쪽 아래에 있는 스피커 아이콘을 마우스 오른쪽 단추로 클릭) 시스템 소리, 브라우저 등을 음소거 하지만 obs 또는 AltspaceVR는 음소거 하지 않습니다.

> 중요 한 녹음 후 이러한 볼륨 믹서 설정의 음소거를 잊지 마세요.

이제 OBS로 다시 이동 하 여 **기록 중지** 를 선택 합니다. 방금 기록한 비디오를 찾으려면 파일로 이동 하 고 기록 **>표시** 합니다. 그러면 OBS 비디오 파일이 포함 된 폴더가 열리고 테스트 비디오를 두 번 클릭 합니다.

기록이 상당히 큰 경우에는 OBS에서 바탕 화면 오디오의 슬라이더를 낮추고 테스트에 다른 기록을 만듭니다.

Pro: Ctrl + Alt + P를 사용 하 여 사진 모드를 전환 하 고, 보기에서 UI를 제거 하 여 좋은 정리를 얻을 수 있습니다.

축 하 합니다 AltspaceVR 비디오 레코더입니다.

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>PC에서 AltspaceVR 2D 모드의 YouTube 라이브 스트리밍

### <a name="the-short-version"></a>짧은 버전

AltspaceVR 및 OBS를 설치합니다. AltspaceVR 및 OBS를 시작합니다. 라이브 스트림 'Right Now' 또는 '이후 날짜'를 사용할 수 있습니다. YouTube에서 YouTube Stream Key를 통해 OBS를 설정합니다. OBS 및 YouTube에서 스트리밍을 시작하면 경합이 시작됩니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

라이브 스트림 대신 로컬 녹음을 사용하여 녹음을 테스트하는 방법 및 카메라샷을 설정하는 방법에 대한 지침은 이 페이지 맨 위에 있는 [PC의 2D 모드에서 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc) 기록 섹션을 참조하세요.

## <a name="setting-up-live-streaming-on-youtube"></a>YouTube에서 라이브 스트리밍 설정

'지금 바로' 라이브 스트림을 얻거나 '이후 날짜'를 통해 향후 라이브 스트림을 설정할 수 있습니다.

1. 브라우저를 열고 [https://www.youtube.com/](https://www.youtube.com/) 로그인한 다음, 로 이동합니다. [https://studio.youtube.com/](https://studio.youtube.com/)
2. 오른쪽 위에서 **만들기를** 선택한 **다음, 라이브로 이동을** 선택합니다.

**'Right now'** 메서드:

1. **지금 바로/시작을 선택합니다.**
1. **스트리밍 소프트웨어/GO** 선택
1. **편집을** 선택하고 오른쪽 위에서 비디오 세부 정보 및 사용자 지정을 편집합니다.
1. **Stream 설정** 에서 기본값을 유지합니다.
1. **Stream 키(인코더에 붙여넣기)** 옆에 키를 **복사하여** OBS에 붙여넣을 수 있습니다.
1. OBS/설정   /  **스트림 열기**
1. **서비스** 드롭다운 메뉴에서 **YouTube - RTMPS를** 선택합니다.
1. YouTube의 Stream 키를 OBS의 **스트림 키** 필드에 붙여넣습니다.
1. **적용,** 확인을 차례로 **클릭합니다.**
1. OBS에서 **스트리밍 시작을** 선택합니다.
1. YouTube로 전환하면 이제 YouTube에서 라이브로 표시됩니다.
1. 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택해야 합니다.
1. '비디오 링크'를 클릭하면 YouTube 라이브 스트림이 표시되고 들 수 있습니다. 
1. 이 URL은 라이브 스트림 링크이며 :) 모든 소셜 채널에 공유할 수 있습니다.
1. 라이브 스트림을 중지하려면 YouTube에서 스트림 종료를 선택한 다음, OBS에서 스트리밍 중지를 선택합니다.

'**Later date**' method:
1. 왼쪽 위에서 **관리** 아이콘을 선택합니다.
1. 오른쪽 위에 있는 **스트림 예약을** 선택합니다.
1. 제목, 설명, 범주, 썸네일(1280x720), **NEXT** 추가
1. 라이브 채팅 옵션, **다음**
1. 프라이빗, 비공개 또는 퍼블릭(퍼블릭 선택)
1. 라이브로 이동하려는 날짜 및 시간, **완료를** 예약합니다.

 **나중에 라이브 스트림을 시작할 준비가 되면 다음을 수행합니다.**
1. Stream 설정 기본값을 유지합니다.
1. **Stream 키(인코더에 붙여넣기)** 옆에 키를 **복사하여** OBS에 붙여넣을 수 있습니다.
1. OBS/설정   /  **스트림 열기**
* **서비스** 드롭다운 메뉴에서 **YouTube - RTMPS를** 선택합니다.
1. YouTube의 Stream 키를 OBS의 **스트림 키** 필드에 붙여넣습니다.
1. **적용,** 확인을 차례로 **클릭합니다.**
1. OBS에서 **스트리밍 시작을** 선택합니다.
1. YouTube로 전환하면 이제 YouTube에서 라이브로 표시됩니다.
1. 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택해야 합니다.
1. '비디오 링크'를 클릭하면 YouTube 라이브 스트림이 표시되고 들 수 있습니다. 
1. 이 URL은 라이브 스트림 링크이며 :) 모든 소셜 채널에 공유할 수 있습니다.
1. 라이브 스트림을 중지하려면 YouTube에서 **스트림 종료를** 선택한 다음, OBS에서 **스트리밍 중지를** 선택합니다.

보너스 포인트의 경우 소셜 비디오를 공유하고 @AltspaceVR 태그를 :)