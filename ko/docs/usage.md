---
id: docs_usage
guide: docs_getting_started
layout: guide
additional_reading_tags: ["basics", "cli"]
---

{% include vars.html %}

이제 여러분은 Yarn을 [설치]({{url_base}}/docs/install)했고, Yarn을 사용할 수 있습니다.
여기에 여러분에게 필요한 자주 쓰는 명령어들을 모아봤습니다.

**새로운 프로젝트 시작하기**

```sh
yarn init
```

**의존성 추가하기**

```sh
yarn add [package]
yarn add [package]@[version]
yarn add [package]@[tag]
```

**의존성 업그레이드하기**

```sh
yarn upgrade [package]
yarn upgrade [package]@[version]
yarn upgrade [package]@[tag]
```

**의존성 제거하기**

```sh
yarn remove [package]
```

**프로젝트 내 모든 의존성 설치하기**

```sh
yarn
```

혹은

```sh
yarn install
```
