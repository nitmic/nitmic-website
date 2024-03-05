# nitmic-hp

URL：http://nitmic.club.nitech.ac.jp/

## Overview

- **名古屋工業大学コンピュータ俱楽部NITMic** のホームページ開発リポジトリです
  
- 静的サイトジェネレーター[Hugo](https://github.com/gohugoio/hugo)を利用しています
  - 使用テーマ：[Mainroad](https://github.com/Vimux/Mainroad)
    
- ホスティングは課外活動用ウェブサイトホスティングサービスを利用しています
  - 詳細：[国立大学法人名古屋工業大学　情報基盤センター](https://www.cc.nitech.ac.jp/service/students/web-hosting-club.html)（学内のみからアクセス）

## Usage

- 詳しい利用法や運用方法は[Wiki](https://github.com/nitmic-git/nitmic-hp/wiki)をご参照ください


### このリポジトリをローカルにcloneする

[Hugo](https://github.com/gohugoio/hugo)の[テーマ](https://themes.gohugo.io/)を使用する為、サブモジュールもクローンする必要があります
```
# クローン
$ git clone git@github.com:nitmic-git/nitmic-hp.git

# サブモジュールをクローン（更新）
$ git submodule update --init --recursive
```

### ローカルでプレビューする
静的サイトジェネレーター[Hugo](https://github.com/gohugoio/hugo)をインストールし、下記のコマンドを実行することでローカルでプレビューすることができます
```
$ hugo server

# ログの例
Start building sites … 
hugo v0.89.4-AB01BA6E windows/amd64 BuildDate=2021-11-17T08:24:09Z VendorInfo=gohugoio
                   | EN
-------------------+------
  Pages            | 115
  Paginator pages  |   3
  Non-page files   |   0
  Static files     | 159
  Processed images |   0
  Aliases          |  47
  Sitemaps         |   1
  Cleaned          |   0

Built in 362 ms
Watching for changes in D:\repository\nitmic-hp\{archetypes,assets,content,data,layouts,static,themes}
Watching for config changes in D:\repository\nitmic-hp\config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```
お使いのブラウザで http://localhost:1313/ にアクセス
