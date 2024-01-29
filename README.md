# setup_pc
私が普段使いのパソコンをセットアップする手順をまとめます。  
  
  1. Windows Update を実行。
  2. 「netplwiz」を実行して、「ユーザーがこのコンピューターを使うには、ユーザー名とパスワードの入力が必要」のチェックを外す。チェック欄がない場合は、レジストリエディタで「SOFTWARE￥Microsoft￥Windows NT￥CurrentVersion￥PasswordLess￥Device」にある「DevicePasswordLessBuildVersion」の値を「2」から「0」にする。
  3. 最新のUbuntu 日本語Remix をデフォルト設定でクリーンインストール。  
  4. 「ソフトウェアの更新」の「設定」で「ダウンロード元」を日本のサーバーに、「他のソフトウェア」でパートナーにチェックを入れ、ソースコードのチェックを外す。  
  5. 「言語サポート」でインストールを完了。  
  6. [「/etc/inputrc」で「history-search-backward」を有効](https://github.com/78tch/setup_pc/blob/master/inputrc.md)にする。  
  7. [「/etc/fstab」で2nd SSD を自動マウント](https://github.com/78tch/setup_pc/blob/master/fstab.md)する。  
  8. [「apt-get」で「byobu」「git」「virtualbox」「vagrant」をインストール](https://github.com/78tch/setup_pc/blob/master/aptget.md)する。  
  9. 「Ubuntuソフトウェア」で「Peek」「Discord」「OBS」をインストール。  
  10. 「Visual Studio Code」「Chrome」のサイトからdeb ファイルをDLしてインストール。
  11. [git の設定](https://github.com/78tch/setup_pc/blob/master/git.md)をする。
  12. [Visual Studio Code の設定。](https://github.com/78tch/setup_pc/blob/master/vscode.md)
  13. [vagrant でテスト環境を用意。](https://github.com/78tch/setup_pc/blob/master/vagrant.md)
  14. Windows の場合。
  15. test