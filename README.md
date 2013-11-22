SassフレームワークCompass
============
# 目的 #
SassフレームワークCompass詳細

# 前提 #
| ソフトウェア   | バージョン   | 備考        |
|:---------------|:-------------|:------------|
| OS X           |10.8.5        |             |
| ruby           |2.0.0p247     |             |
| sass           |3.2.12        |             |
| compass        |0.12.2        |             |

# 構成 #
+ [セットアップ](#cha1)
+ [Compassを利用する準備](#cha2)
+ [Compassのインポートとモジュール](#cha3)
+ [Compassのミックスインを使う](#cha4)
+ [Compassの設定変数を定義する](#cha5)
+ [Compassの関数(Helpers)](#cha6)
+ [Compassで簡単CSSスプライト(Compass Sprites)](#cha7)
+ [高度なCSSスプライトの使用方法(Sprite Helpers)](#cha8)

# 詳細 #
## <a name="cha1">セットアップ ##

    $ rvm use ruby-2.0.0-p247
    $ rvm gemset create compass
    $ rvm use ruby-2.0.0-p247@compass
    $ gem install sass
    $ gem install compass


## <a name="cha2">Compassを利用する準備 ##
+ プロジェクトを作成する

        $ compass create introduction --sass-dir "scss" --css-dir "css"
        $ cd introduction
        $ tree
        .
        ├── config.rb
        ├── css
        │   ├── ie.css
        │   ├── print.css
        │   └── screen.css
        └── scss
            ├── ie.scss
            ├── print.scss
            └── screen.scss        

+ config.rbの設定

+ Compassでコンパイルしてみる

        $ compass w

## <a name="cha3">Compassのインポートとモジュール ##
+ Compassをインポートする  
  scss/screen.scss  

        @import "compass";

## <a name="cha4">Compassのミックスインを使う ##
+ [CSS3モジュール](introduction/scss/css3.scss)

+ [Utilitiesモジュール](introduction/scss/css4.scss)

+ [Typographyモジュール](introduction/scss/css5.scss)

## <a name="cha5">Compassの設定変数を定義する ##
+ [ペンダープレフィックスのオン/オフ](introduction/scss/css6.scss)

+ [レガシーブラウザの対応のオン/オフ](introduction/scss/css7.scss)

+ その他の設定変数

## <a name="cha6">Compassの関数(Helpers) ##
+ [画像関連の関数(Image Helpers)](introduction/scss/css8.scss)

+ [色(Color Helpers)](introduction/scss/css9.scss)

+ [セレクタで使う関数(Selector Helpers)](introduction/scss/css10.scss)

## <a name="cha7">Compassで簡単CSSスプライト(Compass Sprites) ##
+ [マジックインポートでスプライト画像を作成する](introduction/scss/css11.scss)

+ [背景の位置を書き出す](introduction/scss/css12.scss)

+ [Spritesの設定変数](introduction/scss/css13.scss)

+ [マジックセレクタで疑似クラスを作成する](introduction/scss/css14.scss)

+ [個別のセレクタにプロパティと値を渡す](introduction/scss/css15.scss)

## <a name="cha8">高度なCSSスプライトの使用方法(Sprite Helpers) ##

+ [スプライト関数(Sprite Helpers)](introduction/scss/css16.scss)

+ [関数を組み合わせて使う](introduction/scss/css17.scss)

+ sprite-map()関数で使えるミックスイン

# 参照 #

[compass](http://compass-style.org/)

[Web制作者のためのSassの教科書](http://book.scss.jp/)
