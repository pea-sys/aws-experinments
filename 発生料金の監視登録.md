# 発生料金の監視設定

1. AWS マネジメントコンソールから Billing サービスを選択します

   ![1](https://user-images.githubusercontent.com/49807271/165496677-29818af1-278a-4e34-b35b-f39b6866d3ab.jpg)

2. 請求設定を選択します

   ![2](https://user-images.githubusercontent.com/49807271/165496737-c7dd6365-a17b-4a26-8403-59d3b8ed33c2.jpg)

3. 各種設定項目にチェックを入れて設定を保存します

   ![3](https://user-images.githubusercontent.com/49807271/165497722-dcc349cb-b0f4-49a1-bf04-8337e90f6b76.jpg)

4. 「請求アラートを管理する」リンクをクリックし、CloudWatch サービスのダッシュボードにアクセスします

5. アラームを作成をクリック

   ![4](https://user-images.githubusercontent.com/49807271/165498913-b79736fb-f4ad-4d4e-b1d4-f0f39c6c1cdc.jpg)

6. アラームの作成をクリック

   ![5](https://user-images.githubusercontent.com/49807271/165499430-8310adb9-b730-48aa-9920-681e26465431.jpg)

7. メトリクスの選択をクリック

   ![6](https://user-images.githubusercontent.com/49807271/165500174-1fc8cc94-f6c2-4726-aaa2-b7e06a9dcc1a.jpg)

8. 請求 → 概算合計請求額を選択

   ![8](https://user-images.githubusercontent.com/49807271/165500731-e8edceab-52e7-4d2e-a6aa-bd59b68ba338.jpg)

9. USD を選択して、メトリクスの選択

   ![9](https://user-images.githubusercontent.com/49807271/165501047-e5f8c066-6f1d-4222-b6cc-eb47f6abf34e.jpg)

10. 監視設定を登録します
    ここでは 10 ドルを越えた場合に、メール通知を受け取るようにしています
    
    ![8](https://user-images.githubusercontent.com/49807271/165502937-9b93f9ac-74f4-488a-8590-3d3e8b6cb509.jpg)

11. 通知の追加を選択し、トピックを作成します

    ![10](https://user-images.githubusercontent.com/49807271/165503764-17ff03c1-f71c-4380-b3cc-d1d5345806ca.jpg)

12. トピック作成後、通知先のメールアドレスに承認確認が来るので承認します

13. 「次へ」ボタンをクリック

14. アラート名を設定して、「次へ」ボタンクリック

    ![12](https://user-images.githubusercontent.com/49807271/165504510-2bcc8d74-190f-40ef-aca9-da45d625cbc3.jpg)

15. アラームの作成をクリックして完了です
