# Golf x Dorone

# ⛳️ Projects

ドローン撮影の免許を取得した友人から、ドローンを使って撮影した映像や画像を紹介する独自のアプリケーションを作って欲しいという依頼がありました。そこでドローンで撮影した映像を魅力的に紹介できるアプリケーションを作成することにしました。まずは最低限の機能でリリースし、ビジネス設計をしながら必要な機能を順次開発していきます。
まだビジネス設計が固まっていない中でのシステム開発なので、拡張がしやすい設計にすることを意識しています。

目標はドローンで撮影したゴルフ場の画像や映像を紹介するサービスとしてリリースすることです。普段撮影している地上からの画像では得られない臨場感ある画像や映像を魅力的に紹介するサービスにしたいと考えています。
機能面ではゴルフ場の経営者の方がドローン撮影の依頼をしたり、撮影以外にも動画制作、SNS 企画などの幅広い仕事を一般の方が依頼できるようなもの（お問い合わせ機能）が必要になります。※番組制作経験のある友人が仕事を受け付けるため
またゴルフプレイヤーに向けてゴルフ場（ラウンド）の情報やゴルフが得意な友人がゴルフに関する情報を発信するプラットフォームサイト的な役割を果たすサービスとして展開していく予定です。

# 🖋Purpose

システム設計や環境構築からデプロイまで、システム開発における一連の流れを習得したいと思い、着手しました。業務で使用したことのある React と、スクールでの学習経験しかない Rails（API モード）を使用し、SPA を作成したいと思いました。
また AWS の認定資格取得をきっかけにインフラ構築への関心が高まり、AWS サービスを使用し最低限の設定と運用管理で、簡単にデプロイできる方法を実際に試してみたいと思いました。

# 🔧Features(MVP)

| ページ   | 機能                         | 対応状況 |
| :------- | :--------------------------- | :------- |
| Customer | ブログ閲覧                   | 対応済み |
| Customer | お問合せ機能                 | 対応済み |
| Customer | TOP ページ映像紹介           | 未着手   |
| Customer | 映像アーカイブ               | 未着手   |
| Customer | その他ビジネス紹介ページ     | 実装中   |
| Admin    | ブログ作成/更新/削除機能     | 対応済み |
| Admin    | お問合せ閲覧                 | 対応済み |
| Admin    | 画像/映像アップロード機能    | 実装中   |
| Admin    | メール認証                   | 未着手   |
| Admin    | パスワード再設定機能         | 未着手   |
| Admin    | ユーザープロフィール編集機能 | 未着手   |

# 💡Solution

- ゴルフ場をお探しの方/ゴルフプレイヤーの方：ゴルフ場の様子を空撮映像で確認することができます。
- ゴルフ場経営者の方: ドローンの撮影代行を行います。

# 🌐 URL

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

![infra](profile/statics/infra_image.png)
