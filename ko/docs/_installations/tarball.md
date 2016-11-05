#### 설치 스크립트

macOS와 Unix 게열의 환경에서 Yarn을 설치하는 가장 쉬운 방법 중 하나는 쉘 스크립트입니다.
터미널에서 다음 명령어를 수행하여 Yarn을 설치할 수 있습니다:

```sh
curl -o- -L https://yarnpkg.com/install.sh | bash
```

#### tarball을 이용한 메뉴얼 설치

[tarball를 설치]({{site.baseurl}}/latest.tar.gz)하고 아무 곳에 압축 해제하여 Yarn을 설치할 수 있습니다.

```sh
cd /opt
wget https://yarnpkg.com/latest.tar.gz
tar zvxf yarn-*.tar.gz
# Yarn은 이제 /opt/yarn-[version]/ 에 있습니다
```
