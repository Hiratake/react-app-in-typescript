# React Starter Kit in TypeScript

[TypeScript](https://www.typescriptlang.org/) と [React](https://ja.reactjs.org/) の学習用リポジトリ

- [ハンズオンで学ぶ TypeScript - JavaScript エンジニアのための TypeScript徹底入門](https://www.udemy.com/course/ts-for-js-developers/)

## Node のインストール方法

本アプリケーションは [Node.js](https://nodejs.org/) を前提としています。macOS の場合だと以下の手順で導入できます。Node のバージョンは`.node-version`を参照し、同じものを使用してください。

    $ wget -P /tmp https://nodejs.org/download/release/v12.14.1/node-v12.14.1.pkg
    $ sudo installer -pkg /tmp/node-v12.14.1.pkg -target /
    installer: Package name is Node.js
    installer: Upgrading at base path /
    installer: The upgrade was successful.
    $ node -v
    v12.14.1

## アプリケーションの起動方法(Dockerを使用しない場合)

本プロジェクトは、[create-react-app](https://reactjs.org/docs/create-a-new-react-app.html) により作成したアプリケーションから React の学習に最低限必要な機能のみを厳選し、軽量化したものです。
以下の手順でアプリケーションを起動できます。

    $ wget https://github.com/DiveIntoHacking/react-starter-kit-in-typescript-with-node-v12.14.1/archive/v1.5.tar.gz
    $ tar zxvf v1.5.tar.gz
    $ cd react-starter-kit-in-typescript-with-node-v12.14.1-1.2
    $ yarn install
    $ yarn start

## アプリケーションの起動方法(Dockerを使用する場合)

    $ wget https://github.com/DiveIntoHacking/react-starter-kit-in-typescript-with-node-v12.14.1/archive/v1.5.tar.gz
    $ tar zxvf v1.5.tar.gz
    $ cd react-starter-kit-in-typescript-with-node-v12.14.1-1.1
    $ touch .bash_history
    $ docker-compose build
    $ docker-compose run --rm app yarn install
    $ docker-compose up
