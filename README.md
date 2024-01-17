# Turbo Performance说明

## 一.motivation代码，测试数据及图片

代码均在motivation文件夹下

### `motivation_scale.py`

测试数据在代码内，保存图片名称为motivation_scale.png

### `motication_complexity.py`

测试数据在代码内，保存图片名称为motivation_complexity.png

### `motivation_spike.py`

测试数据为spike.csv，第一列数据为shuffle read时间，单位是s，第二列是shuffle read数据量大小。保存图片名称为motivation_spike.png

### `motivation_imbalance.py`

测试数据为motivation_imbalance.txt，第一列是端口1的出口带宽，第二列是端口2的出口带宽。保存图片名称为motivation_imbalance.png

### `motivation_executor.py`

测试数据在代码内，保存图片名称为motivation_executor.png

### `motivation_bandwidth.py`

测试数据为motivation_bandwidth.txt，第一列是端口1的出口带宽，第二列是端口2的出口带宽。保存图片名称为motivation_bandwidth.png

## 二.evaluation代码，测试数据及图片

如无强调，代码就在evaluation文件夹下

### `block_cmp.py`

代码在/evaluation/blocksize文件夹中，测试数据分别为10kb,100kb,1mb,4mb的block size下使用不同通信方式（TCP, RDMA, Turbo）网卡两端口的出口带宽，rckb10.txt则表示通信方式为RC RDMA，数据块大小为10kb的两端口出口带宽。代码中，调用不同函数（kb10，kb100，mb1，mb4）画对应数据块大小的测量图，保存图片为6-1.png(10kb),6-2.png(100kb),6-3.png(1mb),6-4.png(4mb)。

### `average_bandwidth_cmp.py`

测试数据分别在RC_bandwidth.txt，DC_bandwidth.txt，Turbo_bandwidth.txt中。保存图片名称为6-5.png
