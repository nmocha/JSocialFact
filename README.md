# JSocialFact: 日本語社会性バイアスQAデータセット ver.1
repository for the  (JSocialFact).

本データセット(JSocialFact ver.1)は***データセットとなります。

## データセットの概要
JBBQはAge, Disability status, Gender identity, Physical appearance, Sexual orientationの計5つの社会的カテゴリに関する多岐選択式のQAデータセットです。

各カテゴリのテンプレートは、カテゴリに関する言及を含み曖昧性のある文脈、曖昧性を解消させる文脈、語彙、文脈に関してカテゴリに属するグループや人物に有害な偏見を引き起こす問題文（カテゴリに否定的な問題文）、中立的な問題文、回答選択肢（カテゴリに属するラベル、カテゴリに属さないラベル、曖昧性のある文脈のみからは答えが定まらないunknownラベルの3値）、テンプレート作成に参照したソースの情報、から主に構成されています。 テンプレートは全カテゴリで計245件（Age: 72件，Disability: 52件，Gender: 41件，Physical: 52件，Sexual: 28件）あり、テンプレートに語彙を代入して生成された問題数は計50,856件（Age: 28,176件, Disability: 8,064件, Gender: 3,912件, Physical: 7,536件, Sexual: 3,168件）あります。

## データフォーマット
データフォーマットはBBQのデータフォーマットに準拠しています。

question_polarity: 対象とするカテゴリに対する否定的な問題（neg）か中立的な問題（nonneg）か
context_condition: 文脈が曖昧のあるもの（ambig）か曖昧性を解消するもの（disambig）か
answer_info : 質問に対する選択肢の属性の情報
additional_metadeta: 対象とするカテゴリに関する情報と根拠となるURL
context: 文脈文
question: 質問文
ans0, ans1, ans2 : 質問に対する選択肢
label: 質問の正解
is_additional: 1であれば，JBBQで追加したテンプレート
英語のBBQデータセットの詳細は、以下の論文とリポジトリをご参照ください。

BBQ: A hand-built bias benchmark for question answering Alicia Parrish, Angelica Chen, Nikita Nangia, Vishakh Padmakumar, Jason Phang, Jana Thompson, Phu Mon Htut, Samuel Bowman github

## ご利用上の注意
データセットの利用をご希望の方はこちらのフォームに必要事項をご記入ください。データセットへのリンクをお送りします。この方法以外でのデータの再配布は禁止します。 本データセットはその性質上不適切な表現を含みます。承諾の上、LLMの安全性・公平性向上のためにご利用ください。 本データセットの利用においては、以下の参考文献をご参照ください。

## 参考文献
@article{}
## 免責事項
本データセットの制作者は、利用者が利用者自身又は第三者に与えた損害について、一切の責任を負わないものとする。また、本データセットのサービス提供の遅延、中断又は停止により利用者又は第三者が被った損害について、制作者は一切の責任を負わないものとする。制作者は、予告なしに、本データセットの運営を停止もしくは中止し、又は本データに掲載される情報の全部若しくは一部を変更する場合がある。

## License
This work is licensed under a Creative Commons Attribution 4.0 International License.
