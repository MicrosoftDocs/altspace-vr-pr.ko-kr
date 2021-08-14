---
title: AltspaceVR 앱 버전 찾기
description: AltspaceVR 앱, 설정 및 클라이언트 로그를 사용하여 현재 실행 중인 AltspaceVR 버전을 찾는 방법을 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 앱 버전
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128255"
---
# <a name="finding-the-altspacevr-app-version"></a>AltspaceVR 앱 버전 찾기

문제를 해결하는 과정에서 현재 실행 중인 AltspaceVR 앱의 버전을 묻는 메시지가 표시될 수 있습니다.

## <a name="in-altspacevr"></a>AltspaceVR에서

AltspaceVR에서 앱 버전을 찾으려면 **설정 메뉴로** 이동하고 왼쪽 탐색 모음에서 **정보** 를 선택합니다. 아래 스크린샷과 같이 여기에서 '앱 버전'이 보고됩니다.

![패널 정보 열기가 있는 설정 메뉴 열기](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>Windows System 설정

Microsoft Store 통해 AltspaceVR을 설치한 경우 Windows 시스템 설정에서 앱 버전을 추가로 찾을 수 있습니다.  이 시나리오는 클라이언트에 성공적으로 로그인할 수 없는 경우 앱 버전을 보고할 때 적합합니다.

Windows 시스템 설정에서 앱 버전을 찾으려면 **시작 메뉴를** 열고 **앱 & 기능을** 입력하고 결과를 선택합니다. 앱 목록에서 **AltspaceVR로** 이동합니다. AltspaceVR을 마우스 왼쪽 단추로 클릭하고 표시되는 메뉴에서 **고급 옵션을** 선택합니다.

![고급 옵션이 강조 표시된 앱 및 기능 메뉴 열기](images/app-version-img-02.png)

고급 **옵션** 의 **사양** 헤더 아래에서 **앱 버전이** **버전** 레이블의 오른쪽에 나열되어야 합니다.

![앱 버전이 강조 표시된 고급 옵션이 열립니다.](images/app-version-img-03.png)

## <a name="in-client-logs"></a>클라이언트 로그에서

AltspaceVR은 애플리케이션을 시작하는 동안 클라이언트 로그 파일의 앱 버전을 "Altspace 버전"으로 보고합니다. 클라이언트에 성공적으로 로그인할 수 없지만 실패하기 전에 시작하려고 시도한 경우 앱 버전을 얻는 것이 좋습니다.

## <a name="windows"></a>Windows

Windows 클라이언트 로그 파일은 Windows 탐색기를 통해 찾을 수 있습니다.

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

이 파일은 AltspaceVR을 시작할 때마다 덮어씁니다. 'Player.log'는 최신 세션을 나타내고 'Player-prev.log'는 이전 세션을 나타냅니다.

## <a name="via-powershell"></a>PowerShell을 통해

고급 사용자는 다음과 같이 PowerShell을 통해 클라이언트 로그에서 이 문자열을 검색할 수 있습니다.

입력:

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

출력:

[2.047] AltspaceVR 버전: 3.2.23.e66c2