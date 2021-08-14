---
title: 개요
description: AltspaceVR, 혼합 현실 확장, 세계 편집기 및 개발 중에 도움을 받는 방법에 대해 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 세계 편집기, Unity 업로더, 포럼
ms.openlocfilehash: 97003073facfa0f4135111fff0ed6128b42ca81b96a8a70fdebef22d8988f548
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126322"
---
# <a name="getting-started-with-altspacevr"></a>AltspaceVR 시작

AltspaceVR 개발자 포럼을 시작합니다. 다음 섹션에서 AltspaceVR에 콘텐츠를 추가할 수 있는 다양한 방법을 살펴봅니다.

## <a name="mixed-reality-extension-mre-sdk"></a>MRE(Mixed Reality 확장) SDK

MRE SDK는 Node.JS 사용하여 AltspaceVR 확장을 빌드하기 위한 새로운 SDK입니다. 시작하기:

1. AltspaceVR(Steam 또는 Oculus Store)을 설치하고, AltspaceVR 계정을 만들고, 앱을 숙지합니다.
2. [Git 명령줄 도구 설치](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
3. [MRE SDK 샘플 리포지토리로](https://github.com/Microsoft/mixed-reality-extension-sdk-samples) 이동하여 단계별 지침에 따라 샘플을 빌드하고 실행합니다.

다음도 가능합니다.

* [MRE SDK Discord Community](https://discord.com/invite/xyBcQec) 조인하여 다른 MRE 개발자와 채팅합니다.
* [Building Tic-Tac-Toe 비디오 시청](https://www.youtube.com/watch?v=DQHrdK9JSXI&ab_channel=AltspaceVR)
* [Visual Studio Code](https://github.com/Microsoft/mixed-reality-extension-sdk#using-visual-studio-code) 사용하여 MRES를 편집하고 빌드하는 방법을 알아봅니다.
* Hello World [소스 코드](https://github.com/Microsoft/mixed-reality-extension-sdk-samples/tree/master/samples/hello-world) 찾아보기
* [AltspaceVR의 주간 개발자 모임에](https://account.altvr.com/channels/sdk) 참여

더 많은 리소스가 곧 출시될 예정입니다.

## <a name="world-editor"></a>세계 편집기

AltspaceVR 내에서 홈 공간에서 기본 제공 세계 편집기를 사용할 수 있습니다. 공간 수정을 시작하는 가장 쉬운 방법입니다. 홈 공간에 있는 경우 오른쪽 아래의 세계 편집기 단추를 선택합니다. 시작 [With World Building 페이지를](../world-building/world-building-getting-started.md)참조하세요. 세계 편집기를 사용하면 3d 개체, MREs(Teleporters 및 확장)를 배치하고 세계 skybox를 변경할 수 있습니다.

초기 액세스 [프로그램에](../world-building/early-access.md)조인하는 경우 [AltspaceVR My Worlds 페이지에서](https://account.altvr.com/users/sign_in)더 많은 세계를 만들 수 있습니다.

웹 사이트, 세계 편집기 및 Unity 업로더를 포함하여 세계를 빌드하는 엔드투엔드 프로세스를 다루는 [Karnivore23의 멋진 비디오도](https://www.youtube.com/watch?v=G8xgR3cDMjk&ab_channel=MarkGill) 있습니다.

## <a name="unity-uploader"></a>Unity 업로더

세계와 사용자 지정 키트 모두에 Unity 업로더를 제공합니다. 이 기능은 개발 초기 단계입니다. 자세히 알아보려면 World [Builders Discord 채널에](https://discord.com/invite/Kp59Frb) 참여하여 채팅하거나 [World Building 도움말 페이지에서](../world-building/getting-help.md)읽어보세요.

Unity 2019.2로 업데이트할 레거시 Unity 2018 키트 또는 템플릿이 있는 경우 [업그레이드 가이드를](https://developer.altvr.com/upgrade-2019-2/)확인하세요.

## <a name="integrating-the-mre-sdk-into-your-own-app"></a>MRE SDK를 사용자 고유의 앱에 통합

Unity3D에서 고유한 앱 또는 게임을 만들고 앱 내에서 MRE를 실행하려면 [MRE Unity 클라이언트 라이브러리](https://github.com/Microsoft/mixed-reality-extension-unity) 리포지토리를 참조하세요.
