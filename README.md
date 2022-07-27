# 課題 15-2: 簡易GUI電卓への機能追加

### 課題の説明
第15回の解説ページにある `WinCalcSample` は、GUI表示になっているものの足し算と引き算の機能しかないため電卓としてはかなり物足りない。
そこで、このコードを発展させた `ProgF2` を次の条件を満たす形で作成しなさい。

- ウィンドウのタイトルを `GUI電卓 各自の学生番号 氏名` とする
- 掛け算、割り算、剰余のボタンと機能を加える
- 割り算の場合、中央のテキストフィールドの数字が0または0.0であれば、右側のテキストフィールドに`0では割れません`を表示する
- 左と中央のテキストフィールドの間に、押したボタンと同じ演算を示すテキストを表示させる（テキストは押したボタンに合わせて変わる）
- 左と中央のテキストフィールドが空っぽまたは数字以外の文字の状態でボタンを押すと例外が発生するので、try-catch文を用いた例外処理を組み込み、例外時には演算を示すテキストを消して右側のテキストフィードに `エラー` を表示する

（注意）本課題でのテストコード提供はないので、各自の実行結果を丁寧に確認してください。


### 完成したProgF2.main()を実行して表示されるウィンドウの例（ 4720000 生命工太 の場合）
起動直後

![ProgF2起動直後](https://user-images.githubusercontent.com/50605381/181152690-d7b74ca9-6cec-432d-b5a9-3e70990ce48f.png)

中央のテキストフィールドの数字が0.0の場合

![ProgF2で0割り算](https://user-images.githubusercontent.com/50605381/181151009-921378d2-fe12-46b9-b901-851273dc4a23.png)

左または中央のテキストフィールドが空っぽまたは文字の場合

![ProgF2で空白演算](https://user-images.githubusercontent.com/50605381/181153703-50a86166-1245-4305-944e-a8beef748461.png)
