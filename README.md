# lsを読むために落としてきたもの
https://amzn.asia/d/3f7vYgw

```sh
$ wget ftp://ftp.ring.gr.jp/pub/GNU/coreutils/coreutils-8.21.tar.xz
$ tar Jxf coreutils-8.21.tar.xz
```

## build/install
`~/${HOME}/coreutils-8.21`にインストールする感じでBuildする。

```sh
$ ./configure --prefix="${HOME}/coreutils-8.21"
$ make CFLAG="-g" # デバッグできる様にしておく
$ make install    # install する。
```

## 実行
```sh
$ ~/coreutils-8.21/bin/ls -l
```
