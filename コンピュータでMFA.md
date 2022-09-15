# コンピュータで MFA

[MFA(Multi Factor Authentication)]  
多要素認証を意味します。ユーザー名とパスワードだけだと、AWSアカウントの乗っ取り対策として心許ないので、MFAを設定することで、  
認証要素を増やすことが推奨されています。MFAを利用するには、認証コードを発行するデバイスが必要になります。


[実行環境]  
Chrome   バージョン: 100.0.4896.127（Official Build） （64 ビット）

[手順]  
1. コンソールホーム画面の検索窓に「IAM」と入力し、 IAM サービスを選択します。
   ![1](https://user-images.githubusercontent.com/49807271/163696657-13716051-eb75-41b8-ad24-7b64a9ca2e38.jpg)

2. MFA を追加していない場合、IAM のダッシュボードで MFA 追加が推奨されます。  
   「MFA を追加」ボタンを押します。
   ![2](https://user-images.githubusercontent.com/49807271/163697142-373bdeee-0c00-4ceb-9c2c-007c671eadc9.jpg)

3. 「MFA を追加」ボタンを押すと、セキュリティ認証情報が表示されます。「MFA の有効化」ボタンを押します。
   ![4](https://user-images.githubusercontent.com/49807271/163697195-74326494-67c9-4b20-986c-7c585faaf2c4.jpg)

4. MFA デバイスの選択ダイアログが表示されます。仮想 MFA デバイスを選択します。
   ![5](https://user-images.githubusercontent.com/49807271/163697268-acb0b079-048a-4dab-a3ed-5e9098ee9035.jpg)

5. シークレットキーの表示をクリック  
   ![6](https://user-images.githubusercontent.com/49807271/163697317-8ac23614-2eec-4483-bd49-232c3f7eb95e.jpg)

6. 認証アプリをインストールします。色々種類があるので、信頼できるアプリを選択しましょう。
   ~~自分は以下をダウンロードしました。(https://chrome.google.com/webstore/detail/gauth-authenticator/ilgcnhelpchnceeipipijaljkblbcobl/related)~~  
gauthは現在、ブラウザローカルストレージを使用しているのでセキュリティ上の問題を抱えていると言えます。別のアプリを選択しましょう。

7. ブラウザの右上からアドインを選択します。

   ![6](https://user-images.githubusercontent.com/49807271/163697405-81dc49e6-2ca8-4d97-99a4-ba1c2d11eaa8.jpg)

8. Add ボタンを押し、任意の管理しやすい名前を付けます。
   Secret Key の項目は、手順 5 で表示されるキーを入力し、Add ボタンを押します。  
   ![6](https://user-images.githubusercontent.com/49807271/163697456-8d32015a-9593-4dd8-935b-9d45f6342d22.jpg)

9. 定期的に認証コードが更新されるため、2 連続で更新表示される 6 桁の数字を入力し、「MFA の割り当て」ボタンを押します。
   ![8](https://user-images.githubusercontent.com/49807271/163697548-d1fa0c68-9c3e-4fd1-99f3-be4033e944bf.jpg)

10. 次のメッセージが表示されれば、割り当て完了です。
    ![9](https://user-images.githubusercontent.com/49807271/163697656-1f02cfe1-bb8e-4131-b94c-2fd6bcb84e7d.jpg)

11. AWS アカウントをログアウトして、再度ログインを試してみます。
    ログイン時に MFA 認証が求められたら、認証アプリの認証コードを入力してログインします。
    ![11](https://user-images.githubusercontent.com/49807271/163697700-0c74dfb7-2a44-4d81-95d8-59fda553da05.jpg)

以上です。
