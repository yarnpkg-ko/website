
### Windows

Windows에서 Yarn을 설치하는 두가지 방법이 있습니다.

#### 인스톨러 내려받기

이 방법은 실행시 Windows에 Yarn을 설치하는 `.msi` 파일을 제공합니다.

인스톨러를 사용하려면 [Node.js](https://nodejs.org/)를 먼저 설치해야합니다.

<a class="btn btn-primary" href="https://yarnpkg.com/latest.msi">인스톨러 내려받기</a>

#### Chocolatey로 설치하기

[Chocolatey](https://chocolatey.org/)는 Windows를 위한 패키지 매니저이고, [다음 방법](https://chocolatey.org/install)으로
Chocolatey를 설치합니다.

Chocolatey를 설치하면 다음 명령어를 콘솔에 입력해서 yarn을 설치합니다:

```sh
choco install yarn
```

[Node.js](https://nodejs.org/)가 설치되어 있어야 합니다.

#### 주의
프로젝트 폴더와 Yarn 캐시 폴더 (%LocalAppData%\Yarn) 를 안티바이러스 화이트 리스트에 추가해주세요. 그렇지 않으면 내려 받은 모든 파일들을 일일이 검사하기 때문에 패키치 설치가 현저하게 느려집니다.
