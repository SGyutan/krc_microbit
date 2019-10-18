## KRCオリジナル基板用の（Microbit用）送受信コード
受信側のDC制御関数をそれぞれのボード用に書き換えることで、別のボードにも対応できます。

Qiitaに説明した記事があります。
[Microbit:DC motor制御その3（無線送受信プログラムの変更）](https://qiita.com/Gyutan/items/93adbd19596235c11cf6)


DFRobotのボードを使ったプログラムを追加。
腕の動作がサーボモーターになっている。
サーボモータの電圧が4.8Vなので、動かすとMicrobit側の電圧が落ちて初期化から始まってしまう。
ボード側の電圧を6V（電池4つ）にしても状況は同じで落ちる。直接Microbit側に供給しないといけない。
