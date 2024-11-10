```bash
git clone https://github.com/OpenDriveLab/OpenLane-V2.git
cd OpenLane-V2
conda create -n openlanev2 python=3.8 -y
conda activate openlanev2
pip install -r requirements.txt
python setup.py develop
```

```bash
pip install torch==1.9.1+cu111 torchvision==0.10.1+cu111 torchaudio==0.9.1 -f https://download.pytorch.org/whl/torch_stable.html
```

```bash
pip install openmim
mim install mmcv-full
mim install mmdet
mim install mmsegmentation
git clone https://github.com/open-mmlab/mmdetection3d.git
cd mmdetection3d
pip install -e .
```

```bash
python demo/pcd_demo.py /home/kuangen/Projects/OpenLane-V2/mmdetection3d/demo/data/kitti/000008.bin configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py checkpoints/second_hv_secfpn_8xb6-80e_kitti-3d-car-75d9305e.pth
```