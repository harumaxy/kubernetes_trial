# Kubernetes
を練習するためのリポジトリ

# Note

# kubectl run

即興で、ネットワークを確認するためのPodを立ち上げるのに便利なコマンド

```bash
kubectl run <pod名> --restart=Never --image=centos:6 --rm -it 
```

`docker run` と似たような感じ

# Cloud Code

Google公式の、Kubernetes用のVSCode拡張
多数の実戦投入可能なスニペットが使える

[Kubernetes YAML を使う  |  Cloud Code for VS Code  |  Google Cloud](https://cloud.google.com/code/docs/vscode/yaml-editing?hl=ja)

## 使い方
1. cmd + shift + P
2. Cloud Code : Apply current json/yaml kubernetes deployed resorces
現在開いているyamlファイルで、Kubernetes Resorcesのコードスニペットが有効になる

## 機能
- スニペット/テンプレート
- コンテキストによる補完
- 現在のスキーマから、正しいオプションを提示する
- カーソルを置くとドキュメント表示
- 定義に移動
- 現在、クラスタにデプロイされているリソースと、マニフェストファイルの差分を表示
- シークレットの利用
- Secret リソースに`data:` フィールドのbase64文字列を入力して、カーソルを合わせるとデコードした文字が出る
- 確認に便利