# これは何か

色々なものの練習用として動くものを用意した場所

Nablarchのブランクプロジェクトとして作成（web）
https://nablarch.github.io/docs/LATEST/doc/application_framework/application_framework/blank_project/setup_blankProject/setup_Web.html

# H2に格納されているデータを確認する方法

以下の手順で確認する。

1.「mvn waitt:run」でアプリを起動している場合は終了させる。

2.h2/bin/h2.batを実行する。

3.しばらく待つとブラウザが起動するので、各項目に以下の通りに入力し、[Connect]ボタンをクリックする。

| 項目     | 値                  |
|:---------|:--------------------|
|JDBC URL  |jdbc:h2:../db/SAMPLE |
|User Name |SAMPLE               |
|Password  |SAMPLE               |

4.左側のペインのテーブル名をクリックすると、クリックしたテーブルに対するSELECT文が生成される。

5.[Run]ボタンをクリックすると、生成したSELECT文が実行され、テーブルのデータを確認することができる。

6.使用終了時は、左上のdisconnectボタン(赤色で書かれたアイコンのボタン)をクリックして切断する。
  **切断を忘れると、WebアプリからH2に接続できなくなる。**
