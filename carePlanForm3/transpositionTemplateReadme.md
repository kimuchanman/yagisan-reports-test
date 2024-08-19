まず、yagisan-reports の height 属性にテンプレート変数を使えない現状挙動により、転置しています。転置自体は国も許可しています。

曜日ごとに event のリストを流してやる必要があります。

event の内容としては、以下のようなものです。
実例の参考に [transpositionTemplateData.json](./transpositionTemplateData.json) をご覧ください。

```yaml
event:
  - x: 予定の開始時間（n時）*10.25 # 10.25は1時間の横幅です
    width: 予定の長さ（時間）*10.25
    content: 予定の内容。 \n で改行できます。
```
