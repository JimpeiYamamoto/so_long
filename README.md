# 42_so_long
C言語でグラフィック用ライブラリであるminilibxを用いて作成した2Dゲームです。  
コマンドライン引数から受け取った任意のMAPファイル(.ber)を読み込んでゲームをプレイすることができます。
## インストール
```
git clone git@github.com:JimpeiYamamoto/42_so_long.git 
```
## コンパイル(Linux環境)
```
make bonus
```
## 遊び方
```
./so_long_bonus [MAPFILE].ber
```
### ルール
- プレイヤーはWSADキーを使って上下左右に動くことができます。
- お化けに捕まらないように、お宝を全て拾って家まで帰るとクリアです。
### MAPFILE.berの例
```
1111111111111
10010000000C1
1000011111001
1P0011E000001
1111111111111
```
- 1 : 壁
- 0 : 床
- C : お宝
- P : プレイヤー
- E : 出口
### 工夫した点
- アニメーションをつけて視覚的にも楽しめるようにした
- お化けの動き方を最適化することで退屈しない内容とした