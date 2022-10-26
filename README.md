# BaseRecSys
「推薦システム実践入門」
oreilly.co.jp/books/9784873119663/

src, notebook, utilは、統一モジュール。srcには、base_recommender.pyのクラス設計に沿って、各種アルゴリズムが実装。utilには、データの読み込みや評価の統一モジュールが実装。notebookには、srcで実装したアルゴリズムを利用して、アルゴリズムの動作確認をするコードが記述。



$ wget -nc --no-check-certificate https://files.grouplens.org/datasets/movielens/ml-10m.zip -P ./data

$ unzip -n chapter5/data/ml-10m.zip -d ./data

chapter5
├─── src
│   ├── base_recommender.py
│   ├── association.py
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
└─── colab
    ├── Association.ipynb
    ├── BPR.ipynb
    └── etc...
