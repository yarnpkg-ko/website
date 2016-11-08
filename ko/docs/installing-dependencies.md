---
id: docs_installing_dependencies
guide: docs_yarn_workflow
layout: guide
additional_reading_tags: ["dependencies", "package-json", "yarn-lock", "cli-install"]
---

버전 제어를 통해서 패키지를 이제 막 [체크아웃](https://www.kernel.org/pub/software/scm/git/docs/git-checkout.html)하였다면
의존성 목록에 있는 패키지들을 설치해야 합니다.

> 만약 프로젝트에 [의존성 패키지를 추가](./managing-dependencies#toc-adding-a-dependency)했다면, 이 패키지들은 추가되는 과정에서 자동으로 설치됩니다.

### 의존성 설치하기 <a class="toc" id="toc-의존성-설치하기" href="#toc-의존성-설치하기"></a>

[`yarn install`](./cli/install)은 프로젝트 내의 모든 의존성을 설치하는 용도로 이용됩니다. 의존성은 프로젝트의 `package.json` 파일과 `yarn.lock` 파일에 저장된 정보로 탐색됩니다.

패키지를 개발하는 동안, 흔히 다음 과정 이후에 의존성을 설치합니다:

1. 패키지를 생성하는 프로젝트의 코드를 이제 막 체크아웃한 경우.
2. 프로젝트의 다른 개발자가 당신이 사용해야 하는 새로운 의존성을 프로젝트에 추가한 경우.

### 설치 선택사항 <a class="toc" id="toc-설치-선택사항" href="#toc-설치-선택사항"></a>

아래와 같은 다양한 선택사항들이 있습니다:

1. `yarn`과 `yarn install`을 이용한 모든 의존성 설치
1. `yarn install --flat`을 이용한 각각 패키지별 버전 하나씩 설치
1. `yarn install --force`를 이용한 모든 의존성 다시 내려받기
1. `yarn install --production`을 이용한 제품용 의존성 설치

`yarn install` 명령어에 추가할 수 있는 플래그에 대한 [모든 목록](./cli/install)을 확인하세요.
