---
title: 녹화 및 라이브 스트리밍
description: PC에서 AltspaceVR 이벤트를 기록하고 라이브 스트리밍하여 승격하고 사용자와 공유하는 방법을 알아봅니다.
ms.date: 04/26/2021
ms.topic: article
keywords: 스트리밍, 녹화, 비디오, 오디오, youtube, obs
ms.openlocfilehash: 0bf32d8ac7e2d409eb5e2c31a9da8a878e0e5eef
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923020"
---
# <a name="recording-and-live-streaming"></a>녹화 및 라이브 스트리밍

AltspaceVR 환경을 녹화하고 라이브 스트리밍하여 전 세계의 다른 사람을 표시하는 것은 일반적으로 이벤트, AltspaceVR 및 VR을 홍보할 수 있는 좋은 방법입니다. 시작하는 방법을 보려면 아래를 살펴보세요.

이 문서에서는 다음을 수행하는 방법을 알아봅니다.

* [PC의 2D 모드에서 AltspaceVR 기록](#recording-altspacevr-in-2d-mode-on-pc)
* [PC의 2D 모드에서 AltspaceVR의 YouTube로 라이브 스트림](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>PC의 2D 모드에서 AltspaceVR 기록

### <a name="the-short-version"></a>짧은 버전

1. AltspaceVR 및 OBS를 설치합니다. 2D 모드에서 AltspaceVR을 시작하고, OBS를 시작하고, AltspaceVR을 기록하고 기록하도록 OBS를 설정합니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

1. [https://obsproject.com/](https://obsproject.com/)로 이동합니다.
2. **Windows를** 선택하여 OBS를 다운로드합니다. 이 게시물은 **OBS v22.0.2를** 사용하고 있습니다.
3. OBS 설치

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>OBS를 실행하기 전에 AltspaceVR을 2D 모드로 실행합니다.

1. 웹 사이트에서 AltspaceVR 다운로드 및 설치: [altvr.com/get](https://altvr.com/getaltspacevr)
2. PC에서 HMD의 USB 케이블을 분리하여 2D 모드에서 AltspaceVR을 시작하거나, Ctrl+Alt+Del, 서비스, Oculus VR 런타임 서비스, 마우스 오른쪽 단추 클릭, 중지가 있는 경우 AltspaceVR을 시작합니다. 
    * 이렇게 하면 Oculus를 사용하지 않도록 설정하고 2D 모드에서 AltspaceVR을 시작하고, 이러한 단계를 반복하고, 시작을 사용하여 VR 모드를 다시 가져옵니다.

이제 OBS로 Alt-Tab.

1. 원본에서 **+ > Game Capture > 새로 만들기를** 선택합니다.
2. 텍스트를 'AltspaceVR 캡처'로 **편집하고, 소스 표시를 선택하고,** 확인을 선택합니다.
3. 원본에서 **AltspaceVR 캡처를** 두 번 클릭합니다.
4. **특정 창을 캡처하도록** **모드** 변경
5. 창: [AltspaceVR.exe]: AltspaceVR
6. 창 일치 우선 순위: 제목과 일치합니다. 그렇지 않으면 동일한 실행 파일의 창을 찾습니다.
7. 커서를 캡처하는 Scroll down: 선택 취소
8. 확인을 선택합니다.

이렇게 하면 AltspaceVR이 OBS에 표시됩니다. 이제 OBS에서 다음 속성을 설정하려면 **파일 > 설정으로** 이동합니다.

|탭|설정|
|---|---|
| **일반** | 기본값 유지 |
| **STREAM** | 기본값 유지 |
| 출력 모드 | 고급으로 전환 |
| 스트리밍 탭 | 오디오 트랙 1 <br> 인코더: x264 <br> 출력 크기 다시 조정: 선택 취소 <br> Rate 컨트롤: CBR <br> 비트 전송률: 6000(30fps의 경우 6000, 60fps의 경우 9000) <br> 키 프레임 간격 = 2 <br> CPU 사용량 사전 설정 = veryfast |
| 기록 탭 | 유형: 표준 <br> 기록 경로: D:/Video(비디오 파일을 저장할 위치로 이동) <br> 녹화 형식: mp4(녹화하는 동안 충돌이 발생하면 mp4 대신 여기서 flv를 사용해 보세요. 충돌하는 경우 비디오는 flv에서 계속 사용할 수 있습니다.) <br> 오디오 트랙 1 <br> 인코더: 스트림 인코더 사용 |
| 오디오 탭 | 오디오 비트 전송률: 160(모든 트랙의 경우) |
| 재생 버퍼 탭 | 기본값 유지 |
| **오디오** | 샘플 속도: 48khz <br> 채널: 스테레오 <br> 데스크톱 오디오 디바이스: 기본값 <br> 데스크톱 오디오 디바이스 2: 사용 안 함 <br> 마이크/보조 오디오 디바이스: 기본값 |
| **비디오** | 기본(캔버스) 해상도: 1920x1080 <br> 출력(크기 조정) 해상도: 1920x1080 <br> 다운스케일 필터: Bicubic(선명하게 확장된 크기 조정, 16개 샘플) <br> 일반적인 FPS 값: 30 |
| **단축키** | 기본값 유지 |
| **고급** | 프로세스 우선 순위: 보통 | <br>

<br>이제 **적용을** 선택한 **다음, 확인을** 선택하여 모든 OBS 설정을 저장합니다. 

1. AltspaceVR로 Alt-Tab 올바른 공간/세계/이벤트로 들어가서 비디오를 녹화하려는 카메라(즉, 아바타)를 정렬합니다.
2. OBS로 Alt-Tab 준비가 되면 **기록 시작을** 클릭합니다.

OBS의 오른쪽 아래에 REC: 가 계산을 시작하고 점이 빨간색으로 표시되어 기록 중임을 의미합니다.

다음을 통해 테스트 기록을 만듭니다. 
1. AltspaceVR에서 메뉴를 열기/닫기/롤오버하여 UI 소리 만들기
2. 'Sibilance, Sibilance'라고 말하거나 다른 사용자가 일반 볼륨에서 서로 대화하도록 해야 합니다.
3. 이 작업을 수행하는 데스크톱 오디오 및 마이크/보조 수준을 확인하여 작동하는지 확인합니다.

기록할 때 일반적으로 Mic/Aux를 음소거합니다. 계속 진행하여 Mic/Aux에 대한 화자 아이콘을 선택하면 X가 빨간색으로 바뀝니다.

* 이벤트를 기록할 때 마이크가 가장 잘 음소거되도록 오디오 및 다른 사용자의 오디오를 일치시키기가 매우 어렵습니다.
* 오디오의 또 다른 문제는 OBS가 설정되는 방식입니다. 컴퓨터에서 모든 오디오를 캡처하므로 PC에서 YouTube를 시청하는 경우 해당 오디오 또는 디스패코드 알림을 기록합니다.
* AltspaceVR의 오디오만 기록하려면 볼륨 혼합기로 이동하고(Windows 오른쪽 아래에 있는 스피커 아이콘을 마우스 오른쪽 단추로 클릭) 시스템 소리, 브라우저 등을 음소거하지만 OBS 또는 AltspaceVR을 음소거하지는 않습니다.

> [!IMPORTANT]
> 기록 후 이러한 볼륨 혼합기 설정을 다시 켜야 합니다.

이제 OBS로 돌아가서 파일에서 **기록 중지**>**기록 표시를** 선택합니다. 그러면 OBS 비디오 파일이 있는 폴더가 열리고 테스트 비디오를 두 번 클릭합니다.

경우에 따라 녹음이 매우 시끄러워서 데스크톱 오디오에 대한 슬라이더를 낮추고 테스트할 다른 녹음을 만듭니다.


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>PC의 AltspaceVR 2D 모드에서 YouTube로 라이브 스트리밍

### <a name="the-short-version"></a>짧은 버전

AltspaceVR 및 OBS를 설치합니다. 2D 모드에서 AltspaceVR을 시작하고, 라이브 스트림을 시작하거나, YouTube에서 '새 라이브 이벤트'를 만들고, YouTube Stream Key로 OBS를 설정하고, OBS에서 스트리밍을 시작하고, YouTube에서 스트리밍을 시작하고, 경합을 시작합니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

1. [https://obsproject.com/](https://obsproject.com/)로 이동합니다.
2. OBS를 다운로드하려면 **Windows를** 선택합니다(이 게시물은 OBS v22.0.2 사용).
3. OBS 설치

OBS를 실행하기 전에 AltspaceVR을 2D 모드로 실행합니다.
1. 웹 사이트에서 AltspaceVR을 다운로드합니다. [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. 2D 모드에서 AltspaceVR을 시작하려면 PC에서 HMD의 USB 케이블을 분리하거나, Ctrl+Alt+Del, 서비스, Oculus VR 런타임 서비스, 마우스 오른쪽 단추로 클릭, 중지가 있는 경우. 이렇게 하면 Oculus Home을 사용하지 않도록 설정하고 2D 모드에서 AltspaceVR을 시작하고, 이러한 단계를 반복하고, VR 모드를 다시 시작합니다.

3. OBS로 Alt-Tab

4. 원본에서 , **+** 게임 캡처 선택, 새로 만들기, 텍스트를 'AltspaceVR 캡처'로 편집, 원본 표시 확인, 확인을 선택합니다.
5. AltspaceVR 캡처를 두 번 클릭합니다.
6. 모드: 특정 창 캡처
7. 창: [AltspaceVR.exe]: AltspaceVR
8. 창 일치 우선 순위: 제목과 일치합니다. 그렇지 않으면 동일한 실행 파일의 창을 찾습니다.
9. 커서 캡처를 Scroll down: 확인 선택 취소

이렇게 하면 AltspaceVR이 OBS에 표시됩니다. 잘하셨습니다!

이제 OBS에서 파일>설정으로 이동합니다.

| 탭 | 설정 |
|---|---|
| 일반 | 스트리밍 시 자동으로 기록 틱(라이브 스트리밍 외에도 비디오 파일을 컴퓨터에 기록함) |
| STREAM | 스트림 유형: Streaming Services <br> 서비스: YouTube/YouTube 게임(Twitch, Mixer, Facebook Live 등으로 스트리밍할 수도 있습니다.)<br>서버: 기본 YouTube ingest server <br>스트림 키: YouTube에서 스트림 키 붙여넣기(아래 'YouTube에서 라이브 스트리밍 설정' 참조) |
| 출력 | 출력 모드: 고급으로 전환 |
| 스트리밍 | 오디오 트랙 1 <br>인코더: x264 <br>스트리밍 서비스 인코더 설정 적용: 틱 <br>출력 크기 다시 조정: 선택 취소 <br>Rate 컨트롤: CBR <br>비트 전송률: 6000(30fps의 경우 6000, 60fps의 경우 9000) <br>키 프레임 간격 = 2 <br>CPU 사용량 사전 설정 = veryfast |
| 기록 중 | 유형: 표준 <br>기록 경로: D:/Video(이전에 '스트리밍 시 자동으로 기록'을 선택한 경우 비디오 파일을 저장할 위치로 이동) <br>녹화 형식: mp4(녹화하는 동안 충돌이 발생하면 mp4 대신 여기서 flv를 사용해 보세요. 충돌하는 경우 비디오는 flv에서 계속 사용할 수 있습니다.) <br>오디오 트랙 1 <br>인코더: 스트림 인코더 사용 |
| 오디오 | 오디오 비트 전송률: 160(모든 트랙) 샘플 속도: 48khz <br>채널: 스테레오 <br>데스크톱 오디오 디바이스: 기본값 <br>데스크톱 오디오 디바이스 2: 사용 안 함 <br>마이크/보조 오디오 디바이스: 기본값 |
| 재생 버퍼 | 기본값 유지 |
| 동영상 | 기본(캔버스) 해상도: 1920x1080 <br>출력(크기 조정) 해상도: 1920x1080 <br>다운스케일 필터: Bicubic(선명하게 확장된 크기 조정, 16개 샘플) <br>일반적인 FPS 값: 30 |
| 단축키 | 기본값 유지 |
| 고급 | 프로세스 우선 순위: 보통 |
|||

<br>이제 적용, 확인을 차례로 클릭한 다음 OBS를 닫았다가 다시 엽니다. 이 경우 모든 OBS 설정이 저장됩니다. 보기 좋은 :)

라이브 스트림 대신 로컬 녹음을 사용하여 녹화를 테스트하는 방법 및 녹화하기 전에 카메라 샷 설정을 먼저 얻는 방법에 대한 지침은 위의 'PC에서 2D 모드로 AltspaceVR을 기록하는 방법' 섹션을 참조하세요.

오디오의 또 다른 문제는 OBS가 설정되는 방식입니다. 컴퓨터에서 모든 오디오를 캡처하므로 YouTube를 시청하는 경우 해당 오디오 또는 Teams 메시지 또는 알림 소리를 기록합니다.

AltspaceVR의 오디오만 기록하려면 볼륨 혼합기(Windows 오른쪽 아래에 있는 스피커 아이콘을 마우스 오른쪽 단추로 클릭)로 이동하고 시스템 소리, 브라우저 등을 음소거하지만 OBS 또는 AltspaceVR을 음소거하지 않습니다.

녹음한 후 오디오를 다시 켜는 것을 잊지 마세요;)

AltspaceVR 비디오 레코더입니다.

## <a name="setting-up-live-streaming-on-youtube"></a>YouTube에서 라이브 스트리밍 설정

라이브 스트림을 빠르게 **얻거나(스트림)** 향후 라이브 스트림 **이벤트(관리)를** 설정할 수 있습니다. '관리' 방식으로 설정하는 것이 좋습니다.

1. 브라우저를 열고 [https://www.youtube.com/](https://www.youtube.com/) 로그인한 다음, 로 이동합니다. [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. 계정 아이콘을 선택하고 오른쪽 위에 있는 드롭다운에서 Creator Studio를 선택합니다.
3. 페이지의 왼쪽에 있는 라이브 스트리밍입니다.

'**Stream now**' 메서드:

* 편집을 선택하여 라이브 스트림 정보를 입력합니다.<br>
* 스트림 설정에서 기본값을 유지합니다.<br>
* 스트림 키(인코더에 붙여넣기)에서 '표시'를 선택하고 이 키를 복사하여 OBS에 붙여넣을 수 있습니다.<br>
* OBS/설정/스트림 열기<br>
* YouTube의 스트림 키를 OBS의 스트림 키 필드에 붙여넣습니다.<br>
* 적용한 다음, 확인<br>
* OBS에서 스트리밍 시작을 선택합니다.<br>
* YouTube로 전환하면 이제 YouTube에서 라이브로 표시됩니다.<br>
* 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택해야 합니다.<br>
* '비디오 링크'를 복사하여 새 브라우저 탭에 붙여넣으면 YouTube 라이브 스트림 페이지가 표시됩니다.<br>
* 이 URL은 라이브 스트림 링크이며 :) 모든 소셜 채널에 공유할 수 있습니다.<br>
* 라이브 스트림을 중지하려면 OBS에서 스트리밍 중지를 선택합니다. 그러면 YouTube의 라이브 스트림이 종료됩니다.<br>
* 그런 다음 YouTube에서 스트림을 중지합니다.<br>

'**Manage**' 메서드:
* '스트림 예약'을 선택합니다.
* 이전 관리형 라이브 스트림을 이미 설정한 경우 새로 만들기 또는 설정 다시 사용
* 제목, 날짜, 시작 시간, 설명, 썸네일 업로드 및 태그 추가 – AltspaceVR에 태그를 :)
* 드롭다운 메뉴에서 공용을 선택합니다(기본값은 'Unlisted').
* 기본값 사용
* 스트림 키 복사(인코더에 붙여넣기)
* 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택해야 합니다. YouTube 라이브 스트림 이벤트 링크입니다. 실제 이벤트보다 소셜 방식으로 공유할 수 있습니다.
* 이제 OBS 열기
* 파일/설정
* STREAM
* 복사한 스트림 키를 스트림 키 필드에 붙여넣습니다.
* 적용한 다음, 확인
* '스트리밍 시작'을 선택합니다.
* YouTube로 돌아가면 '미리 보기' 창에 스트림이 표시되고 GO LIVE가 오른쪽 위에 켜집니다.
* 라이브로 이동을 선택합니다.
* 이제 라이브가 되었습니다!
* '보기 페이지의 보기' 링크가 열려 있는 브라우저 탭으로 이동하여 비디오가 제대로 보이는지 확인합니다. Windows Volume Mixer에서 오디오를 음소거할 때 브라우저에서 오디오를 해제했기 때문에 오디오를 들어보지 않습니다. 휴대폰에서 오디오를 확인하거나 친구에게 오디오를 확인해 달라고 요청합니다.
* 보기 좋네요!
* AltspaceVR로 다시 Alt-Tab 이벤트에서 카메라(즉, 아바타)를 이동합니다.
* 라이브 스트림을 마쳤으면 YouTube 'Live Control Room' 페이지로 돌아갑니다.
* '스트리밍 중지'를 선택합니다.
* 라이브 이벤트 스트리밍을 중지할 것인지 묻는 대화 상자가 열립니다. 확인
* OBS로 이동하여 스트리밍 중지도 선택합니다.
* 축하합니다. 이제 AltspaceVR 슬라이더가 되었습니다.

보너스 포인트의 경우 소셜 미디어에서 전 세계와 비디오를 공유하고 :) 태그를 추가해야 합니다. @AltspaceVR