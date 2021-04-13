---
title: 개요
description: AltspaceVR, mixed reality 확장, 전 세계 편집기 및 개발 하는 동안 도움을 받는 방법에 대해 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 세계 편집기, unity 업 로더, 포럼
ms.openlocfilehash: e2277e1425af72544d2e1ed450e01a15ff537039
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213107"
---
# <a name="getting-started-with-altspacevr"></a>AltspaceVR 시작 하기

AltspaceVR 개발자 포럼을 시작 합니다. 다음 섹션에서 AltspaceVR에 콘텐츠를 추가할 수 있는 여러 가지 방법을 살펴봅니다.

## <a name="mixed-reality-extension-mre-sdk"></a>혼합 현실 확장 (MRE) SDK

MRE SDK는 Node.JS을 사용 하 여 AltspaceVR 확장을 빌드하기 위한 새로운 SDK입니다. 시작하기:

1. AltspaceVR (스트림 또는 Oculus 스토어에서)를 설치 하 고, AltspaceVR 계정을 만들고, 앱을 숙지 합니다.
2. [Git 명령줄 도구 설치](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
3. [Mre SDK 샘플 리포지토리로](https://github.com/Microsoft/mixed-reality-extension-sdk-samples) 이동 하 고 단계별 지침에 따라 샘플을 빌드하고 실행 합니다.

또한 다음을 수행할 수 있습니다.

* [MRE SDK Discord 커뮤니티](https://discord.com/invite/xyBcQec) 에 가입 하 여 다른 mre 개발자와 채팅할 수 있습니다.
* [빌딩 3 목 비디오 보기](https://www.youtube.com/watch?v=DQHrdK9JSXI&ab_channel=AltspaceVR)
* [Visual Studio Code](https://github.com/Microsoft/mixed-reality-extension-sdk#using-visual-studio-code) 를 사용 하 여 mres를 편집 및 빌드하는 방법을 알아봅니다.
* [헬로 월드 소스 코드](https://github.com/Microsoft/mixed-reality-extension-sdk-samples/tree/master/samples/hello-world) 찾아보기
* [AltspaceVR의 주간 개발자 모임을](https://account.altvr.com/channels/sdk) 참여

추가 리소스 제공 예정

## <a name="world-editor"></a>세계 편집기

AltspaceVR 내에서 기본 제공 세계 편집기를 홈 공간에 사용할 수 있습니다. 이 방법은 공간 수정을 시작 하는 가장 쉬운 방법입니다. 홈 공간에 있는 경우 오른쪽 아래에서 전 세계 편집기 단추를 선택 합니다. [세계 빌드 시작 페이지](../world-building/world-building-getting-started.md)를 참조 하세요. 세계 편집기를 사용 하 여 3d 개체, teleporters 및 확장 (MREs)을 놓고 세계 skybox를 변경할 수 있습니다.

[초기 액세스 프로그램](../world-building/early-access.md)에 참여 하는 경우 [AltspaceVR My 세계 페이지](https://account.altvr.com/users/sign_in)에서 더 많은 환경을 만들 수 있습니다.

또한 웹 사이트, 전 세계 편집기 및 Unity 업 로더를 비롯 하 여 빌드에 대 한 종단 간 프로세스를 다루는 [Karnivore23의 훌륭한 비디오가](https://www.youtube.com/watch?v=G8xgR3cDMjk&ab_channel=MarkGill) 있습니다.

## <a name="unity-uploader"></a>Unity 업 로더

Microsoft는 세계 및 사용자 지정 키트 모두에 대해 Unity 업 로더를 제공 합니다. 이 기능은 개발 초기에 진행 됩니다. 자세히 알아보려면 [세계 빌더가 Discord 채널](https://discord.com/invite/Kp59Frb) 을 연결 하 여 채팅에 참여 하거나, [전 세계의 도움말 페이지](../world-building/getting-help.md)를 참조 하세요.

레거시 Unity 2018 키트 또는 템플릿을 Unity 2019.2로 업데이트 하는 경우 [업그레이드 가이드](https://developer.altvr.com/upgrade-2019-2/)를 확인 하세요.

## <a name="integrating-the-mre-sdk-into-your-own-app"></a>사용자 고유의 앱에 MRE SDK 통합

Unity3D에서 사용자 고유의 앱 또는 게임을 만든 경우 앱 내에서 MREs를 실행 하려면 [Mres Unity 클라이언트 라이브러리](https://github.com/Microsoft/mixed-reality-extension-unity) 리포지토리를 살펴보세요.
