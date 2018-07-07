* parity install

parity는 직접 설치해야함

```
$ sudo apt-get update
$ sudo apt-get install openssl libssl-dev libudev-dev
$ sudo apt-get install cargo
$ sudo apt-get install git
$ sudo apt-get install curl
$ sudo apt-get install build-essential
$ sudo apt-get dist-upgrade -y
$ sudo apt-get install pkg-config
$ git clone https://github.com/paritytech/parity
$ curl -sSf https://static.rust-lang.org/rustup.sh | sh
$ bash <(curl https://get.parity.io -L) -r stable
$ parity --help
```

* geth install

geth는 [설치 페이지](https://geth.ethereum.org/downloads/)에서 운영체제에 맞춰서 설치가능.

직접 빌드시 아래를 따름. 직접 빌드할 경우 코드수정 후 설치가능.

```
$ apt-get update
$ apt-get install -y build-essential libgmp3-dev golang-1.9 golang-1.9-doc git
$ git clone https://github.com/ethereum/go-ethereum.git
$ cd go-ethereum
$ sudo ln /usr/lib/go-1.9/bin/go /usr/bin/go # golang 경로설저
$ git checkout refs/tags/v1.7.3
$ make geth
$ sudo cp build/bin/geth /usr/local/bin/
```
