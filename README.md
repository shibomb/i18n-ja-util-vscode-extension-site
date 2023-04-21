# i18n ja util

翻訳作業ユーティリティです。

ご利用前に必ず [LICENSE](LICENSE.md) を読んで同意ください。

## **Feature: Grammarly**

選択した英語などの文章を対象に、OpenAI API を利用した日本語校正を行います。

- コマンドで起動:
  エディタ上で英語などの文章を選択中に `F1`, `Grammaryly` でコマンドが実行されます。
- ショートカットで起動:
  エディタ上で英語などの文章を選択中に  
  Win: `shift + win + f1` / Mac: `shift + cmd + f1`

## **Feature: Kana Readable**

文章中の読みにくい漢字をひらがなに変換します。

- コマンドで起動:
  エディタ上で文章を選択中に `F1`, `KanaReadable` でコマンドが実行されます。
- ショートカットで起動:
  エディタ上で文章を選択中に  
   Win: `shift + win + f2` / Mac: `shift + cmd + f2`

---

## Requirements

Grammarly 機能を使うためには、この拡張機能の設定に OpeanAI API Key を設定する必要があります。

## Extension Settings

- `i18n-ja-util.openai_apikey` :

  YOUR_API_KEY from https://platform.openai.com/account/api-keys

- `i18n-ja-util.openai_model` :

  OpenAI model. see https://platform.openai.com/docs/models/overview

  default: \"gpt-3.5-turbo\"

- `i18n-ja-util.prompt_prefix` :

  Prompt prefix.

  default:

```
下記の文章を「ですます調」の読みやすい日本語に校正してください。文章がjsonの場合、jsonの形を保持してください。htmlタグがあった場合はhtmlタグ部分は原文のままにしてください。NumberやStringなどのデータ型と思わしき部分は日本語にしないでください。説明は不要ですので結果だけを示してください。以下が対象の文章です:
\`\`\`
```

- `i18n-ja-util.prompt_suffix` :

  Prompt suffix.

  default:

```
\n\`\`\`
```

## Release Notes

see [CHANGELOG.md](CHANGELOG.md)

---

**Enjoy Internationalization!**

Copyright (c) 2023 shibomb. All rights reserved.
