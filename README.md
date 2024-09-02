# モノレポの例

[情報科学若手の会第 57 回](https://wakate.org/2024/08/13/57th-general/) で発表するための例として作ったものです．

発表資料: [https://github.com/Stealthmate/wakate](https://github.com/Stealthmate/wakate)

## このレポの見方

情報科学若手の会新規サービス W を作っていると想像してみてください．

サービス W を運営するには API やフロントエンド，インフラの定義などいろんな要素が必要ですね．それらすべてがこのレポの中で定義されるような構成になっています．具体的には

1. [`packages/api`](./packages/api) - サービス W を提供する上で必要なバックエンド． Rust で書かれています．
2. [`packages/web`](./packages/web) - サービス W のユーザーが利用するフロントエンド． Nuxt を使って開発されています．
3. [`packages/kubernetes`](./packages/kubernetes) - サービス W を Kubernetes 上にデプロイするための manifest．
4. [`packages/infra`](./packages/infra) - サービス W をデプロイするための Kubernetes クラスタや DB などの要素を Terraform で定義したもの．
