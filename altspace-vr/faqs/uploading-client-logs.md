---
title: 클라이언트 로그를 업로드 어떻게 할까요??
description: AltspaceVR와 관련 된 문제가 발생할 때 사용 가능한 클라이언트 로그 필드와 클라이언트 로그를 업로드 하는 방법에 대해 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 클라이언트 로그
ms.openlocfilehash: e2fe1ea8b8070ca4c7d290269974610ce84f9cea
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923170"
---
# <a name="how-do-i-upload-my-client-logs"></a><span data-ttu-id="627d3-104">클라이언트 로그를 업로드 어떻게 할까요??</span><span class="sxs-lookup"><span data-stu-id="627d3-104">How do I upload my client logs?</span></span>

<span data-ttu-id="627d3-105">AltspaceVR client 응용 프로그램은 AltspaceVR를 사용 하는 동안 발생 하는 진단 데이터 및 이벤트 로그를 보관 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-105">The AltspaceVR client application keeps a log of diagnostic data and events that occur while you're using AltspaceVR.</span></span> <span data-ttu-id="627d3-106">문제를 해결 하는 과정에서 팀에서 검토할 수 있도록 로그를 "업로드" 하 라는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-106">In the course of troubleshooting an issue, you may be asked to "upload your logs" so that our team can review them.</span></span> <span data-ttu-id="627d3-107">이 기능을 사용 하 여 문제를 해결 하는 데 도움이 되도록 팀에 로컬 로그 콘텐츠를 보낼 수 있는 AltspaceVR의 기능입니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-107">This is a feature of AltspaceVR that allows you to send our team your local log content to help us troubleshoot your issue.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="627d3-108">AltspaceVR에서</span><span class="sxs-lookup"><span data-stu-id="627d3-108">In AltspaceVR</span></span>

<span data-ttu-id="627d3-109">AltspaceVR에서 클라이언트 로그를 업로드 하려면 **설정 메뉴로** 이동 하 여 왼쪽 탐색 모음에서 **지원** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-109">To upload client logs in AltspaceVR, navigate to the **settings menu** and select **Support** in the left navigation bar.</span></span> <span data-ttu-id="627d3-110">아래 스크린샷에 표시 된 것 처럼 로그를 업로드 하기 위한 몇 가지 옵션을 여기에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-110">Several options to upload logs are available here, as shown in the screenshot below.</span></span>

![지원 패널 열기 및 로그 필드가 강조 표시 된 설정 메뉴](images/help-altvr-uploadlogs.png)

## <a name="fields"></a><span data-ttu-id="627d3-112">필드</span><span class="sxs-lookup"><span data-stu-id="627d3-112">Fields</span></span>

<span data-ttu-id="627d3-113">**"무엇이 문제 인가요?"**</span><span class="sxs-lookup"><span data-stu-id="627d3-113">**"What Went Wrong?"**</span></span>
<span data-ttu-id="627d3-114">발생 한 상황을 설명 합니다. 예를 들어, 버그를 발견 한 경우 실제로 발생 한 상황에 대비 하 여 예상 되는 결과를 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-114">Describe what happened - for example, if you find a bug, describe what you expected to happen in contrast to what actually happened).</span></span> <span data-ttu-id="627d3-115">이 정보는 업로드를 누를 때 로그와 함께 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-115">This information will be sent along with the log when you press upload.</span></span>

<span data-ttu-id="627d3-116">**"로그 업로드"** 이 단추는 현재 세션에서 로그를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-116">**"Upload Logs"** This button will upload logs from the current session.</span></span> <span data-ttu-id="627d3-117">이 세션에서 문제가 발생 하는 경우 (예: AltspaceVR client를 닫지 않은 경우)이 옵션을 사용 하 고 보고 하려는 경우에이 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-117">Use this option if you find an issue in this same session (for example, if you haven't closed the AltspaceVR client) and would like to report it.</span></span>

<span data-ttu-id="627d3-118">**"마지막 로그 업로드"** 이 단추는 이전 세션에서 로그를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-118">**"Upload Last Logs"** This button will upload logs from the previous session.</span></span>

<span data-ttu-id="627d3-119">**"마지막 크래시 로그 업로드"** 이 단추를 클릭 하면 발생 한 최신 크래시에서 더 많은 로그 콘텐츠가 업로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-119">**"Upload Last Crash Log"** This button will upload more log content from the latest crash you've experienced.</span></span>

## <a name="in-client-logs"></a><span data-ttu-id="627d3-120">클라이언트 로그</span><span class="sxs-lookup"><span data-stu-id="627d3-120">In Client Logs</span></span>

<span data-ttu-id="627d3-121">컴퓨터에서 로그 파일을 검색할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-121">You can also retrieve your log files from your computer.</span></span> <span data-ttu-id="627d3-122">이러한 로그를 검색 하는 방법에 대 한 지침은 [여기](https://docs.microsoft.com/windows/mixed-reality/altspace-vr/faqs/app-version#in-client-logs)에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-122">Instructions on how to retrieve these logs can be found [here](https://docs.microsoft.com/windows/mixed-reality/altspace-vr/faqs/app-version#in-client-logs).</span></span>

<span data-ttu-id="627d3-123">이러한 파일을 찾았으면 제출을 클릭 하기 전에 [지원 티켓을 열고](https://help.altvr.com/hc/en-us/requests/new) 티켓 요청에 로그를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="627d3-123">Once you've located those files, [open a support ticket](https://help.altvr.com/hc/en-us/requests/new) and upload your logs on your ticket request before clicking submit.</span></span>
