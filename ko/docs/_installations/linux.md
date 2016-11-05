### Debian/Ubuntu Linux

Debian 혹은 Ubntu Linux에서, Debian 패키지 저장소를 통해서 내려받을 수 있습니다.
먼저 저장소를 설정해야 합니다:

```sh
sudo apt-key adv --fetch-keys http://dl.yarnpkg.com/debian/pubkey.gpg
echo "deb http://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
```

Ubuntu 14.04와 Debian Stable에서, 새로운 버전의 Node.js를 얻기 위해서 [NodeSource 저장소](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)를 설정해야 합니다.
(Debian Testing과 Ubuntu 16.04에서는 충분한 버전의 Node.js가 패키지로 제공되기 때문에 이 과정이 필요 없습니다.)

그 후에 간단하게 아래 명령어를 실행합니다:

```sh
sudo apt-get update && sudo apt-get install yarn
```

### CentOS / Fedora / RHEL

CentOs, Fedora 그리고 RHEL에서, RPM 패키지 저장소를 통해서 Yarn을 설치할 수 있습니다.
```sh
sudo wget https://dl.yarnpkg.com/rpm/yarn.repo -O /etc/yum.repos.d/yarn.repo
```

만약 Node.js가 설치되어 있지 않다면, [NodeSource 저장소](https://nodejs.org/en/download/package-manager/#enterprise-linux-and-fedora)를 설정해야합니다:
```sh
curl --silent --location https://rpm.nodesource.com/setup_6.x | bash -
```

그 후에 간단하게 아래 명령어를 실행합니다:
```sh
sudo yum install yarn
```

### Arch Linux

Arch Linux에서, **AUR**을 통해서 Yarn을 설치할 수 있습니다.

yaourt와 같은 [AUR Helper](https://wiki.archlinux.org/index.php/AUR_helpers)를 사용하고 있다면 간단하게 아래 명령어를 실행합니다:
```sh
yaourt -S yarn
```

### Solus

Solus에서 Solus 저장소를 통해서 yarn을 설치할 수 있습니다.
```sh
sudo eopkg install yarn
```

### 경로 설정

{% include_relative _installations/unix_path_setup.md %}
