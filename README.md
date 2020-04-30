## ラズパイ版
- MongoDB
  - 2.x が最新版
  - 設定項目やCRUDオペレーションの関数に差異がある
## memo
- mongodbモジュールのバージョン指定
  - `npm install mongodb@1.2.13`
  - package.json参照
- 認証設定
  - ユーザー作成
    - `db.addUser({user:"admin", pwd:"password", roles:[{role:"root", db:"admin"}]})`
  - mongo起動
    - `mongod --auth`
  - 関数
    - `deleteOne()`→`remove()`
    - `insertOne()`→`insert()`
  - 設定ファイル
    - `auth true`
