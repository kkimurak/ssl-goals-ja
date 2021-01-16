# ロボカップ小型機リーグ基本理念及び長期目標

[English](README.md) | Japanese  

ロボカップ小型機リーグ(SSL)基本理念および長期目標の非公式日本語訳の、AsciiDoc形式のソースコードです。

原文は[小型機リーグ公式GitHubリポジトリ](https://github.com/robocup-ssl/ssl-goals)よりご覧いただけます。

## ビルド

本ドキュメントはmaster-jaブランチの更新に応じて、自動的に[Githuub Page](https://kkimurak.github.io/ssl-goals-ja/sslgoals.html)に公開されます。[PDF版](https://kkimurak.github.io/ssl-goals-ja/sslgoals.pdf)もご利用いただけます。  

### ネイティブ版AsciDoctorの使用

AsciiDoctorをインストールしてください (https://asciidoctor.org/)。 その後、以下のコマンドでHTML5版をビルドできます :

```sh
# HTML5版のビルド
asciidoctor sslgoals.adoc
```

日本語を含むPDFを生成する場合、asciidoctor-pdf-cjk-kai_gen_gothicを使うと良いでしょう :

```sh
# Build the PDF version
asciidoctor-pdf -r asciidoctor-pdf-cjk-kai_gen_gothic -a pdf-style=KaiGenGothicJP sslgoals.adoc
```

### dockerイメージの使用

Dockerをインストールしているのであれば、日本語環境向けに最適化されたAsciiDoctorイメージを使うことができます :
rをインストールしているのであれば、日本語環境向けに最適化されたAsciiDoctorイメージを使うことができます :

```sh
# dockerイメージをpullする
docker pull htakeuchi/docker-asciidoctor-jp
# HTML5版のビルド
docker run -v $PWD:/documents/ htakeuchi/docker-asciidoctor-jp asciidoctor sslgoals.adoc
# Build the PDF version
docker run -v $PWD:/documents/ htakeuchi/docker-asciidoctor-jp asciidoctor-pdf -r asciidoctor-pdf-cjk-kai_gen_gothic -a pdf-style=KaiGenGothicJP asciidoctor-pdf sslgoals.adoc
```
