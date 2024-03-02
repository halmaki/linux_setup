# Setup Laptop
普段使いのノートパソコンのセットアップ

## [EndeavourOS](https://endeavouros.com/)をインストール
1. [EndeavourOS](https://endeavouros.com/)からディスクイメージをダウンロード
2. ブートしたらインストーラーに従ってインストール
> **注意**
> 持ち運ぶのでluksを使用して暗号化する

## パッケージを最新に更新する
```bash
sudo pacman -Syu
```
その他必要なソフトのインストール
```bash
sudo pacman -S code gvim neovim
```

## 日本語入力をできるようにする
```bash
sudo pacman -S fcitx5 fcitx5 fcitx5-mozc
```
インプットメソッドにMozcを使用する
環境変数を設定するために`~/.xprofile`に
```bash
GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx
```
を書いて、一旦ログアウトする。その後、fcitx5-configtoolでMozcを追加する。

## i3 WMの設定

