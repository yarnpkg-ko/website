### 대안들

다른 OS를 사용하고 있거나 OS에 특화된 설정이 작동하지 않는 경우, 몇 가지 대안이 존재합니다.
만약 Node.js를 설치하지 않았다면, [Node.js를 설치](https://nodejs.org/)해야 합니다.

Debian, Ubuntu 그리고 CentOS와 같은 흔한 Linux distributions에서, 우리의 패키지를 통하여 Yarn을 설치하는 것을 추천합니다.

{% include_relative _installations/tarball.md %}

#### npm을 통해서 설치하기

또한 [node package manager](http://npmjs.org/)를 설치했다면 이를 통해서 Yarn을 설치할 수 있습니다.
[Node.js](https://nodejs.org/)를 설치했다면 npm 또한 설치되어 있습니다.

npm을 가지고 있다면 다음 명령어를 실행합니다.

```sh
npm install --global yarn
```

### 경로 설정

#### Unix/Linux/macOS

{% include_relative _installations/unix_path_setup.md %}

#### Windows

{% include_relative _installations/windows_path_setup.md %}
