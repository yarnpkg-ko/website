---
id: docs_version_control
guide: docs_yarn_workflow
layout: guide
additional_reading_tags: ["dependencies", "package-json", "yarn-lock"]
---

다른 개발자들이 당신의 패키지를 개발하거나 이용하려면, 필요한 모든 파일들을 소스 제어 시스템에 확실히 등록해야 합니다.

### 필요한 파일들 <a class="toc" id="toc-필요한-파일들" href="#toc-필요한-파일들"></a>

다른 개발자가 여러분의 패키지를 관리하려면 아래의 파일들이 꼭 소스 제어에 포함되야 합니다.

- `pakcage.json`: 여러분의 패키지가 의존하는 패키지들에 대한 목록을 포함합니다.
- `yarn.lock`: 여러분의 패키지가 의존하는 패키지 각각의 정확한 버전을 저장합니다.
- 당신의 패키지에 기능성을 부여하는 실제 소스 코드들

> Yarn 패키지에서 필요한 최소의 요구사항을 담은 [Yarn 예제 패키지](https://github.com/yarnpkg/example-yarn-package)를 직접 확인해보세요.
