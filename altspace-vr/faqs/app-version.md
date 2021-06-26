---
title: AltspaceVR app 버전 찾기
description: AltspaceVR 앱, 설정 및 클라이언트 로그를 사용 하 여 현재 실행 중인 AltspaceVR 버전을 찾는 방법에 대해 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 앱 버전
ms.openlocfilehash: 6b710e1724b890fa7ba0eecfcd774ef63128d5b7
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923180"
---
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="60a9c-104">AltspaceVR app 버전 찾기</span><span class="sxs-lookup"><span data-stu-id="60a9c-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="60a9c-105">문제를 해결 하는 과정에서 현재 실행 중인 AltspaceVR 앱의 버전을 묻는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="60a9c-106">AltspaceVR에서</span><span class="sxs-lookup"><span data-stu-id="60a9c-106">In AltspaceVR</span></span>

<span data-ttu-id="60a9c-107">AltspaceVR에서 앱 버전을 찾으려면 **설정 메뉴로** 이동 하 여 왼쪽 탐색 모음에서 **정보** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="60a9c-108">아래 스크린샷에 표시 된 것 처럼 ' 앱 버전 '이 여기에 보고 됩니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![정보 창 열기로 설정 메뉴 열기](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="60a9c-110">Windows 시스템 설정</span><span class="sxs-lookup"><span data-stu-id="60a9c-110">In Windows System Settings</span></span>

<span data-ttu-id="60a9c-111">Microsoft Store을 통해 AltspaceVR를 설치한 경우 Windows 시스템 설정에서 앱 버전을 추가로 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="60a9c-112">이 시나리오는 클라이언트에 성공적으로 로그인 할 수 없는 경우 앱 버전을 보고 하는 경우에 적합 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="60a9c-113">Windows 시스템 설정에서 앱 버전을 찾으려면 **시작 메뉴** 를 열고 **앱 & 기능** 을 입력 한 후 결과를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="60a9c-114">앱 목록에서 **AltspaceVR** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="60a9c-115">AltspaceVR를 마우스 왼쪽 단추를 클릭 하 고 나타나는 메뉴에서 **고급 옵션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![고급 옵션이 강조 표시 된 앱 및 기능 메뉴 열기](images/app-version-img-02.png)

<span data-ttu-id="60a9c-117">**고급 옵션** 의 **사양** 헤더 아래에서 **응용 프로그램 버전이** **버전** 레이블 오른쪽에 나열 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![강조 표시 된 앱 버전으로 고급 옵션 열기](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="60a9c-119">클라이언트 로그</span><span class="sxs-lookup"><span data-stu-id="60a9c-119">In Client Logs</span></span>

<span data-ttu-id="60a9c-120">AltspaceVR는 응용 프로그램 시작 중에 클라이언트 로그 파일의 앱 버전을 "Altspace Version"으로 보고 합니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="60a9c-121">이 옵션은 클라이언트에 성공적으로 로그인 할 수 없는 경우 앱 버전을 가져오는 것이 좋습니다. 그러나 실패 하기 전에 시작 하려고 했습니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="60a9c-122">Windows</span><span class="sxs-lookup"><span data-stu-id="60a9c-122">Windows</span></span>

<span data-ttu-id="60a9c-123">Windows에서 Windows 탐색기를 통해 클라이언트 로그 파일을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

<span data-ttu-id="60a9c-124">AltspaceVR를 시작할 때마다이 파일을 덮어씁니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="60a9c-125">' Player-prev '은 최신 세션을 나타내고 ' s s s. i n s. i n t '는 이전 세션을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="60a9c-126">PowerShell을 통해</span><span class="sxs-lookup"><span data-stu-id="60a9c-126">Via PowerShell</span></span>

<span data-ttu-id="60a9c-127">고급 사용자는 다음과 같이 PowerShell을 통해이 문자열에 대 한 클라이언트 로그를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="60a9c-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="60a9c-128">입력:</span><span class="sxs-lookup"><span data-stu-id="60a9c-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="60a9c-129">출력:</span><span class="sxs-lookup"><span data-stu-id="60a9c-129">Output:</span></span>

<span data-ttu-id="60a9c-130">[2.047] AltspaceVR 버전: 3.2.23. e66c2</span><span class="sxs-lookup"><span data-stu-id="60a9c-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>