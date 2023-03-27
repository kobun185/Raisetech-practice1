# 第5回課題提出

- 組み込みサーバー Pumaでの起動
  ![picture 2](images/197a4ecc52a76497077e06dae10867e56ed1a74a0a650f0f94d48ca244f0035a.png)  

- Pumaでのブラウザ接続
  ![picture 3](images/704ceb8547ade2f88de800c95fa988b8ba8ee4338d3bcfadfbddc735334d368d.png)  

- Nginxの起動
  ![picture 4](images/75e181523b0e973a262b98754d02cad5e0bc244c3254949e748441f9c840533c.png)  

- Unicornの起動
  ![picture 5](images/b4b29db6f6ea8c5ba37215ebf5bd52cc436dd8fc92e893ba462b12dd6a8f49f5.png)  

- ELBの追加
  ![picture 6](images/14da1cabc86181c498459130794947374de2aa6cc0fe27192f14e8063aa5cdeb.png)  

  ![picture 7](images/b807bd05adc40060b9b4f730f2f7c1716afac5caba8ec72da42f73f6459ac12f.png)  

- ターゲットグループのヘルスチェック
  ![picture 8](images/8606f2ea98bdcb30aa91ef0f1247d2e8e7893ea1c8ea1041e33ad97437ad0525.png)  

- S3の追加
  ![picture 9](images/e5cba048a05e35b47077d4cd3e50fa11a28d260be1d52d35e67d28df113a81f4.png)  

  ![picture 10](images/052cb9510e4b56c7f674987546b3b09b6d52298517f43fbcb25e375c6b748c72.png)  

  ![picture 11](images/064885da3ad15d15c9626d25d3b9983d4a3698a87e8ec5100979873c09cf9e53.png)  
<br>
- 構成図

  ![picture 12](images/ba1b22b970dc9a8ead21586c35624d43c4892ba99d6550b91a33d588929ffaeb.png)  
<br>
## 今回の課題でつまずいたポイント  
  - OpenSSL::Cipher::CipherErrorの解決
    - credentials.yml.encとmaster.keyを一旦削除し、再度作り直す事で解決しました。<br>credentials.yml.encとmaster.keyの組み合わせについて調べた事で、鍵の仕組みについて理解が深まりました。
      <br>
    -  環境変数を反映するには、一旦ログアウトしないといけない事に気付くまで、時間がかかってしまいました。<br>
      <br>
  - S3作成後のCORSエラー(No 'Access-Control-Allow-Origin')
    - S3のCORS設定をJSON形式でアクセスを許可できるように追記しました。 <br>オリジンとクロスオリジン、ヘッダーなど、リソース共有の仕組みについて理解が深まりました。<br>
      <br>
## 今回の課題から学んだこと
- エラーコードをしっかり読んで、仮説と検証をする大切さを再確認しました。<br>

- 今回の課題は提出できるまで、かなり時間をかけてしまった。<br>ただ、行った事を思い出せるように、メモを取りながら作業したため、スムーズに作業を再開できた点は良かったと思います。<br>
<br>
## 課題
 -  エラーなどで詰まった際、仮説と検証に何日もかけてしまう事があった。<br>質問するまで、どの程度時間をかけるのか、自分で目安を決めた方が良いと思いました。
