# つくつくフロント側技術選定

フロントエンド側の技術選定や実装ルールを決める

## 利用技術

- ライブラリ
  - React
- フレームワーク
  - Next.js
- UIコンポーネント
  - material-ui
- 状態管理
  - Redux
- GraphQLクライアント
  - apollo
- Linter
  - ESLint
- UI開発環境
  - Storybook
- 実装志向
  - [Atomic Design](https://qiita.com/yoshimo123/items/302fb3f1698a8db3cf23)

## 実装ルール

[React Componentの実装ルールを決めてみた](https://moneyforward.com/engineers_blog/2020/02/18/react-component-rules/)から拝借🙏適宜付け足していきましょう！

- Atomic Designを意識する
  - 各レベルのルール
  - 自分のレベル以下の要素で構成する
  - 最初から完璧に設計する必要はない
- ファイルの命名規則
- Functional Componentで実装する
- Container ComponentとPresentational Componentに分けて実装する
- Templates以下のComponentではuseQuery・useMutationを実行しない
- global state と local stateの使い分け
- スタイル管理
- その他
  - export defaultを使用しない
  - Componentを作成する際はclassNameを受け取ることが可能なようにpropsを定義する
  - Material-UIを利用する
- Componentの利用
  - RailsのViewへのReact Componentの埋め込み
  - client/Components/other/以下のComponentは原則利用しない

## ブランチルール

- masterへの直コミット禁止
- 必ずPRを作成してマージ
- 作業ブランチ命名規則（暫定・理想はissueに紐付けたい）
  - feature/{your_name}_{work_name}
