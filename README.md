# parcel-wasm-skeleton
WebAssemblyの素振り環境.

## Requirements
Rust 及び `wasm32-unknown-unknown` ターゲットを有効化する必要があります.

```bash
# Rust のインストール
# ref: https://www.rust-lang.org/ja-JP/install.html
$ curl https://sh.rustup.rs -sSf | sh
$ export PATH="$HOME/.cargo/bin:$PATH"
$ rustc --version


## nightlyの有効化
$ rustup install nightly
$ rustup default nightly
$ rustc --version


# `wasm32-unknown-unknown` ターゲットの有効化
# ref: https://www.hellorust.com/news/native-wasm-target.html
$ rustup update
$ rustup target add wasm32-unknown-unknown --toolchain nightly
```

## Usage
1. `mkdir new-project && cd $_`
1. `wget -O - https://github.com/mizdra/parcel-wasm-skeleton/archive/master.tar.gz | tar xzvf - --strip=1 --exclude LICENSE`
1. `npx npm-check-updates -a`
1. `yarn install --force`
1. `yarn run start`


## Option
- `license MIT > LICENSE`