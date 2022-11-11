# SINet
### Human Pose Estimation via Scale-Interacted Neural Network
This repo is based on [HRNet](https://github.com/leoxiaobin/deep-high-resolution-net.pytorch). Please follow [HRNet](https://github.com/leoxiaobin/deep-high-resolution-net.pytorch) to install datasets and set up the programming environment.
### Training SINet
```
python tools/train.py --cfg experiments/coco/covariance_hrnet/imagenet_pretrain_783_v6_w32_256x192_adam_lr1e-3.yaml
```
### Testing SINet
```
python tools/train.py --cfg python tools/test.py \
    --cfg experiments/coco/covariance_hrnet/imagenet_pretrain_783_v6_w32_256x192_adam_lr1e-3.yaml \
    TEST.MODEL_FILE ${Your Weight File} \
    TEST.USE_GT_BBOX False
```