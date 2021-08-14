---
title: 레코딩 및 라이브 스트리밍
description: 사용자와의 판촉 및 공유를 위해 PC에서 AltspaceVR 이벤트를 기록 하 고 라이브 스트리밍하는 방법에 대해 알아봅니다.
ms.date: 04/26/2021
ms.topic: article
keywords: 스트리밍, 기록, 비디오, 오디오, youtube, obs
ms.openlocfilehash: 95a742cb2bfe5c277e698175bd9f657fcac5923d181c3eeb6905004d25f81aa6
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126110"
---
# <a name="recording-and-live-streaming"></a>레코딩 및 라이브 스트리밍

전 세계의 사람들을 보여 주기 위해 AltspaceVR 환경을 기록 하 고 라이브 스트리밍하는 것은 일반적으로 이벤트, AltspaceVR 및 VR의 수준을 올리는 좋은 방법입니다. 시작 하는 방법을 보려면 아래를 확인 하세요.

이 문서에서는 다음을 수행하는 방법을 알아봅니다.

* [PC에서 2D 모드로 AltspaceVR 기록](#recording-altspacevr-in-2d-mode-on-pc)
* [PC에서 2D 모드로 AltspaceVR에서 YouTube로 라이브 스트림](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>PC에서 2D 모드로 AltspaceVR 기록

### <a name="the-short-version"></a>짧은 버전

1. AltspaceVR 및 OBS가 설치 되어 있어야 합니다. AltspaceVR를 2D 모드로 시작 하 고, OBS를 시작 하 고, AltspaceVR를 기록 하도록 OBS를 설정 하 고, 기록 합니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

1. [https://obsproject.com/](https://obsproject.com/)로 이동합니다.
2. **Windows** 를 선택 하 여 obs를 다운로드 합니다. 이 게시물은 **Obs v 22.0.2** 를 사용 합니다.
3. OBS 설치

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>OBS를 실행 하기 전에 AltspaceVR이 2D 모드로 실행 되 고 있어야 합니다.

1. 웹 사이트에서 AltspaceVR 다운로드 및 설치: [altvr.com/get](https://altvr.com/getaltspacevr)
2. HMD의 USB 케이블을 PC에서 분리 하거나 Rift: Ctrl + Alt + Del, Services, Oculus VR Runtime Service, 마우스 오른쪽 단추 클릭, 중지를 사용 하 여 AltspaceVR를 2D 모드로 시작 해야 합니다. 
    * 그러면 Oculus를 사용 하지 않도록 설정 하 고 2D 모드에서 AltspaceVR를 시작 합니다. 이러한 단계를 반복 하 고 시작을 사용 하 여 VR 모드를 다시 가져옵니다.

이제 OBS로 Alt-Tab 합니다.

1. 원본에서: **+ > 게임 캡처 > 새로 만들기** 를 선택 합니다.
2. 텍스트를 ' AltspaceVR 캡처 '로 편집 하 고, 틱을 **표시** 하 고, 확인을 선택 합니다.
3. 원본에서 **AltspaceVR 캡처** 를 두 번 클릭 합니다.
4. **특정 창 캡처** 로 **모드** 변경
5. 창: [AltspaceVR.exe]: AltspaceVR
6. 창 일치 우선 순위: 제목 일치, 그렇지 않으면 동일한 실행 파일의 창 찾기
7. 아래로 스크롤하여 커서 캡처: untick
8. 확인을 선택합니다.

이렇게 하면 AltspaceVR가 OBS에 표시 됩니다. 이제 OBS에서 다음 속성을 설정 하려면 **파일 > 설정** 로 이동 합니다.

|탭|설정|
|---|---|
| **일반** | 기본값 유지 |
| **스트림** | 기본값 유지 |
| 출력 모드 | 고급으로 전환 |
| 스트리밍 탭 | 오디오 트랙 1 <br> 인코더: x264 <br> 출력 크기 조정: 읽으려고 <br> Rate 컨트롤: CBR <br> 비트 전송률: 6000 (6000의 경우, 60 fps의 경우 9000) <br> 키 프레임 간격 = 2 <br> CPU 사용량 사전 설정 = veryfast |
| 기록 탭 | 유형: 표준 <br> 기록 경로: D:/Video (비디오 파일을 저장 하려는 위치로 이동) <br> 기록 형식: mp4 (기록 하는 동안 약간의 충돌이 발생 하면 mp4 대신 flv 사용해 보세요. 충돌 하는 경우에도 flv에서 비디오를 사용할 수 있습니다.) <br> 오디오 트랙 1 <br> 인코더: stream encoder 사용 |
| 오디오 탭 | 오디오 비트 전송률: 160 (모든 트랙의 경우) |
| 재생 버퍼 탭 | 기본값 유지 |
| **오디오** | 샘플링 주기: 48khz <br> 채널: 스테레오 <br> 데스크톱 오디오 장치: 기본값 <br> 데스크톱 오디오 장치 2: 사용 안 함 <br> Mic/Aux 오디오 장치: 기본값 |
| **비디오** | 기본 (캔버스) 해상도: 1920 x 1080 <br> 출력 (크기 조정) 해상도: 1920 x 1080 <br> 다운 눈금 필터: 쌍입방 (Sharpened 크기 조정, 16 개 샘플) <br> 일반적인 FPS 값: 30 |
| **바로 가기 키** | 기본값 유지 |
| **고급** | 프로세스 우선 순위: 보통 | <br>

<br>이제 **적용** 을 선택 하 고 **확인** 을 선택 하 여 모든 obs 설정을 저장 합니다. 

1. AltspaceVR에 대 한 Alt-Tab 올바른 공간/세계/이벤트를 확인 하 고 카메라를 온라인으로 전환 합니다. 즉, 아바타 라면 비디오를 기록 하려고 합니다.
2. OBS로 Alt-Tab 하 고 준비가 되 면 **기록 시작** 을 클릭 합니다.

OBS가 계산을 시작 하 고 점이 빨간색 임을 나타내는 OBS의 오른쪽 아래에 표시 됩니다. 즉, 기록 하는 중입니다.

테스트 기록을 다음과 같이 설정 합니다. 
1. AltspaceVR의 메뉴 열기/닫기/롤오버를 사용 하 여 UI 소리를 만듭니다.
2. ' Sibilance, Sibilance ' 라고 unmuted 하거나 일반 볼륨에서 사용자에 게 연락 하기 위해 다른 사용자에 게 문의 하세요.
3. 이 작업을 수행 하는 것 처럼 데스크톱 오디오 및 Mic/Aux 수준을 확인 합니다.

일반적으로 녹음할 때 Mic/Aux를 음소거 합니다. 계속 해 서 Mic/Aux의 스피커 아이콘을 선택 하면 X로 빨간색으로 바뀝니다.

* 오디오와 다른 사용자의 오디오를 일치 시키는 것이 매우 어렵기 때문에 이벤트를 기록할 때 마이크가 최적으로 음소거 됩니다.
* 오디오의 또 다른 문제는 OBS를 설정 하는 방법입니다. 컴퓨터의 모든 오디오를 캡처하여 PC에서 YouTube를 시청 하는 경우 해당 오디오 또는 Discord 알림을 기록 합니다.
* AltspaceVR에서 오디오만 기록 하려면 볼륨 Mixer (Windows 오른쪽 아래에 있는 스피커 아이콘을 마우스 오른쪽 단추로 클릭)로 이동 하 고 시스템 소리, 브라우저 등을 음소거 하지만 obs 또는 AltspaceVR는 음소거 하지 않습니다.

> [!IMPORTANT]
> 기록 후 이러한 볼륨 Mixer 설정을 다시 설정 해야 합니다.

이제 OBS로 다시 이동 하 고 파일에서 **기록 중지** **>기록 표시** 를 선택 합니다. 그러면 OBS 비디오 파일이 포함 된 폴더가 열리고 테스트 비디오를 두 번 클릭 합니다.

기록이 상당히 큰 경우에는 데스크톱 오디오의 슬라이더를 낮추고 테스트 하기 위해 다른 기록을 만듭니다.


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>PC에서 AltspaceVR 2D 모드의 YouTube 라이브 스트리밍

### <a name="the-short-version"></a>짧은 버전

AltspaceVR 및 OBS가 설치 되어 있어야 합니다. 2D 모드에서 AltspaceVR를 시작 하 고, 라이브 스트림을 시작 하거나, YouTube에서 ' 새 라이브 이벤트 '를 생성 하 고, youtube 스트림 키로 OBS를 설정 하 고, OBS에서 스트리밍을 시작 하 고, YouTube에서 스트리밍을 시작 하 고, 레이스를 진행 합니다.

### <a name="the-slightly-longer-version"></a>약간 더 긴 버전

1. [https://obsproject.com/](https://obsproject.com/)로 이동합니다.
2. obs를 다운로드 하려면 **Windows** 을 선택 합니다 (이 게시물은 obs v 22.0.2를 사용).
3. OBS 설치

OBS를 실행 하기 전에 AltspaceVR이 2D 모드로 실행 되 고 있어야 합니다.
1. 웹 사이트에서 AltspaceVR를 다운로드 합니다. [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. AltspaceVR를 2D 모드로 시작 하려면 PC에서 HMD의 USB 케이블을 분리 하거나 Rift: Ctrl + Alt + Del, Services, Oculus VR Runtime Service, 마우스 오른쪽 단추 클릭, 중지를 클릭 합니다. 이렇게 하면 Oculus Home을 사용 하지 않도록 설정 하 고 AltspaceVR를 2D 모드로 시작 하 고, 이러한 단계를 반복 하 여 VR 모드를 다시 시작 합니다.

3. OBS로 Alt-Tab

4. 원본에서을 선택 **+** 하 고, 게임 캡처를 선택 하 고, 새로 만들기를 선택 하 고, ' AltspaceVR 캡처 '로 텍스트를 편집 하 고, 틱 소스 표시, 확인
5. AltspaceVR Capture를 두 번 클릭 합니다.
6. 모드: 특정 창 캡처
7. 창: [AltspaceVR.exe]: AltspaceVR
8. 창 일치 우선 순위: 제목 일치, 그렇지 않으면 동일한 실행 파일의 창 찾기
9. 아래로 스크롤하여 커서 캡처: untick OK

이렇게 하면 AltspaceVR가 OBS에 표시 됩니다. 잘하셨습니다!

이제 OBS에서 File>설정로 이동 합니다.

| 탭 | 설정 |
|---|---|
| 일반 | 스트리밍이 자동으로 기록 됩니다 (라이브 스트리밍 외에도 컴퓨터에 비디오 파일 기록). |
| 스트림 | 스트림 형식: 스트리밍 서비스 <br> Service: youtube/youtube 게임 (Twitch, Mixer, Facebook Live 등으로 스트리밍할 수도 있음)<br>서버: 기본 YouTube 수집 서버 <br>스트림 키: YouTube에서 스트림 키 붙여넣기 * * * (' YouTube에서 라이브 스트리밍 설정 ' 참조) |
| 출력 | 출력 모드: 고급으로 전환 |
| 스트리밍 | 오디오 트랙 1 <br>인코더: x264 <br>스트리밍 서비스 인코더 설정 적용: 틱 <br>출력 크기 조정: 읽으려고 <br>Rate 컨트롤: CBR <br>비트 전송률: 6000 (6000의 경우, 60 fps의 경우 9000) <br>키 프레임 간격 = 2 <br>CPU 사용량 사전 설정 = veryfast |
| 기록 중 | 유형: 표준 <br>기록 경로: D:/Video (' 스트리밍 시 자동으로 기록 '을 선택한 경우 비디오 파일을 저장 하려는 위치로 이동) <br>기록 형식: mp4 (기록 하는 동안 약간의 충돌이 발생 하면 mp4 대신 flv 사용해 보세요. 충돌 하는 경우에도 flv에서 비디오를 사용할 수 있습니다.) <br>오디오 트랙 1 <br>인코더: stream encoder 사용 |
| 오디오 | 오디오 비트 전송률: 160 (모든 트랙의 경우) 샘플 속도: 48khz <br>채널: 스테레오 <br>데스크톱 오디오 장치: 기본값 <br>데스크톱 오디오 장치 2: 사용 안 함 <br>Mic/Aux 오디오 장치: 기본값 |
| 재생 버퍼 | 기본값 유지 |
| 동영상 | 기본 (캔버스) 해상도: 1920 x 1080 <br>출력 (크기 조정) 해상도: 1920 x 1080 <br>다운 눈금 필터: 쌍입방 (Sharpened 크기 조정, 16 개 샘플) <br>일반적인 FPS 값: 30 |
| 바로 가기 키 | 기본값 유지 |
| 고급 | 프로세스 우선 순위: 보통 |
|||

<br>이제 적용, 확인을 차례로 클릭 한 다음 OBS를 닫았다가 다시 열어야 합니다. 그러면 모든 OBS 설정이 저장 됩니다. 좋은:) 찾기

라이브 스트림 대신 로컬 기록을 사용 하 여 기록을 테스트 하는 방법에 대 한 지침과 기록 하기 전에 카메라 샷을 먼저 설정 하는 방법에 대 한 지침은 위의 ' PC에서 2D 모드에서 AltspaceVR를 기록 하는 방법 ' 섹션을 참조 하세요.

오디오의 또 다른 문제는 OBS를 설정 하는 방법입니다. 컴퓨터에서 모든 오디오를 캡처 하므로 YouTube를 시청 하는 경우 해당 오디오 또는 Teams 메시지 또는 알림 소리가 기록 됩니다.

AltspaceVR에서 오디오만 기록 하려면 볼륨 Mixer (Windows 오른쪽 아래에 있는 스피커 아이콘을 마우스 오른쪽 단추로 클릭)로 이동 하 고 시스템 소리, 브라우저 등을 음소거 하지만 obs 또는 AltspaceVR는 음소거 하지 않습니다.

녹음;) 후에 오디오를 다시 켜는 것을 잊지 마세요.

축 하 합니다 AltspaceVR 비디오 레코더입니다.

## <a name="setting-up-live-streaming-on-youtube"></a>YouTube에서 라이브 스트리밍 설정

라이브 스트림을 신속 하 게 가져오거나 (**스트림**), 이후 라이브 스트림 이벤트 (**관리**)를 설정할 수 있습니다. ' 관리 ' 방식으로 설정 하는 것이 좋습니다.

1. 브라우저를 열고에 로그인 한 [https://www.youtube.com/](https://www.youtube.com/) 후로 이동 합니다. [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. 계정 아이콘을 선택 하 고 오른쪽 위에 있는 드롭다운에서 Creator Studio를 선택 합니다.
3. 페이지 왼쪽의 라이브 스트리밍입니다.

'**Stream now**' 메서드:

* 라이브 스트림 정보를 입력 하려면 편집을 선택 합니다.<br>
* 스트림 설정에서 기본값을 유지 합니다.<br>
* 스트림 키 (인코더에 붙여넣기)에서 ' 표시 '를 선택 하 고 OBS에 붙여 넣을 수 있도록이 키를 복사 합니다.<br>
* OBS/설정/Stream 열기<br>
* YouTube의 스트림 키를 OBS의 스트림 키 필드에 붙여넣습니다.<br>
* 적용, 확인<br>
* OBS에서 스트리밍 시작을 선택 합니다.<br>
* Youtube로 전환 하면 이제 YouTube에 살고 있는 것을 볼 수 있습니다.<br>
* 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택 해야 합니다.<br>
* ' 비디오 링크 '를 복사 하 여 새 브라우저 탭에 붙여 넣으면 YouTube 라이브 스트림 페이지가 표시 됩니다.<br>
* 이 URL은 라이브 스트림 링크 이며 모든 소셜 채널에서 공유할 수 있습니다:)<br>
* 라이브 스트림을 중지 하려면 OBS에서 스트리밍 중지를 선택 합니다. 그러면 YouTube에서 라이브 스트림이 종료 됩니다.<br>
* 그런 다음 YouTube에서 스트림 중지<br>

'**Manage**' 메서드:
* ' 스트림 예약 ' 선택
* 이전에 관리 되는 라이브 스트림을 이미 설정한 경우 새 만들기 또는 설정 다시 사용
* 제목, 날짜, 시작 시간, 설명, 업로드 미리 보기 및 태그를 추가 합니다. AltspaceVR 태그를 잊지 마십시오:)
* 드롭다운 메뉴에서 공용을 선택 합니다 (기본값은 ' 목록 없음 ').
* 기본값 사용
* 스트림 키 복사 (인코더에 붙여넣기)
* 실제 YouTube 라이브 스트림 비디오 페이지를 보려면 오른쪽 위에 있는 공유 아이콘을 선택 해야 합니다. 이는 YouTube 라이브 스트림 이벤트 링크입니다 .이 링크를 실제 이벤트 앞에서 소셜 방식으로 공유할 수 있습니다.
* 이제 OBS를 엽니다.
* 파일/설정
* 스트림
* 복사한 스트림 키를 스트림 키 필드에 붙여넣습니다.
* 적용, 확인
* ' 스트리밍 시작 '을 선택 합니다.
* YouTube로 돌아가서 ' 미리 보기 ' 창이 스트림을 표시 하는 것을 볼 수 있으며 이제 오른쪽 위에 라이브가 켜져 있습니다.
* 라이브 전환 선택
* 이제 살고 있습니다.
* ' 조사식에 보기 ' 페이지가 열려 있는 브라우저 탭으로 이동 하 여 비디오가 제대로 보이는지 확인 합니다. Windows 볼륨 Mixer에서 음소거 할 때 브라우저에서 오디오를 꺼 었으 므로 오디오를 듣지 못합니다. 휴대폰에서 오디오를 확인 하거나 친구에 게 오디오를 확인 하도록 요청 하세요.
* 잘 생각 합니다.
* AltspaceVR로 다시 이동 하 여 이벤트를 중심으로 카메라 (즉, 아바타)를 이동 합니다. Alt-Tab
* 라이브 스트림이 완료 되 면 YouTube의 Live Control 대화방 페이지로 돌아갑니다.
* ' 스트리밍 중지 '를 선택 합니다.
* 대화 상자가 열리고 라이브 이벤트 스트리밍을 중지할지 여부를 확인 합니다.
* OBS로 이동 하 여 스트리밍 중지도 선택 합니다.
* 축 하 합니다, 이제 AltspaceVR 스 트리머!

보너스 점수는 소셜 미디어의 세계와 비디오를 공유 하 고:) 태그를 지정 해야 합니다. @AltspaceVR