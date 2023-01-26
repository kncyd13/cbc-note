## 参考 8：レピュテーションとポリシールール、Dynamic Rules Engine

レピュテーションとポリシーのルールが競合した場合、ポリシーの\[許可\]ルールにファイルやフォルダのパスが登録されているのであれば、その\[許可\]ルールが、他のすべてのルールおよびレピュテーションよりも優先されます。

参考資料：
- Endpoint Standard: How do Reputations Interact With Policy rules?  
  https://community.carbonblack.com/t5/Knowledge-Base/Endpoint-Standard-How-do-Reputations-Interact-With-Policy-rules/ta-p/82453

また、CBCはポリシーによる防御ルール以外に、Dynamic Rules Engineと呼ばれる脅威解析ユニット(TAU)が配信する防御ルールが適用されています。ポリシーによる影響を受けないため、仮にMonitoredポリシーが適用されているCBセンサーであってもDynamic Rules Engineは動作しています。そのため、Monitoredポリシーを設定しているにもかかわらず、Dynamic Rules Engineによって脅威検知が発生して、プロセスの実行がブロックされる可能性があることにご注意ください。
