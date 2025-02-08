# NITMic 公式 Web サイト

![workflow](https://github.com/nitmic/nitmic-website/actions/workflows/build.yml/badge.svg)
![workflow](https://github.com/nitmic/nitmic-website/actions/workflows/deploy.yml/badge.svg)
![workflow](https://github.com/nitmic/nitmic-website/actions/workflows/disk_space_alert.yml/badge.svg)

URL：http://nitmic.club.nitech.ac.jp/

## Overview

- **名古屋工業大学コンピュータ俱楽部 NITMic** の公式 Web サイト開発リポジトリです
- 静的サイトジェネレーター [Hugo](https://github.com/gohugoio/hugo) を利用しています
  - 使用テーマ：[Mainroad](https://github.com/Vimux/Mainroad)
- ホスティングは課外活動用ウェブサイトホスティングサービスを利用しています
  - 詳細：[国立大学法人名古屋工業大学 情報基盤センター](https://www.cc.nitech.ac.jp/service/students/web-hosting-club.html)（学内のみからアクセス）

## Usage

- 詳しい利用法や運用方法は [Wiki](https://github.com/nitmic/nitmic-website/wiki) をご参照ください

### このリポジトリをローカルに clone する

下記のコマンドを実行することでこのリポジトリをローカルに clone することができます

```
$ git clone git@github.com:nitmic/nitmic-website.git
```

### ローカルでプレビューする

静的サイトジェネレーター [Hugo](https://github.com/gohugoio/hugo) と [GO](https://go.dev/) をインストールし、下記のコマンドを実行することでローカルでプレビューすることができます

```
$ hugo server
Watching for changes in /workspaces/nitmic-website/{archetypes,assets,content,data,layouts,static}
Watching for config changes in /workspaces/nitmic-website/config.toml
Start building sites …
hugo v0.115.4-dc9524521270f81d1c038ebbb200f0cfa3427cc5 linux/amd64 BuildDate=2023-07-20T06:49:57Z VendorInfo=gohugoio


                   | EN
-------------------+------
  Pages            | 145
  Paginator pages  |   5
  Non-page files   |   0
  Static files     | 182
  Processed images |   0
  Aliases          |  60
  Sitemaps         |   1
  Cleaned          |   0

Built in 2611 ms
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

お使いのブラウザで http://localhost:1313/ にアクセス
