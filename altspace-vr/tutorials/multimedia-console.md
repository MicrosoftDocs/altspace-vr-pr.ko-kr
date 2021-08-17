---
title: 멀티미디어 콘솔 사용
description: AltspaceVR 환경에서 멀티미디어 콘솔 구성, 게시 및 제어를 시작 하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 콘솔, 멀티미디어
ms.openlocfilehash: a24b3700f1687aed6bc00fd218aacd7cc12908e521af6239fac0ae97f48b4b9a
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127371"
---
# <a name="using-the-multimedia-console"></a>멀티미디어 콘솔 사용

멀티미디어 콘솔은 이벤트와 세계에서 미디어를 공유할 수 있도록 하는 도구입니다. 이를 사용 하 여 이미지, 프레젠테이션 슬라이드, livestreams, 비디오, 재생 목록 등과 같은 항목을 공유할 수 있습니다. 다음은 멀티미디어 콘솔 **v 0.5.0 +** 를 사용 하는 방법에 대 한 단계별 지침입니다. 

## <a name="getting-started"></a>시작

멀티미디어 콘솔 시작은 두 부분으로 이루어진 프로세스입니다.  먼저 사용자 환경에 배치한 멀티미디어 콘솔 세션의 구성을 생성 하 고 게시 하는 데 사용할 웹 포털이 있습니다.  두 번째는 사용자 환경에서 실제 멀티미디어 콘솔 앱을 배치 하 고 사용 해야 하는 구성 코드를 설정 하는 것입니다.

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>웹 포털을 사용 하 여 멀티미디어 콘솔 구성

