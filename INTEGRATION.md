```
FROM nvidia/cuda:9.1-cudnn7-runtime-ubuntu16.04
```

```bash
apt-get update && \
apt-get install -y wget git python-dev python-pip && \
pip install requests scipy rawpy && \
pip install --user --upgrade tensorflow && \
export TF_CPP_MIN_LOG_LEVEL=2 && \
cd && \
git clone https://github.com/ramongduraes/Learning-to-See-in-the-Dark.git && \
cd Learning-to-See-in-the-Dark && \
python download_models.py && \


```