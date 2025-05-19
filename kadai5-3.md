## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
* エンドポイント:https://zipcloud.ibsnet.co.jp/api/search
* 機能:*郵便番号を入力するとそれに対応する都道府県、市区町村の情報を返すAPI
* リクエストとレスポンスのフォーマット
* リクエスト:https://zipcloud.ibsnet.co.jp/api/search?zipcode=1000001
* レスポンス:住所：{
  "message": null,
  "results": [
    {
      "zipcode": "1000001",
      "prefcode": "13",
      "address1": "東京都",
      "address2": "千代田区",
      "address3": "千代田",
      "kana1": "ﾄｳｷｮｳﾄ",
      "kana2": "ﾁﾖﾀﾞｸ",
      "kana3": "ﾁﾖﾀﾞ"
    }
  ],
  "status": 200
}

### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
* 名称：ランダム猫画像API
* 参照URL：[https://api.thecatapi.com/v1/images/search](https://thecatapi.com/)
* エンドポイントと機能
* エンドポイント:https://api.thecatapi.com/v1/images/search
* 機能:the cat api を使って、入力内容に応じて猫の画像を表示する
* リクエストとレスポンスのフォーマット
* リクエスト：GET https://api.thecatapi.com/v1/images/search?limit=1
* レスポンス：[
  {
    "id": "MTY3ODIyMQ",
    "url": "https://cdn2.thecatapi.com/images/MTY3ODIyMQ.jpg",
    "width": 500,
    "height": 750
  }
]

### Q3-3. 感想
* 今回の課題で苦労したこと
* どのようなAPIを使うか迷った
* 少しいじらないとうまく作動しなかった
* 演習を通して理解できたこと
* 世の中には面白いAPIがたくさんあり、単語を入力するだけでデータを出力できるということが分かった
* Web APIの利便性や課題など
* 基本的に簡単な情報をいれるだけで動くので、とても使いやすいし、すぐに除法が出てきてくれるので便利だと思った。
* データベースなどが大量に必要な場合があるのでそこは課題なのかなと思った。
