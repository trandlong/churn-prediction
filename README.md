## Make sure to use virtualenv install of python3 -m venv
```bash
virtualenv -p python3 .venv
brew install libtiff libjpeg webp little-cms2 ffmpeg
pip install -r requirements.txt
```
### Install LearnTool
```bash
pip install git+https://github.com/Kaggle/learntools.git
```

## Using conda to install virtual environment
```bash
conda create --prefix $PWD/venv python=3.9
conda activate $PWD/venv

conda install -y catboost numpy lightgbm
conda install -y -c conda-forge pdpbox eli5 #imbalanced-learn

# intel chip run: 
conda install -y -c conda-forge tensorflow
pip install -r requirements.txt

# M1 chip run
conda install tensorflow-deps
pip instal -r macos-m1.txt
pip install -r requirements.txt
```