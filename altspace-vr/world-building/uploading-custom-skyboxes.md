---
title: 사용자 지정 Skyboxes 업로드
description: AltspaceVR 환경의 사용자 지정 skyboxes 업로드 및 문제 해결에 대한 단계별 지침을 가져옵니다.
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes, 문제 해결
ms.openlocfilehash: 912df5a4c87b7a5817824c6ee75ec8707439636b83b4d46996bbc4129ee6e9de
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126796"
---
# <a name="uploading-custom-skyboxes"></a>사용자 지정 Skyboxes 업로드

Skybox는 환경을 몰입형으로 만드는 세계에 대한 **배경을** 만드는 방법입니다. 다양한 종류의 Skyboxes가 있지만 **현재는 등각형 을** 지원합니다. 다음은 360 카메라를 통해 가져온 예제입니다(더 많은 [예제는 여기).](http://moments.mankindforward.com/) 

![360실의 등각 보기](images/custom-skyboxes-img-01.jpeg)

[Unity 업로더를](world-building-toolkit-getting-started.md) 사용할 수도 있지만 이 방법은 더 간단합니다.

1. [Worlds > Skyboxes로](https://account.altvr.com/skyboxes) 이동하고 오른쪽의 **만들기** 단추를 누릅니다.

![Skyboxes 패널에 열려 있는 Worlds 웹 사이트 페이지](images/custom-skyboxes-img-02.png)

2. 이름을 입력하고 360 이미지를 지정합니다. 사진일 필요는 없으며, 직접 그릴 수 있는 프로그램이 있거나 일부 온라인을 검색할 수 있습니다. 준비가 되면 **만들기** 를 선택합니다. 

![Skybox 만들기 양식](images/custom-skyboxes-img-03.png)

3. 필요에 따라 미리 **보기** 이미지를 업로드하여 이 skybox를 쉽게 식별할 수 있습니다. WAV 형식으로 앰비언트 오디오를 업로드할 수도 있습니다. 

> [!IMPORTANT]
> 360 이미지를 업로드한 후 미리 보기 이미지와 앰비언트 오디오를 별도로 업로드하는 것이 좋습니다. 함께 업로드하는 경우 파일 크기가 충분히 커서 프로세스를 지연시킬 수 있습니다. [](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 앰비언트 오디오와 함께 Skybox를 사용하는 방법의 좋은 예입니다. World-Builder가 오디오 볼륨을 어떻게 낮게 유지했는지, 사람들이 불편해하지 않도록 들으신 소리가 산발적으로 들립니다. 

4. World를 입력하고 세계 편집기를 엽니다. Skyboxes 아래에서 새 Skybox를 선택합니다. 몇 초 후에 하늘이 문자 그대로 변경됩니다. 세계의 다른 사용자도 하늘 변화를 볼 수 있습니다. 다시 전환하려면 동일한 목록에서 **기본** skybox를 선택합니다. 

## <a name="troubleshooting"></a>문제 해결

**하늘 :-(에 이음매 또는 선이 있습니다.** 곧 수정할 버그입니다.

**업로드 실패**
    * 자체적으로 360개 이미지만 업로드해 보세요.
    * 다른 작은 파일을 테스트로 사용해 보세요.

**360개 사진을 찾을 수 없습니다.**
    * 깜박임은 좋은 소스입니다(필터를 변경하여 창의적인 공용 필터를 찾음).
    * 직접 만드세요! 2016년 10월 30일, 2016년 12월 31일, 2016년 12월 
**하늘이 세분성 또는 블로키로 보입니다.** 고해상도 이미지를 찾아야 할 수도 있습니다. 일반적으로 약 2-5MB 및 ~5000픽셀 x 2000픽셀

**내 세계 프레임 속도에 지쳐요!**
이미지가 너무 클 수 있습니다. 생성된 일부 skybox는 8k일 수 있습니다. 일반적으로 모바일 친화적인 2k 버전과 함께 제공됩니다. 이 버전을 사용합니다.

**앰비언트 오디오에 대한 도움말**
    * Audacity와 같은 무료 소프트웨어를 사용하여 볼륨을 줄이거나 고유한 루프를 만듭니다. 오디오가 반복되고 사람들의 난로에서 재생되므로 낮게 유지하고 불편하지 않습니다.
    * [무료 소리는](https://freesound.org/) 무료 사운드의 좋은 소스입니다.
