## co-pss
====

大学でのプログラミング学習の共有リポジトリ

## Description
issueにて課題などの使用をアップロードし
興味を持った人間がcodeを書く
## Requirement
C開発環境構築が必要  
以下一番多そうなWSLでの構築(下記リンク参照)  
<http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToEnableWSL.html>

WSLの有効化,ubuntuのインストールを完了する  
```
   $sudo sed -i.bak -e "s/http:\/\/archive\.ubuntu\.com/http:\/\/jp\.archive\.ubuntu\.com/g" sources.list  
    $sudo apt update  
    $sudo apt upgrade  
    $sudo apt install build_essential  
    $sudo apt install vim  
```

以下VSCodeを使用した際にterminalにubuntuを設定する方法を示す  
    ・WindowsのCドライブにproC(名前は任意)というリポジトリを作る  
    ・vscodeを起動しfile => prefernces => settings を選択  
    ・右上の{}のアイコンを押しsettings.jsonを開き以下のcodeを入力する  
    `$"terminal.integrated.shell.windows": "ubuntu.exe",`  
    ・VSCodeをリブートする  
    ・VSCodeでターミナルを起動し以下のcodeを入力する  
    `$ sudo vim /etc/passwd`  
    おそらく一番下に  
    Ubuntuユーザ名::1000:1000:"",,,:/home/ユーザ名:/bin/bash  
    となっている場所があるので  
    Ubuntuユーザ名::1000:1000:"",,,:/mnt/c  
    に書き換える(vimの使い方はググって)  
    ・VSCodeをリブートする  
  
以上で環境構築完了です！  
## Usage

## Install
以下をVSCodeのターミナルに入力してください  
`$git clone https://github.com/YuuyaMasaki/co-pss`
