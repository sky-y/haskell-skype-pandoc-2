## 内容

マークアップ形式のドキュメントを変換する、Haskell製のツール [Pandoc](https://pandoc.org/) に関する勉強会です。発表は、Pandocユーザーズガイド の日本語訳をなさっている [@sky\_y](https://twitter.com/sky_y) さんに行なっていただきます。

当該勉強会は、全2回の予定です。今回は、その第2回目です。

### 第2回の概要

PandocにはFilter機能というユーザ拡張機能があります。これにより「見出しレベルを変更する」など、より柔軟に文書の変換ができます。

第2回では「Pandocフィルタを実装する」という形で、Haskell初心者が入門できるチュートリアルを予定しています。

- 自己紹介
- Pandocとは（第1回の短いおさらい）
- PandocのFilterとは
- PandocのASTを知る
- Haskellの概要
- StackでHaskellのHelloWorldを書こう
- Pandoc FilterをHaskellで書こう

## 想定する参加者

### 必要なスキル

下記の知識を前提とします。

- コマンドラインの基本的な知識がある
- 何らかのプログラミング経験がある
    - 1つの言語以上を知っていればOKです
        - 例: JavaScript, Python, Ruby, C#, Swiftなど
    - Haskellや関数型言語の知識や経験は不要です！

### 参加をおすすめする方

- Haskellや関数型言語について、知らないけど興味がある方
    - 特に今回は、「Haskellはとっつきにくい、怖い」と思われる方に向けてチュートリアルを進めます
- ドキュメントの変換に興味がある方
    - Pandocについて知っている（または前回のチュートリアルに参加した）が、さらにPandocを活用したいと思われる方
    - 日常的にドキュメントを変数する仕事やタスクを行っている方

## 事前準備（任意・推奨）

以下の作業を行っておくと、チュートリアルがよりスムーズに進行できると思います。
可能な方は、事前に行っておくことをおすすめします。

（発表後に「もくもく会」として時間を取るので、必須ではありません。）

- Pandoc本体のインストール
    - [第1回資料](https://github.com/sky-y/haskell-skype-pandoc-1/blob/master/index_github.md) の「準備: Pandocをインストールする」を参考にしてください
- Stack（Haskellソースをコンパイルするためのビルドツール）
    - 2017年現在では、HaskellのソースコードはStackを用いてコンパイルすることが標準となっています
    - インストール方法
        - Windows
            - [GitHubのダウンロードページ](https://github.com/commercialhaskell/stack/releases/latest)を開く
            - `stack-1.3.2-windows-x86_64-installer.exe` をダウンロードしてインストール
        - Mac(Homebrew)
            - `$ brew install haskell-stack`
    - さらに時間に余裕のある方は、下記のページを参考にしてHelloWorldを書いてみてください:
        - [Stackでやる最速Haskell Hello world! (GHCのインストール付き！) - Qiita](http://qiita.com/igrep/items/da1d8df6d40eb001a561)
    - その他の詳細は [Stack公式チュートリアル](https://docs.haskellstack.org/en/stable/README/) をご覧ください

## 日時

-   日付: 2月17日（金）
-   時間: 22:00 ～ 23:30

#### タイムスケジュール

| 時間           | 内容                                             |
|----------------|--------------------------------------------------|
| 21:45 ～ 22:00 | 通信テストを開始                                 |
| 22:00 ～ 22:05 | 勉強会開始、挨拶                                 |
| 22:05 ～ 23:05 | 発表 ([@sky\_y](https://twitter.com/sky_y) さん) |
| 23:05 ～ 23:25 | 質問、もくもく会                                 |
| 23:25 ～ 23:30 | 次回の説明、終了                                 |

#### 注意

**参加受付日時は、X月XX日 (X) 21:00 まで** です。ご注意ください。

場所
----

Skype と Slack を用います。**Skype は必須**です。詳しい使用目的は、以下に記載しております。

ともに、Web ブラウザで利用することができます。Web ブラウザが落ちる可能性を考慮して、各々の専用アプリを利用することを個人的にはおすすめ致します（参加者の自由判断）。専用アプリを使用する方は、アプリをダウンロードして設定を行なっておいてください。

-   [Skype のアプリ](https://www.skype.com/ja/download-skype/)
-   [Slack のアプリ](https://slack.com/downloads/)

#### Skype

-   使用目的: 進行役の **画面共有**、および参加者の **音声共有**
-   URL: **開催日の前日 (2月16日) の20時頃に、connpassのアカウントとして登録しているメールアドレス宛** にメールを送信します。そこに、URL を記載しておきます。
-   参考URL: [参加者へ一括メッセージを送る](http://help.connpass.com/organizers/bulk-message)

#### Slack

-   使用目的: コード共有やURL共有などの、**文字情報の共有**
-   URL: [Googleフォーム](https://goo.gl/EzRKbs) にて必要事項を記入してくださると、[当該グループ](https://haskellwithskype.slack.com/)に参加できます。
-   上記 URL からグループに参加できない場合は、個別対応をいたしますので、[@lawtwai](https://twitter.com/lawtwai) にご連絡ください。

#### スライド

GitHub Pagesにてします。現在作成中ですが、当日も下記のアドレスにアップします。

- スライド(HTMLプレゼンテーション): <https://sky-y.github.io/haskell-skype-pandoc-2/>
- スライド(復習用): [haskell-skype-pandoc-2/index_github.md](https://github.com/sky-y/haskell-skype-pandoc-2/blob/master/index_github.md)
- GitHubリポジトリ全体: [sky-y/haskell-skype-pandoc-2](https://github.com/sky-y/haskell-skype-pandoc-2)

その他の注意事項
----------------

#### 人数制限について

-   Skype には、グループ音声通話の可能な人数に制限があります。**当日に参加できない方は、参加キャンセルの手続きを connpass で行なってください** 。
-   参考URL: [Skype で通話をする方法](https://support.skype.com/ja/faq/FA10613/skype-detong-hua-wosurufang-fa-wojiao-etekudasai)

#### Skype について

###### 音声入力

プライバシーの観点から、必要でなければミュートにしてください。

###### 画面共有

参加者の方が、ご自身の画面を共有することはないと思います。デスクトップの整理や部屋の片付けは、不要かと思います。

## その他

不明な点や質問がございましたら、[@lawtwai](https://twitter.com/lawtwai) にご連絡ください。
