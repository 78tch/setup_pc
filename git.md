# git の設定  
ユーザー名とメールアドレスを設定するのと、GitHub にアップロードする際に都度パスワード入力をしなくていいように、パスワードを保存する設定にします。
```sh
$ git config user.name "hogehoge"
$ git config user.email hogehoge@example.com  
$ git config --global credential.helper store  
```  
確認します。
```sh
$ git config user.name  
hogehoge  
$ git config user.email  
hogehoge@example.com  
$ git config --global credential.helper  
store  
```  
  
  
<img src="images/git1.png" alt="image">  
