# 365music

## 🌐 App URL

### **http://52.196.17.34/**
![readme-top](https://user-images.githubusercontent.com/84176168/131131476-0c63c84c-ca21-4a0f-8c5a-0a69643c2813.png)

## サイト概要
聞いた楽曲の感想や、行ったライブ・フェスの感想など音楽にまつわることを自由に呟けるSNSサイト。
ユーザー同士フォロー機能でつながることができ、同じ趣味のユーザーを探し交流することができます。
またカレンダー機能もあり、自分の音楽ライフスケジュール（ライブ・フェスなどの予定）を管理できます。

### サイトテーマ
音楽好きの集う、音楽に特化したSNS

### テーマを選んだ理由
音楽は日常で自然と耳にするものです。
嬉しかった時や勇気づけられた時、落ち込んでしまった時。特になんでもない普通の日。どんな時でも音楽は聞かれるものです。
そんな身近な存在である音楽とSNSを融合させて、「この音楽を聞いていた時こんな気持ちだった」や「このライブに行ってこんなことを感じた」など、
日常プラス音楽に関わるちょっとした呟きができる気軽な場があれば、
音楽に対する感想や考えを共有することで音楽好きの輪を広げられるのではないかと思い、このテーマにしました。
またライブなどのスケジュール管理もできる機能がついていれば、より便利かなと考えました。

### ターゲットユーザー
年齢問わず、音楽が好きな方すべてが対象ユーザーとなります。

### 主な利用シーン
好きなアーティストの新曲を聞いた後に「とにかく感想を書きたい！」と思った時や、
ライブ・フェスに行った後に「この感情をどこかにぶつけたい！」と思った時に利用していただきたいです。
また自分はこう思ったけど、他の人はどんなことをこの音楽から感じたんだろうと思った際に使用していただきたいです。

## 設計書
- 画面遷移図
![365music_画面遷移図](https://user-images.githubusercontent.com/84176168/131148542-d4000450-9393-4117-b793-96bc7618ad52.jpg)
- ER図
![365music_ER](https://user-images.githubusercontent.com/84176168/131140203-04bad33d-2476-4e60-b70a-c30b3e9e4772.jpg)
- アプリケーション詳細設計
![PF_365music_アプリケーション詳細設計](https://user-images.githubusercontent.com/84176168/131137786-fec7d8a4-6575-42ab-ad13-16b796e6fbe0.jpg)
- テーブル定義書
https://docs.google.com/spreadsheets/d/10bgqbl-mJ0v9IErz8Or6WT0r02H-692C4Relbp5oZnM/edit?usp=sharing

## チャレンジ要素一覧
https://docs.google.com/spreadsheets/d/13xkINjyrOy5WzcaNKxclcb0LEL1ItdBBcmNCpK8X95I/edit?usp=sharing

## 機能一覧
- ユーザー機能・ログイン機能（devise）
- 投稿機能
    - 画像投稿（refile）
- いいね機能（Ajax）
- コメント機能（Ajax）
- フォロー機能
- ダイレクトメッセージ機能
- カレンダー機能（FullCalendar）
- 検索機能
- お問い合わせ機能
- ページネーション機能（kaminari）

## 動作デモ
- topページ  
![365music_top](https://user-images.githubusercontent.com/84176168/131208073-698cafe0-f811-4cea-abc5-4ba1aa57427a.gif)
- ゲストログイン  
![365music_guestbtn](https://user-images.githubusercontent.com/84176168/131211526-9052842f-377a-447e-afcd-def25d42586d.gif)
- いいね機能・コメント機能の非同期通信化  
![365music_like](https://user-images.githubusercontent.com/84176168/131499652-f6222cbe-77f2-489d-95a3-262c9f12d5b6.gif)
- カレンダー機能（FullCalendar）  
![365music_カレンダー](https://user-images.githubusercontent.com/84176168/131500426-4e20a1c8-835a-496a-aebb-15e442dbdd5e.gif)
- フォームの追加・削除（Coccon）  
![365music_cocoonフォーム](https://user-images.githubusercontent.com/84176168/131500987-3a257fbd-8b71-4fad-913e-c3a64b82e92e.gif)
- 検索機能  
![365music_検索機能](https://user-images.githubusercontent.com/84176168/131219900-b68abed6-2d2e-47c5-bc71-e26f4a4d7694.gif)
- ハッシュタグ検索  
![365music_ハッシュタグ検索](https://user-images.githubusercontent.com/84176168/131222414-d101b4e2-b8ce-4ca4-9deb-2288bbd9862b.gif)

## 開発環境
- OS：Linux(CentOS)
- 言語：HTML,CSS,JavaScript,Ruby,SQL
- フレームワーク：Ruby on Rails
- JSライブラリ：jQuery
- IDE：Cloud9

## 使用技術
- Ruby 2.6.3
- Ruby on Rails 5.2.5
- MySQL
- AWS
    - VPC
    - EC2
    - RDS
- Nginx
- Puma
- RSpec

## 構築方法
```
$ git clone https://github.com/ishr-sk/365music.git
$ cd 365music
$ bundle install
$ rails db:migrate
$ rails db:seed
$ rails s
```

## 使用素材
- 無料写真素材：[Pexels](https://www.pexels.com/ja-jp/)
- イラスト：[Loose Drawing](https://loosedrawing.com/)
- ロゴメーカー：[Hatchful](https://hatchful.shopify.com/ja/)
