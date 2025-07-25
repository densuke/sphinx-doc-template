# 基本ルール

- 使用する言語は日本語とし、コメント類はすべて日本語ベースで出力すること。
- プルリクエストにおいても、レビューでは日本語を使用すること。うっかり英文で書いてしまった場合は、日本語訳版もレビューに追加すること。
- コードにコメントを含めるときも、必ず日本語ベースで行うこと。
  - ただし、シンボルの類いは英語ベースで行い、変数の命名ルール(キャメルケースやスネークケース)はその言語の標準(もしくはデファクトスタンダード)に従うこと
  - ループ変数など、一時的に使うインデックス値はi,j,kなど単純なアルファベットの利用も許容する
  - bashなどシェルの操作の際に使うプロンプト($や%、###など)とPowerShell(`PS>`と暫定的に設定)は気にしないでください。
- 英数字・記号は原則として半角のものを使い、全角は使ってはならない。ただし例外は存在します
  - 数字の桁区切りに使うカンマ(,)は半角であればOK、全角はもちろん禁止
  - 日本語における記号(かぎかっこや句読点、中点)は全角のものを使用する
    - 「」『』【】。、・など日本語の文章で使う記号は全角で良い
    - 半角の存在する、いわゆるパーレン(括弧)や[...]、{...}は半角を使う
  - チルダ(〜)は伸ばし記号として使うことがあるため、半角でも全角でも特に気にしなくてよい
  - それ以外の『全角と半角で共通して存在する記号』は全て半角を使用する
    - 例: `! " # $ % & ' ( ) * + , - . / : ; < = > ? @ [ \ ] ^ _ { | }` およびバッククォート記号
  - 英数字は全て半角とする、全角は赦さない
  - 当然だが全角の空白(スペース)はこの世に存在してはいけない

## Markdownのルール

- myst-parserによるMarkdownを使用すること。
- Markdownの記法は、GitHub Flavored Markdownを基本とする。
- コードブロックは、言語名を指定してシンタックスハイライトを有効にすること。
- Mermaidは {mermaid} タグを使用して記述すること(後述の例参照)。

## Mermaidのサンプル

**インチキ**関西弁によるサンプル

```{mermaid}
flowchart TD
    A[はじまりやで] --> B{ほんまにええんか？}
    B -- せやで --> C[やってまうで]
    B -- ちゃうわ --> D[やめとくわ]
    C --> E[おしまいや]
    D --> E
```
