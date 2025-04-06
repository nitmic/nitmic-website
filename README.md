# NITMic 公式 Web サイト

![workflow](https://github.com/nitmic/nitmic.club.nitech.ac.jp/actions/workflows/build.yml/badge.svg)
![workflow](https://github.com/nitmic/nitmic.club.nitech.ac.jp/actions/workflows/deploy.yml/badge.svg)
![workflow](https://github.com/nitmic/nitmic.club.nitech.ac.jp/actions/workflows/disk_space_alert.yml/badge.svg)

URL：http://nitmic.club.nitech.ac.jp/

## Overview

- **名古屋工業大学コンピュータ俱楽部 NITMic** の公式 Web サイト開発リポジトリです
- 静的サイトジェネレーター [Hugo](https://github.com/gohugoio/hugo) を利用しています
  - 使用テーマ：[Mainroad](https://github.com/Vimux/Mainroad)
- ホスティングは課外活動用ウェブサイトホスティングサービスを利用しています
  - 詳細：[国立大学法人名古屋工業大学 情報基盤センター](https://www.cc.nitech.ac.jp/service/students/web-hosting-club.html)（学内のみからアクセス）

## Usage

### このリポジトリをローカルに clone する

下記のコマンドを実行することでこのリポジトリをローカルに clone することができます：

```
$ git clone git@github.com:nitmic/nitmic.club.nitech.ac.jp.git
```

### Dev Containers で開く

本リポジトリでは、[Visual Studio Code Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers) を用いた開発環境の構築を推奨しています。
Dev Containers を利用することで、Hugo や Go ランタイムなどの必要なツールを自動でセットアップでき、すべての開発者が一貫した環境で作業を行うことが可能になります。

VS Code に [Dev Containers 拡張機能](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) をインストールした状態でリポジトリを開くと、「Reopen in Container（コンテナで再オープン）」という通知が表示されます。
このボタンをクリックすることで、Dev Containers 環境が起動し、すぐに開発を始めることができます。

通知が表示されない場合は、コマンドパレット（`F1` または `Ctrl+Shift+P`）を開き、「Dev Containers: Reopen in Container」を選択してください。

### ローカルでプレビューする

以下のコマンドを実行すると、Hugo によるローカルサーバーが立ち上がり、サイトのプレビューを確認できます：

```
vscode ➜ /workspaces/nitmic.club.nitech.ac.jp (main) $ hugo server
```

実行後、以下のようなログが表示されます：

```
hugo: collected modules in 1239 ms
Watching for changes in /workspaces/nitmic.club.nitech.ac.jp/{archetypes,assets,content,data,layouts,static}
Watching for config changes in /workspaces/nitmic.club.nitech.ac.jp/config.toml
Start building sites …
hugo v0.115.4-dc9524521270f81d1c038ebbb200f0cfa3427cc5 linux/amd64 BuildDate=2023-07-20T06:49:57Z VendorInfo=gohugoio


                   | EN
-------------------+------
  Pages            | 163
  Paginator pages  |   9
  Non-page files   |   0
  Static files     | 206
  Processed images |   0
  Aliases          |  66
  Sitemaps         |   1
  Cleaned          |   0

Built in 5244 ms
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

お使いのブラウザで http://localhost:1313/ にアクセスすると、ローカル環境でサイトのプレビューが表示されます。
編集内容は保存するたびに自動で反映されるため、リアルタイムに確認しながら作業が可能です。
