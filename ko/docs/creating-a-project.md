---
id: docs_creating_a_project
guide: docs_yarn_workflow
layout: guide
---

이미 코드 저장소/폴더를 가지고 있거나, 완전히 새로운 프로젝트를 시작하더라도,
Yarn을 적용하면 매번 같은 방식으로 작동합니다.


Yarn을 추가하고 싶은 디렉토리(꼭 프로젝트의 최상위 디렉토리여야 합니다.)에서 터미널/콘솔로 다음 명령어를 실행합니다:


```sh
yarn init
```

이 명령어는 아래의 질문들을 통해서 새로운 yarn 프로젝트를 생성하는 입력 가능한 양식을 보여줍니다.


```
name (your-project):
version (1.0.0):
description:
entry point (index.js):
git repository:
author:
license (MIT):
```

각각 질문에 대해서 대답할 수 있고, enter/return키를 누르면
기본값을 사용하거나 빈칸으로 둘 수도 있습니다.

### `package.json` <a class="toc" id="toc-package-json" href="#toc-package-json"></a>

이제 다음과 유사하게 보이는 `package.json`을 갖게 됩니다:

```json
{
  "name": "my-new-project",
  "version": "1.0.0",
  "description": "My New Project description.",
  "main": "index.js",
  "repository": {
    "url": "https://example.com/your-username/my-new-project",
    "type": "git"
  },
  "author": "Your Name <you@example.com>",
  "license": "MIT"
}
```

`yarn init`을 실행하면, 다른 작업은 일절 없이 `package.json` 파일을 생성하는 것이 전부입니다.
여러분이 원하는만큼 마음대로 이 파일을 수정할 수 있습니다.


여러분의 `package.json`은 프로젝트에 관련된 정보를 저장하는 용도로 이용됩니다.
이는 프로젝트 이름, 책임자, 어디에 소스 코드가 존재하는지, 그리고 가장 중요한,
프로젝트에 설치해야 할 의존성들이 무엇인지에 대한 정보를 담고 있습니다.