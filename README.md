# setup_pc
私が普段使いのパソコンをセットアップする手順をまとめます。  

## １．大まかな流れ
1. Windows Update を実行。
2. 「netplwiz」を実行して、「ユーザーがこのコンピューターを使うには、ユーザー名とパスワードの入力が必要」のチェックを外す。チェック欄がない場合は、レジストリエディタで「SOFTWARE￥Microsoft￥Windows NT￥CurrentVersion￥PasswordLess￥Device」にある「DevicePasswordLessBuildVersion」の値を「2」から「0」にする。
3. Google Chrome をインストール。（ https://www.google.com/chrome/ ）
4. LINE Windows 版をインストール。（ https://line.me/ja/ ）
5. ZOOM Windows 版をインストール。（ https://zoom.us/ja/download ）
6. Visual Studio Codeをインストール。（ https://azure.microsoft.com/ja-jp/products/visual-studio-code ）
7. git Windows 版をインストール。（ https://gitforwindows.org/ ）
8. [git の設定](#anchor2)
9. [Visual Studio Code の設定、拡張機能の導入](#anchor3)
10. Kindle Windows 版をインストール。（ https://www.amazon.co.jp/kindle-dbs/fd/kcp/ ）
11. Amazon アプリストアをインストール。（ https://blogs.windows.com/windows-insider/2021/10/20/announcing-android-apps-on-windows-11-preview-for-windows-insiders-in-the-beta-channel/ ）
12. Amazon アプリストアで、iRealPro をインストール。


## <a id="anchor2">２．git の設定</a>
ユーザー名とメールアドレスを設定するのと、GitHub にアップロードする際に都度パスワード入力をしなくていいように、パスワードを保存する設定にします。
```dos
mypc C:\GitHub\hoge> git config --global user.name "hogehoge"
mypc C:\GitHub\hoge> git config --global user.email hogehoge@example.com  
mypc C:\GitHub\hoge> git config --global credential.helper store  
```

確認します。
```dos
mypc C:\GitHub\hoge> git config user.name  
hogehoge  
mypc C:\GitHub\hoge> git config user.email  
hogehoge@example.com  
mypc C:\GitHub\hoge> git config --global credential.helper  
store  
```  
  

## <a id="anchor3">３．Visual Studio Code の設定、拡張機能の導入</a>