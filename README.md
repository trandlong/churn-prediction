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

conda install tensorflow-deps
conda install catboost numpy
conda install -c conda-forge pdpbox eli5
pip install -r requirements.txt
```