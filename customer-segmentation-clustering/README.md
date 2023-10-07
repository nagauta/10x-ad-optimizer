# customer-segmentation-clustering
## 初めに
[Kaggle](https://www.kaggle.com/code/karnikakapoor/customer-segmentation-clustering/notebook)をローカルで検証するためのプロジェクトである。

## 検証環境
- MacBook Air (M1, 2020)
- Docker Desktop for Mac

## 環境構築 miniconda3
- `conda env create -n 新たな環境名 -f x-1.yml`
- `customer-segmentation-clustering-checkpoint.ipynb`を開く
- kernaelで`x-1`を選択する
- 手順通りに実行していく

## 環境構築 Docker(作成中)
- `conda create -n sober-macos python=3.10`
- `conda activate x-1`
- `customer-segmentation-clustering-checkpoint.ipynb`を開く
- kernelで`x-1`を選択する　※候補になければvs code ウィンドウリロードする or 再起動

### メイン
- terminalでこちらのディレクトリに移動する
- Docker Desktop for Macを起動する
- `docker-compose up`

### miniconda install
- terminalで別タブを開く
- `docker exec -it <container_name_or_id> /bin/bash`　※立ち上げたコンテナの<container_name_or_id>を設定すること
- cd `work`
- `bash Miniconda3-latest-Linux-aarch64.sh`
- いくつか聞かれるのでyesを押下すればOK
- `conda --version`
- バージョン情報が出力されればOK
- `conda create -n x-1 python=3.10`

### メイン
- 元のタブに戻る
- `open http://127.0.0.1:8888/lab`　※直接ブラウザで開いてもOK
- notebook上で`customer-segmentation-clustering/work/customer-segmentation-clustering.ipynb` を選択する