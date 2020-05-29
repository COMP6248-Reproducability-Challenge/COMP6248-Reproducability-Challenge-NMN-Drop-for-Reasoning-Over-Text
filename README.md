### This repository correspons to the COMP6248-Reproducability-Challenge (2019-2020), and the reproduction report to the NMN-Drop for reasoning over the text.

Zhongxin Xie*, Ming Xiong, Siyuan Liu

Department of Electronic and Computer Science 

University of Southampton

Southampton, England SO17 1BJ

E-mail: (zx4a19, mx2n19, sl18n19) @soton.ac.uk

```
# Make conda environment
conda create -name nmn-drop python=3.6
conda activate nmn-drop

# Install required packages
pip install allennlp==0.9
pip install dateparser==0.7.2
python -m spacy download en_core_web_lg

# Clone code and make symlinks
git clone git@github.com:nitishgupta/nmn-drop.git
cd nmn-drop/
mkdir resources; cd resources; ln -s MODEL_CKPT_PATH/iclr_cameraready ./; cd ..    
ln -s PATH_TO_allennlp-semparse/allennlp-semparse/allennlp_semparse/ ./ 
```
