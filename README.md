tLab × GKE CI/CD Pipeline Sample

このリポジトリは、GitLab CI/CD を使用して Google Kubernetes Engine (GKE) に自動デプロイする構成例です。

## 📌 できること

- GitLab上の `.gitlab-ci.yml` による自動デプロイ
- GCPのサービスアカウント・認証設定
- `kubectl apply` によるマニフェスト反映
- GKE LoadBalancer型Serviceによる外部公開

## 📁 ディレクトリ構成


├── .gitlab-ci.yml # GitLab CI定義\n
├── k8s/\n
│ ├── deployment.yaml # nginx Deployment\n
│ └── service.yaml # LoadBalancer Service\n


## 🔐 注意

このリポジトリには機密情報（kubeconfigやGCPキー）は含まれていません。
実際に動かす際は GitLab の CI/CD Variables にて File型 / Variable型で登録してください。

## 🔄 今後の展望

- Helm 対応への拡張
- Argo CD を用いた GitOps 化
- Terraform によるインフラのIaC化

## 🪪 ライセンス

本リポジトリは MIT ライセンスで公開されています。

## 📝 詳細な構築手順

👉 Qiita記事にて詳細解説中：[GitLab × GKEでCI/CD構築する方法](https://qiita.com/Elie1729/items/ad527d8617ac95bab751)
