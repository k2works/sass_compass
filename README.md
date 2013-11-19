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
+ [CSS3モジュール](scss/css3.scss)

+ Utilitiesモジュール

+ Typographyモジュール

## <a name="cha5">Compassの設定変数を定義する ##

## <a name="cha6">Compassの関数(Helpers) ##

## <a name="cha7">Compassで簡単CSSスプライト(Compass Sprites) ##

## <a name="cha8">高度なCSSスプライトの使用方法(Sprite Helpers) ##

# 参照 #
[compass](http://compass-style.org/)
