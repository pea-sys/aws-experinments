# IAM ユーザー登録

■ 次の IAM ユーザーを登録します

---

- 管理者権限を保有する IAM ユーザー
- S3 の一覧表示可能なユーザー

---

## ■ 手順

1. AWS マネジメントコンソールから IAM サービスを選択します。
   ![1](https://user-images.githubusercontent.com/49807271/165300855-fd56be17-b9fe-477c-a174-0235875b1903.jpg)

2. ユーザーを選択後、ユーザーを追加を選択
   ![2](https://user-images.githubusercontent.com/49807271/165301262-188121ed-0345-473e-b328-5ca59aea50e8.jpg)

3. 必要情報を入力します
   ![3](https://user-images.githubusercontent.com/49807271/165302255-a4d927b9-c2f0-4e0b-8fa3-debb24453805.jpg)

4. 用途に合わせて、AWS の管理ポリシーをアタッチするか
   カスタムポリシーを作成します。
   ![1](https://user-images.githubusercontent.com/49807271/165403252-ce15115b-835b-41f6-93f7-f5792e6b831f.jpg)

5. グループ名を入力し、グループの作成ボタンを押下します
   ![5](https://user-images.githubusercontent.com/49807271/165303389-d38ad31a-b5a4-4040-92f2-9c1d77a76623.jpg)

6. タグは必要に応じて登録し、次のステップ(確認)ボタンを押下します

7. ユーザーの作成ボタンを押します
   ![7](https://user-images.githubusercontent.com/49807271/165316890-4f0c4dbc-a395-4dc9-bfc0-9b925cb717a3.jpg)

8. アクセスキーとシークレットアクセスキーが記載されている csv ファイルのダウンロードボタンを押下します。
   ※このファイルは外部に公開しないよう厳重に取り扱う必要があります

9. サインアウトします

10. IAM ユーザーでログイン出来ることを確認します

    ![9](https://user-images.githubusercontent.com/49807271/165315076-6281bee7-81ea-4f83-8ad7-0f03de9418ab.jpg)

11. 同じ手順で IAM ユーザーをもう一人登録します  
    ただし、ポリシーは「AmazonS3ReadOnlyAccess」を選択します

![12](https://user-images.githubusercontent.com/49807271/165532310-5044a1a2-9868-4e83-a66a-b99682046cb0.jpg)

12. s3 のダッシュボードにアクセスします

## ![13](https://user-images.githubusercontent.com/49807271/165533361-92522583-dfe2-4233-98ec-1b1f5958199b.jpg)

13. バケットの作成をクリックし、バケットを作成します

    ![15](https://user-images.githubusercontent.com/49807271/165638276-4e059323-24db-4f3a-8533-1fafd77ae427.jpg)

14. 「AmazonS3ReadOnlyAccess」の IAM ユーザーでログインします

15. s3 の作成を試みます。  
    書き込み権限がないので次のようなエラーが表示されます

![16](https://user-images.githubusercontent.com/49807271/165749784-48b2bc94-0c62-4bd4-a27d-b4e098d5eacf.jpg)
