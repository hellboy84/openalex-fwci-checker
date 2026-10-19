# OpenAlex FWCI チェッカー

機関を指定して、[OpenAlex](https://openalex.org/) が論文ごとに付けている FWCI（Field-Weighted Citation Impact）を集計し、機関の平均 FWCI が何に支えられているか（分野・出版年・少数の高被引用論文・大規模共著）を確認するツールです。

**▶ ツールを開く: https://hellboy84.github.io/openalex-fwci-checker/**

`index.html` 1 ファイルだけで動きます。ブラウザから OpenAlex API に直接問い合わせるため、サーバーやインストールは不要です。

## 使い方

1. https://hellboy84.github.io/openalex-fwci-checker/ を開く（`index.html` をダウンロードしてブラウザで開いても使えます）
2. 機関名で検索するか、OpenAlex の機関 ID（例: `I4210092806`）を入力する
3. 出版年などの条件を選び、「論文を取得して集計」を押す

FWCI の考え方、結果の読み方、使用例はページ内に載せています。

## 注意

- 数値は OpenAlex のデータによるもので、SciVal（Scopus）などの値とは一致しません。
- API キーなしでも使えますが、1 回に取得できるのは 10,000 件までです。それより論文の多い機関は、[OpenAlex の無料 API キー](https://openalex.org/settings/api)をページの「API キー」欄に入れてください。キーは利用者のブラウザ内にだけ保存されます。

## ライセンス

[CC0 1.0](LICENSE)（パブリックドメイン）。OpenAlex のデータも CC0 です。
