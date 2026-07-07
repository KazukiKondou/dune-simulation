# dune-simulation (all-num-test)

砂丘（dune）形成の数値シミュレーション。可変5定数（`L0`, `A2`, `b`, `q0`, `D`）を
パラメータ範囲で走査し、各条件について 400 ステップ時点の砂丘形状を可視化する。

- 境界条件: x方向（風向き）= 周期境界 / y方向（横断方向）= 壁境界
- 実装: `dune_simulation.ipynb`（コード＋実行結果を同梱）

## 必要環境

```bash
pip install numpy matplotlib plotly jupyter
```

## 実行方法

```bash
jupyter notebook dune_simulation.ipynb
```

各セルを上から実行するとパラメータ走査が走り、結果が描画される。

## 班メンバー向け: 結果の共有

初回:

```bash
git clone <このリポジトリのURL>
cd all-num-test
```

以降、最新の結果を取り込む:

```bash
git pull
```

結果を更新して共有する側:

```bash
git add dune_simulation.ipynb
git commit -m "update: シミュレーション結果を更新"
git push
```
