# MFA ロストによりログインできない場合の対処方法

- 1. 「Troubleshoot MFA」をクリック
     ![1](https://user-images.githubusercontent.com/49807271/189111283-e2e45ffc-ce33-45df-89c3-009c726ab4a6.png)

- 2.「Sign in using alternative factors」をクリック

![2](https://user-images.githubusercontent.com/49807271/189111720-c0221eb1-63e8-4392-848f-b3166ba0533e.png)

- 3.「Send verification email」をクリック

![3](https://user-images.githubusercontent.com/49807271/189118694-a7fc7fc0-76e7-410d-bcf9-0b1dd8d02acf.jpg)

- 4.間もなく登録しているメールアドレスに aws から認証メールが届きますので、「Verify your email address」をクリック

- 5.クリックすると Email address verification にチェックマークが付きます。
  次は電話認証のため「Call me now」をクリック

![4](https://user-images.githubusercontent.com/49807271/189120089-4127a71a-b8fb-46c2-a111-4a62a3f75387.jpg)

- 6.それで認証が出来れば良いのですが、私の場合は出来なかったです。
  その場合、AWS Support の手を借りる必要があります。
  「AWS Support」をクリックします
  ![5](https://user-images.githubusercontent.com/49807271/189120331-28ae37fe-1df0-4e3c-8a1b-a9aab7492bc5.png)

- 7.説明文の手順で認証できなかった場合、AWS Support のボタンを再度押します。  
  日本語でサポートを受けたい場合は平日 9 時～ 18 時に電話が来るので注意。
  ![6](https://user-images.githubusercontent.com/49807271/189120730-1d38a4f4-0ef3-4ac6-9733-6a62b9895150.png)

- 8.後日、電話が来ました。  
   手続きの内容は伏せますが、時間が掛かるものではありませんでした。  
   無事、Admin の MFA は解除されました。  
   当たり前ですが、IAM ユーザーの MFA は解除されません。  
   Admin と IAM で同じデバイスまたは仮想デバイスで MFA を使用している場合は、Admin で IAM ユーザーの MFA を無効化することで、IAM ユーザーでログインできるようになります。

  比較的簡単に MFA 解除の手続きは出来るので、MFA 再紛失のリスクを恐れず、すぐに再設定することをお勧めします。
