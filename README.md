# CloudWatchAdditionalAlarmsForCloudTrail

[AWS が提供してくれているテンプレート](https://docs.aws.amazon.com/ja_jp/awscloudtrail/latest/userguide/use-cloudformation-template-to-create-cloudwatch-alarms.html)を基に、追加で監視したいメトリクスとアラーム、SNSトピックへの通知を同様に CloudFormation テンプレートで定義している。

以下の行為を CloudTrail のログで監視し、違反があればメール通知する:
- MFAを有効化せずにコンソールにログインする行為
- ルートアカウントを利用した任意の行為
