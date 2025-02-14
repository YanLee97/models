# Posenet

Posenet is a backbone network, we use it to classify face pose.

## Train on face pose dataset Dataset
The face pose dataset can be downloaded from [BaiduNetdis](https://pan.baidu.com/s/1KbrMUrUIS_cCzpDgdgjMRQ) code: o9tg .

### Download Ofrecord

```bash
wget https://oneflow-public.oss-cn-beijing.aliyuncs.com/datasets/models/pose/pose_dataset.zip
unzip pose_dataset.zip
```

### Run Oneflow Training script
We have installed visdom to visualize the training model, and run the following program to enter http://localhost:8097/ get the training curve.

```
pip3 install -r requiements.txt --user
```
```
python -m visdom.server
```
```bash
bash train_oneflow.sh
```
## Inference on Single Image

```bash
bash infer.sh
```

### Accuracy
|         | val(Top1) |
| :-----: | :-----------------: |
| Posenet  |        0.906        |