1. 먼저 URL이 필요 하므로 콘텐츠가 온라인으로 호스트 되는지 확인 해야 합니다. (Altvr.com에 사진을 업로드 하 고, 온라인으로 비디오 .mp4 파일을 호스트 하거나, d 라이브 라이브 스트림 링크를 사용할 수 있습니다. https://dlive.tv/yourlivestream) 
2. 에서 멀티미디어 콘솔용 웹 포털로 이동 합니다. [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. 웹 포털에서 멀티미디어 콘솔에 대 한 구성을 생성 하 고 게시할 수 있습니다.  다양 한 속성에 대 한 자세한 내용은 아래를 참조 하세요.
4. 미디어 목록에 미디어를 입력 하 고 일반 설정을 구성한 후에는 앱의 오른쪽 위 부분에서 게시 단추를 선택 합니다.
5. 게시가 완료 되 면 사용자가 배치 된 멀티미디어 콘솔에 입력할 수 있는 두 가지 단어 코드가 포함 된 대화 상자가 나타납니다.
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>사용자 환경에 멀티미디어 콘솔 배치

1. **세계 편집기 > 편집기 패널 > SDK 앱 > 멀티미디어 콘솔** 을 선택 합니다. (등록 되지 않은 앱에 대 한 **기본 > SDK 앱을 위한 세계 편집기 > 기본 사항** 으로 이동 하지 마세요.)  
2. 멀티미디어 콘솔을 스페이스와 대상의 가장 적합 한 도구 모음으로 배치 합니다.
3. 주황색 편집 모드 단추를 클릭 하 여 편집 모드를 시작 합니다.
4. **Media player 소유자에** 게 메시지가 표시 되나요? 이 멀티미디어 콘솔 세션의 공식 소유자 여야 하는 사용자 인 경우를 확인 하 고 계속 합니다. (다른 permissioned 역할도 사용할 수 있습니다. 자세한 목록은 아래를 참조 하세요.)
5. 예를 선택 하 여 기본 호스트 임을 확인 합니다.  
6. 웹 포털 또는 유효한 JSON에서 코드를 입력 하 라는 대화 상자가 표시 됩니다.  대시를 포함 하 여 웹 포털에서 두 개의 단어 코드를 입력 하 고 확인을 누릅니다. (JSON은 아래에 설명 된 고급 구성)
7. 웹 포털에서 구성한 구성을 사용 하 여 몇 초 후에 멀티미디어 콘솔을 로드 해야 합니다.

### <a name="controlling-the-multimedia-console"></a>멀티미디어 콘솔 제어

1. 코드를 입력 하 고 구성 프로세스를 완료 한 후에는 미디어 표시 아래에 컨트롤 단추가 표시 됩니다. 
    * **Play** 미디어 뷰어를 시작 하거나 현재 항목에서 이전에 중지 된 경우 다시 시작 합니다. 
    * **Stop** 은 미디어 뷰어를 중지 하 고 현재 미디어를 숨깁니다.  
    * **다음/** 이전 미디어로 건너뜁니다. 
    * **x/x**   미디어 목록에 현재 인덱스를 표시 하 고 목록에서 임의의 지점으로 이동할 수 있도록 합니다.
    * **Config** 는 웹 포털에서 새 코드를 새로 입력할 수 있도록 하 여 콘솔에 새 구성을 설정 합니다. 

이제 멀티미디어 콘솔을 통해 공유를 시작 하도록 설정 되었습니다.  
 
## <a name="working-with-the-web-portal"></a>웹 포털 작업

웹 포털은 멀티미디어 콘솔의 다양 한 기능을 구성 하는 데 사용할 수 있는 웹 앱입니다.  이러한 기능은 두 가지 범주로 나뉩니다. 일반 미디어 콘솔 설정 및 미디어 재생 목록.

### <a name="multimedia-console-general-settings"></a>멀티미디어 콘솔 일반 설정

**Playback 설정**

미디어 목록에 대 한 일반 재생 설정

* **반복 미디어 목록**-목록의 끝에 도달 하면 미디어 목록이 루프를 반복 해야 하는지 여부를 결정 합니다.
* **시작 방법** -멀티미디어 콘솔을 시작할 방법을 선택 합니다.
    * 수동-미디어를 시작 하기 전에 재생 단추를 누를 때까지 대기 합니다.
    * 시작부터 자동 시작-목록의 처음부터 미디어 목록을 자동으로 시작 합니다.
    * 자동 시작 무작위-목록의 임의의 시작 지점에서 미디어를 자동으로 시작 합니다.

**역할**

멀티미디어 콘솔을 제어 하 고 구성 하기 위한 역할 할당    이러한 역할은 다음 집합으로 세분화 됩니다.

* **Owner Only** -멀티미디어 콘솔 세션의 소유자 인 사용자입니다.
* **관리자 권한** -원래는 멀티미디어 콘솔이 구성 된 공간에서 중재자 또는 호스트 역할을 하는 사용자입니다.
* **모든 사용자** -모든 사용자

이러한 역할은이 목록에서 선택한 항목 위의 모든 역할에도 해당 기능을 사용할 수 있는 권한이 부여 된다는 점에서 스택 합니다.  예: **승격 된 사용자** 는 AltspaceVR의 중재자 또는 host * *가 아닌 경우에도 **소유자** 를 포함 합니다. 역할 할당에 의해 제어 되는 기능은 다음과 같습니다.

* **미디어 플레이어 제어 가능** -멀티미디어 콘솔의 미디어 재생 단추를 제어할 수 있는 역할을 결정 합니다.
* **미디어 플레이어 구성 가능** -구성 단추에 대 한 액세스 권한을 부여 하 여 멀티미디어 콘솔을 구성할 수 있는 역할을 **결정 합니다.**

### <a name="adding-photos-and-videos-to-the-media-list"></a>미디어 목록에 사진 및 비디오 추가

미디어는 멀티미디어 콘솔의 핵심입니다.  이미지 및 비디오 링크는 멀티미디어 콘솔 내에서 미디어 유형으로 지원 됩니다.  새 미디어를 추가 하려면 **이미지 추가** 또는 **비디오 아이콘 추가** 를 선택 하 여 미디어 정보 및 설정을 입력 하는 대화 상자를 표시 합니다.  다음은 미디어 유형 및 연결 된 설정에 대 한 분석입니다.

**이미지**

이미지는 jpeg, png 및 son과 같은 표준 이미지 형식 이어야 합니다. 공용 링크를 사용 하 여 어딘가에 호스팅해야 합니다.

* **이름** -(필수) 이미지를 식별 하려는 이름입니다.
* **이미지 URL** -(필수) 이미지의 공용 URL
* **다음 이후 건너뛰기** -이미지를 건너뛸 때까지 걸리는 시간 (초)입니다.

**비디오**

비디오는 Twitch 및 Flive를 통해 호스트 되는 비디오 또는 라이브 스트림이 될 수 있습니다.  (다른 지원은 적절 한 스트림 url을 가져오기 위해 추가 작업으로 작동할 수 있지만 멀티미디어 콘솔 내에서 완전히 지원 되지 않습니다.)

* **이름** -(필수) 비디오를 식별 하려는 이름입니다.
* **비디오 url** -(필수) 비디오가 호스트 되거나 라이브 스트림이 제공 되는 공용 URL입니다.
* **다음 이후 건너뛰기** -후에 비디오를 건너뛰어야 하는 시간 (초)입니다.

> [!NOTE]
> 필수: 비디오를 올바르게 전달할 수 있도록 비디오 길이와 일치 하는 시간을 입력 합니다. 예를 들어 비디오가 5 분 길이의 경우 300 초에 배치 되 면 비디오가 다음 내용으로 건너뛰지 않습니다.

* **볼륨** -0 (분)-1 (최대) 값의 비디오 볼륨입니다.
* **시작 시간** -비디오 시작부터 시작 되는 시간 (초)입니다.
* **시작 거리 롤오버** -멀티미디어 콘솔에서 이동할 때 볼륨이 표시 되기 시작 하는 세계 미터 단위 거리입니다.
* **비디오 작업 끝** -비디오의 끝에 도달한 후 수행할 작업입니다.
    * 중지-비디오가 끝난 후 미디어 목록이 중지 됨
    * Loop-수동으로 건너뛸 때까지 비디오가 반복 됩니다.
    * 다음 재생-미디어 목록의 다음 미디어가 현재 비디오가 종료 된 후에 시작 됩니다.

## <a name="working-with-json-directly-advancedoptional"></a>JSON 직접 작업 (고급/옵션)

멀티미디어 콘솔은 AltspaceVR에서 콘솔의 프롬프트에 직접 JSON을 입력 하는 것을 지원 합니다.  JSON은 미디어 플레이어 구성을 사용 하는 내부 메커니즘입니다. JSON을 직접 설정 하는 기능을 제공 하는 것은 고급 사용자가 JSON에 대 한 요구 사항 및 친숙 한 워크플로를 직접 만들 수 있도록 하는 것입니다.  Json 구조와 json의 유효성을 검사 하는 스키마에 대 한 간략 한 설명은 다음과 같습니다. 아래 속성에 대 한 자세한 내용은 멀티미디어 콘솔 구성에 대해 설명 하는 위의 섹션을 참조 하세요.  이 섹션에서는 주로 JSON 데이터에 대 한 스키마 예제 및 구조에 대해 집중적으로 설명 합니다.

### <a name="global-media-settings"></a>글로벌 미디어 설정

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>미디어 목록

미디어 목록은 역할 및 재생 설정와 같이 JSON 구조의 루트에 설정 된 속성입니다.  다음 미디어 구성 구조 중 하나를 포함할 수 있는 간단한 배열입니다. (각 가 수행하는 일에 대한 자세한 내용은 위의 속성 설명을 참조하세요.)

**이미지 예제**

*필수 필드: "name" 및 "imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**비디오 예제**

*필수 필드: "name" 및 "videoUrl"*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>예제 JSON

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>스키마

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> 멀티미디어 콘솔 v0.5.0을 사용하여 최신