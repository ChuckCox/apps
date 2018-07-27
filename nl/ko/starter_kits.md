---

copyright:
  years: 2018
lastupdated: "2018-07-05"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}

# 앱 개발
{: #intro}

{{site.data.keyword.cloud_notm}} 개발자 콘솔을 사용하면 개발자가 스타터 킷, 프로비저닝 및 연결 키 {{site.data.keyword.cloud_notm}}-최적화 서비스를 통해 앱을 작성한 다음 작업 코드를 신속하게 다운로드하거나 지속적 딜리버리를 설정할 수 있습니다. 앱을 작성, 보기, 구성 및 관리하고 앱의 코드를 다운로드할 수 있습니다. 스타터 킷을 사용하면 샘플 앱으로 {{site.data.keyword.cloud_notm}} 서비스를 쉽게 평가하고 테스트할 수 있습니다.
{:shortdesc}

## 스타터 킷 개념
{: #starter_kits}

스타터 킷은 클라우드 배치 준비가 되어 있는 사용자가 선택한 언어로 스켈레톤 프로덕션 앱을 동적으로 조립하는 데 매우 유용합니다. 각 스타터 킷에는 특정한 실제 유스 케이스에 대한 언어, 프레임워크 및 패턴이 있습니다. 코드를 다시 작성하지 않고 재사용할 수 있습니다.

### 샘플과 스타터 킷 비교

개발자는 종종 스니펫, 데모 및 샘플과 같이 사전에 작성된 코드를 사용합니다. 스니펫, 데모 및 샘플과 {{site.data.keyword.cloud_notm}} 스타터 킷의 차이점을 어떻게 설명할 수 있습니까?

* **스니펫** - IDE에서 종종 표시되는 몇 줄로 된 코드입니다. 스니펫은 개발자가 프로그래밍 언어 구문을 통합하도록 도와주거나 정의된 API와 통합을 지원합니다.

* **데모** - 주로 고품질, 고성능의 코드로 서비스 범위와 통합 지점을 사용합니다. 종종 설정이 필요하며 비즈니스 문제점을 증명하거나 플랫폼 기능을 시연할 때 사용됩니다. 데모는 클라우드 채택 단계를 평가할 수 있습니다. 때때로 코드가 프로덕션 코드에 포함되어 있습니다.

* **샘플** - 특정 기능, 함수, 서비스 또는 사용자 과정의 작은 예제가 포함된 코드입니다. 샘플은 프로덕션 애플리케이션에서 재사용되거나 포함될 수 있습니다. 샘플을 사용하여 기술적 문제점을 해결하기 위한 기술적 기능과 가능한 접근 방법을 표시할 수 있습니다.

* **{{site.data.keyword.cloud_notm}} 스타터 킷** - 스타터 킷은 프로덕션 준비 자산을 생성하기 위한 일련의 서비스와 통합할 수 있는 프로덕션 준비 패턴입니다. 스타터 킷을 DevOps 파이프라인과 Kubernetes 클러스터에 직접 배치할 수 있습니다. 스타터 킷은 킷이 무엇이고 어떤 일을 하는지 알 수 있도록 사용자에게 충분한 정보를 제공하는 설명 메타데이터를 포함합니다. 또한 무엇을 생성할 것인지 {{site.data.keyword.cloud_notm}}에게 알려주는 지시사항을 포함합니다. 출력은 더 향상될 수 있습니다. 스타터 킷 컨텐츠는 데모만큼 복잡하지 않고 스니펫이나 샘플처럼 간단하지 않습니다. 스타터 킷은 사용자의 요구사항에 따라 동적으로 작성됩니다.

  스타터 킷은 런타임(예: Swift 및 Kitura)과 함께 주요 패턴 구현을 보여줍니다. 서비스 통합을 강조하기 위해 단순 사용자 환경이 포함되어 있을 수 있습니다. 스타터 킷은 정교한 유스 케이스를 사용자 정의할 수 있는 구현입니다.

  스타터 킷에는 {{site.data.keyword.cloud_notm}}에서 이동 가능한 코드로 스캐폴딩 앱 프로젝트를 자동으로 생성할 수 있는 지시사항이 포함되어 있습니다. 또한 프로젝트를 작성할 때 리소스를 자동 프로비저닝하도록 지정할 수도 있습니다.

## 자동 프로비저닝된 리소스
{: #auto_privisioned_resources}

스타터 킷이 필수 리소스를 지정하는 경우 사용자가 프로젝트를 작성할 때 {{site.data.keyword.cloud_notm}}에서 이러한 리소스를 자동으로 작성합니다. 프로젝트가 작성된 후에 리소스를 수동으로 프로비저닝하거나 기존 리소스 인스턴스를 선택하여 프로젝트를 보강할 수 있습니다. 필요한 경우 신임 정보와 함께 *프로젝트 세부사항*보기에서 프로젝트와 연관된 서비스 인스턴스 목록을 볼 수 있습니다.

## 이동 가능한 코드 생성
{: #portable_code}

스타터 킷에서 앱을 작성하면 일관된 형식을 가지며 런타임 독립적인 코드가 자동으로 생성됩니다. 코드를 선택한 환경(예: Kubernetes 또는 Cloud Foundry)에 변경 없이 배치할 수 있습니다.

이 프로젝트에는 프로젝트의 기술적인 세부사항이 포함된 `README` 파일이 포함되어 있으며 앱을 실행할 준비가 되려면 무엇이 필요한지에 대해 설명합니다.

자세한 정보는 [Apple 러닝 리소스를 위한 {{site.data.keyword.cloud_notm}} 개발자 콘솔](https://console.bluemix.net/developer/appledevelopment/learning-resources)을 참조하십시오.
{: tip}

### 생성되는 앱 컨텐츠
{: #content}

{{site.data.keyword.cloud_notm}} 스타터 킷에서 생성되는 코드에는 네 개의 기본 컴포넌트가 있습니다. 즉, 유스 케이스 로직, 언어 컴포넌트, 서비스 인에이블먼트 그리고 클라우드 인에이블먼트입니다. 이러한 컴포넌트를 생성하면 귀중한 시간을 절약하고 최고의 아키텍처를 사용할 수 있습니다.

* **유스 케이스 로직**은 특정한 유스 케이스에 대한 코드입니다. 예제에는 Watson Conversation 챗봇용 코드 또는 모바일 시각적 인식 앱용 코드가 포함되어 있습니다.
* **언어 컴포넌트**는 스타터 킷을 위해 선택한 언어에 특정한 코드 컴포넌트 및 파일입니다. 예를 들어, node.js 프로그래머는 종속성 관리를 위해 `package.json` 파일이 필요하며 이 파일은 {{site.data.keyword.cloud_notm}} 개발자 환경에서 자동으로 작성됩니다.
* **서비스 인에이블먼트**는 앱에서 프로젝트에 연결하고 사용자가 추가한 서비스를 사용할 수 있게 하는 코드입니다. 서비스 인에이블먼트의 예로는 신임 정보 관리, 초기화 코드 및 서비스 특정 SDK가 있습니다.
* **클라우드 인에이블먼트**는 앱을 {{site.data.keyword.cloud_notm}}에서 실행할 수 있게 하는 코드입니다. 예를 들어 Helm 차트를 사용하면 {{site.data.keyword.cloud_notm}} Kubernetes 클러스터에서 실행할 앱이 클라우드 인에이블먼트 카테고리에 포함될 수 있습니다.

{{site.data.keyword.cloud_notm}}에서 생성된 앱은 구조적으로 양호하며 프로젝트에 선택한 언어에 대한 우수 사례를 모델링합니다. 앱 프로젝트의 파일 및 구조에 대한 세부사항을 보려면 다음 주제를 참조하십시오.

* [Java 앱 파일](/docs/apps/projects/java_project_contents.html)
* [Node.js 앱 파일](/docs/apps/projects/node_project_contents.html)
* [Python 앱 파일](/docs/apps/projects/python_project_contents.html)
* [Swift 앱 파일](/docs/apps/projects/swift_project_contents.html).