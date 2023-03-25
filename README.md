# **第6回課題提出**

## **CloudTrailのイベントの中にはどんな情報が含まれていますか?**
<br>
StartInstances<br>
イベント時間：March 16, 2023, 18:58:33 (UTC+09:00)<br>
リソースタイプ：AWS::EC2::Instance<br>
AWS リージョン：ap-northeast-1<br>
<br>
StartDBInstance<br>
イベント時間：March 16, 2023, 18:58:10 (UTC+09:00)<br>
リソースタイプ：AWS::RDS::DBInstance<br>
AWS リージョン：ap-northeast-1<br>
<br>

---
## **CloudWatchアラームの設定とメール通知**
<br>

### **ALBのUnHealthy、アラーム設定とメール通知**
>Railsアプリケーションを使えない状態にすると、<br>コンソールの表示がアラーム状態となり、アラームメールが通知されました。
![picture 13](images/6b0274868f30a5ced73a8ead4a09d00a0b6a68964db7e11aa57eaf3a279c82d3.png)  
![picture 14](images/5af3038ec5a1483b2a2570397ecd21127b088fa4f216ae5b81c8bca2b2125a07.png)  

<br>

### **ALBのHealthy、OKアクション設定とメール通知**
>Railsアプリケーションを使える状態にすると、<br>コンソールの表示がOK状態となり、OKメールが通知されました。
![picture 15](images/7f7fa84b3a189b513ddb4d154f60110302ff26723d3d7f95e95089d188506b79.png)  
![picture 16](images/79dbcb52d4691c3b76d2f2e6b40fe095acc508e2bb770386e60e240615277f39.png)  

<br>

---
## **AWS利用料の見積を作成してください。**

>見積りURL：
https://calculator.aws/#/estimate?id=04bda927bcef046814b42d287ab2559cfc3a14cb

<br>

---
## **マネジメントコンソールから、現在の利用料を確認して教えてください。**

![picture 17](images/bbb319a1b5e3ed98729d2f8bd4deae6320ec2b8189ffe129e53c99640a77f2a3.png)  
<br>

---
## **先月の請求情報から、EC2 の料金がいくらか確認してください。**

![picture 19](images/592d0ebab41b15bfbeb73f7d0452c69c04066afe2115ef7b11205f5ffa267314.png)  
<br>

---
## **無料利用枠で収まっていますか？**

![picture 20](images/0c52b76a73ed414cef5a0677a0b04575d218dbe4aa080a3638b550c82179936b.png)  

> 無料枠の期限が切れているため、無料利用枠で収まっていません。
<br>

---
## **今回の課題から学んだこと**
>今回の作業を通して、ログを取って調べる事、監視して通知する事は<br>重要な事だと学びました。<br>
今回触れなかったサービスや機能も理解できる様、学習を続けたいと思いました。
