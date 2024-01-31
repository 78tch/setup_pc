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
1. 「日本語化する」：Code のインストール直後はUIも英語。なにはなくとも「Japanese Language Pack for Visual Studio Code」機能拡張をインストールして日本語化する。  
2. 「スペース文字を表示する」：Render Whitespace を「all」にする。Markdown の改行である「スペース2個」の有無を見分けるため。  
3. 「対応する括弧の色分け」：標準機能になったため、機能拡張を入れる必要はなくなった。  
4. 「対応する括弧にジャンプする」：括弧の内側にフォーカスを当てて「Ctrl」+「Shift」+「￥」で、対応する括弧にフォーカスがジャンプする。
5. 「ドキュメントのフォーマット」：エディタの右下のステータスバーで「言語モード」を選択し、エディタ上で右クリックして「ドキュメントのフォーマット」を実行すると、インデントなど見易く整形してくれる。  
6. 「Markdown Preview Github Styling」：Markdown 記法で書いた文書をGithub のスタイルでプレビューできる。
7. 「Auto-Open Markdown Preview」：拡張子「.md」なファイルを開くと、プレビューウィンドウも自動で開く。
8. 「Excel to Markdown table」：表計算で範囲をコピーした状態で、コマンドパレットから呼び出すと、「table」記法にして貼り付けてくれる。
9. 「Markdown All in One」：目次、セクション番号、オートコンプリート、キーボードショートカットによる入力補助など。改行したときの自動採番、修正したときの番号振り直しなど。