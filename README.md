# 改进版的iPSR

本项目是对iPSR的代码的复现和改进，相较于原始iPSR的改进点在于进一步处理了iPSR得到的网格模型，使能够恢复模型的尖锐特征。

iPSR论文：Iterative Poisson Surface Reconstruction (iPSR) for Unoriented Points  
项目地址：https://github.com/houfei0801/ipsr


### 依赖
- Python 3.9, numpy, h5py, scipy, Cython
- PyTorch 1.8

### 使用说明
1. 先配置ipsr进行网格重建
2. 配置nmc的环境，使用nmc中已经训练好的模型进行后处理
'''
python main.py --test_bool_float --data_dir groundtruth/gt_NMC --input_type sdf
'''