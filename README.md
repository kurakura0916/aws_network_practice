# AWS CloudFormation
[Amazon Web Services 基礎からのネットワーク＆サーバー構築](https://www.amazon.co.jp/dp/B06Y5ZSYY4/ref=dp-kindle-redirect?_encoding=UTF8&btkr=1)の内容をAWS CloudFormationを使って構築する。

# aws cliを使った実行方法

- スタックの作成
```
aws cloudformation create-stack --stack-name aws-network-basic --template-body file://$PWD/chap02/template.yml --profile my-profile
```

- スタックの削除
```
aws cloudformation delete-stack --stack-name aws-network-basic --profile my-profile

```
必ずスタックは削除するようにする。（EC2のインスタンス等で課金されます）