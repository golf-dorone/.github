# Golf x Dorone ⛳️ 
### プロジェクト概要
ドローンで撮影したゴルフ場の画像や映像を紹介するサービスです。普段撮影している地上からの画像では得られない臨場感ある画像や映像を掲載します。全国のゴルフ場を対象に、ドローンの空撮事業を展開することが目標です。またゴルフプレイヤー達がラウンドの詳細を空からの画像や映像で把握することができるプラットフォームになることも目標としています。

### 登場人物
- ゴルフ場経営者
- ゴルフプレイヤー

### ユーザーが抱える課題
- (ゴルフ場経営者)：地上からの画像や映像ではゴルフ場の全体の様子を伝えきれていない
- (ゴルフプレイヤー)：ゴルフ場紹介サイトでは地上からの写真が多く、全体像が把握しにくい

### 解決方法＆今後の展望
- ゴルフ場経営者に向けてドローン撮影代行事業を展開する
- 撮影したドローン映像を掲載し、ゴルフ場の情報を発信する
- ゴルフ場の各ホールごとの特徴や詳細を上空からの映像と詳細コメント付きで紹介する(プレイヤー視点で)

### サービスを作った背景
ドローン撮影の免許を取得した友人が、ドローンを使って撮影した映像や画像を紹介する独自のサービスを作りたいという依頼がありました。そこでドローンで撮影した映像を魅力的に紹介できるアプリケーションを作成することにしました。また番組制作経験のある友人がドローン撮影事業以外にも仕事を受け付けられるようなお問合せ機能も作成しました。
まずは最低限の機能でリリースし、友人とビジネス設計をしながら必要な機能を順次開発していきます。

### 現在の機能
| ページ | 機能 | 対応状況 |
| :--- | :--- | :--- |
| Customer | ブログ閲覧 | 対応済み |
| Customer | お問合せ機能 | 対応済み |
| Admin | ブログ作成/更新/削除機能 | 対応済み |
| Admin | お問合せ閲覧 | 対応済み |

### 今後実装予定の機能
| ページ | 機能 | 対応状況 |
| :--- | :--- | :--- |
| Customer | TOPページ映像紹介 | 未着手 |
| Customer | 映像アーカイブ | 未着手 |
| Customer | その他ビジネス紹介ページ | 実装中 |
| Admin | 画像/映像アップロード機能 | 実装中 |
| Admin | メール認証 | 未着手 |
| Admin | パスワード再設定機能 | 未着手 |
| Admin | ユーザープロフィール編集機能 | 未着手 |

- Customer: 通常ユーザーが閲覧するpublicなページです。
- Admin: 管理者のみがアクセスし、投稿等を行うページです。

### 🌐 URL

- 本番環境：
```
customer(public)
https://web.golf-dorone.com/customer
```

```
admin(private)
https://web.golf-dorone.com/auth/signin
```

- ローカル環境セットアップ方法

```
FE:
git clone git@github.com:golf-dorone/golf_web.git
yarn install
yarn start

BE:
git clone git@github.com:golf-dorone/golf_api.git
bundle install
rails db:migrate
rais s
```

### 📚Environment & Skill

- フロントエンド：

```
React：18.1.0
Apollo Client
GraphQL Code Generator
TypeScript
Chakra-ui
```

- バックエンド：

```
Ruby：2.7.4
Ruby on Rails：6.1.4
Graphql
Graphiql
```

- インフラ

```
Route53
CloudFront
RDS
ECS(Fargate)
```

<img width="619" alt="スクリーンショット 2022-10-18 10 57 37" src="https://user-images.githubusercontent.com/69895997/196317805-51524ee1-46f6-44f2-8e47-ba74c22ddd69.png">



- ER図
<img width="796" alt="スクリーンショット 2022-10-18 10 54 08" src="https://user-images.githubusercontent.com/69895997/196317124-62f7a6fa-9ec7-48e9-a3b7-b13e0ef4d0c3.png">

