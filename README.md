# BaseRecSys
[推薦システム実践入門](https://www.oreilly.co.jp/books/9784873119663/)の理解。

src, notebook, utilは、統一モジュール。srcには、base_recommender.pyのクラス設計に沿って、各種アルゴリズムが実装。utilは、データの読み込みや評価の統一モジュールが実装。notebookは、srcで実装したアルゴリズムを利用して、アルゴリズムの動作確認をするコードが記述。colabで試せるようにしたつもり。日本語が化ける。


データは以下のようにして取得(以下のようなフォルダ構成になるように)
```
$ wget -nc --no-check-certificate https://files.grouplens.org/datasets/movielens/ml-10m.zip -P ./data
$ unzip -n chapter5/data/ml-10m.zip -d ./data
```

```
BaseRecSys
├─── src
│   ├── base_recommender.py
│   └── etc...
├─── notebook
│   ├── Association.ipynb
│   ├── BPR.ipynb
│   └── etc...
├─── util
│   ├── __init__.py
│   ├── data_loader.py
│   ├── metric_calculator.py
│   └── models.py
└─── data(wgetする)
    └── ml-10M100K
```
