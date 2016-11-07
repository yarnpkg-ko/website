---
id: docs_managing_dependencies
guide: docs_yarn_workflow
layout: guide
additional_reading_tags: ["dependencies", "package-json", "yarn-lock", "cli-add", "cli-upgrade", "cli-remove"]
---

{% include vars.html %}

의존성을 추가하거나 갱신하거나 삭제하고 싶은 경우, 몇 가지 명령어에 대해 알고 있어야 합니다.


각각 명령어는 자동으로 여러분의
[`package.json`]({{url_base}}/docs/package-json)과
[`yarn.lock`]({{url_base}}/docs/yarn-lock) 파일을 갱신합니다.

### 의존성 추가하기 <a class="toc" id="toc-의존성-추가하기" href="#toc-의존성-추가하기"></a>

다른 패키지를 사용하고 싶다면, 먼저 의존성 목록에 추가해야합니다.
그러기 위해서 다음 명령어를 실행합니다:

```sh
yarn add [package]
```

이 명령어는 자동으로 `package.json` 파일의 의존성 목록에 `[package]`를 추가합니다.
뿐만 아니라, 변동 사항을 반영하기 위해 `yarn.lock` 파일을 갱신합니다.

```diff
  {
    "name": "my-package",
    "dependencies": {
+     "package-1": "^1.0.0"
    }
  }
```

또한 플래그를 사용하여 다른 [종류의 의존성]({{url_base}}/docs/dependency-types)
을 추가할 수 있습니다:

- `yarn add --dev` to add to `devDependencies`
- `yarn add --peer` to add to `peerDependencies`
- `yarn add --optional` to add to `optionalDependencies`

[의존성 버전]({{url_base}}/docs/dependency-versions)이나 [태그]({{url_base}}/docs/cli/tag)를
명시하여 설치하고 싶은 버전의 패키지를 특정할 수 있습니다.

```sh
yarn add [package]@[version]
yarn add [package]@[tag]
```

`[버전]`이나 `[태그]`는 `package.json` 파일에 추가되고 의존성을 설치할때 이용됩니다.

For example:

```sh
yarn add package-1@1.2.3
yarn add package-2@^1.0.0
yarn add package-3@beta
```

```json
{
  "dependencies": {
    "package-1": "1.2.3",
    "package-2": "^1.0.0",
    "package-3": "beta"
  }
}
```



### 의존성 판올림하기 <a class="toc" id="toc-의존성-판올림하기" href="#toc-의존성-판올림하기"></a>

```sh
yarn upgrade [package]
yarn upgrade [package]@[version]
yarn upgrade [package]@[tag]
```

이 명령어는 `package.json`과 `yarn.lock` 파일을 판올림합니다.

```diff
  {
    "name": "my-package",
    "dependencies": {
-     "package-1": "^1.0.0"
+     "package-1": "^2.0.0"
    }
  }
```

### 의존성 제거하기 <a class="toc" id="toc-의존성-제거하기" href="#toc-의존성-제거하기"></a>

```sh
yarn remove [package]
```

이 명령어는 `package.json`과 `yarn.lock` 파일을 갱신합니다.
