# GeneratedCodePredictor
自動生成コードかどうか判定する分類器を構築し，その精度を検証するツールです

## なぜ必要？
多くのOSSにはコンパイラコンパイラなどの自動生成コードが含まれています．<br>
ソフトウェア工学分野などで人が書いたソースコードを分析したいというときに，
本ツールを用いて人によって書かれたコードでないコードを取り除くことができます．<br>

## ツールの動作の流れ
1．[ExtractingSourceFeatures](https://github.com/SoichiSumi/ExtractingSourceFeatures)を用いて作成した学習データを入力として受け取る<br>
2. [WekaAPI](https://weka.wikispaces.com/Use+WEKA+in+your+Java+code#Links)を用いて特徴選択・分類器構築・交差検証を行う<br>

## 評価実験結果
ApacheProjectsから手作業で取得した自動生成コードと非自動生成コードを学習データとして，交差検証を行いました．
精度は約95%でした．

実験結果の詳細は近日公開予定です．
