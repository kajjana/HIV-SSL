# Pre-training Strategy for Antiviral Drug Screening with Low-Data Graph Neural Network: A Case Study in HIV-1 K103N Reverse Transcriptase

### Kajjana Boonpalit,<sup>†,§</sup> Hathaichanok Chuntakaruk,<sup>‡,Fj,§</sup> Jiramet Kinchagawat,<sup>†</sup> Peter Wolschann,<sup>↓</sup> Supot Hannongbua,<sup>‡,↓↓</sup> Thanyada Rungrotmongkol,<sup>∗,‡,Fj</sup> and Sarana Nutanong<sup>∗,†</sup>

† School of Information Science and Technology, Vidyasirimedhi Institute of Science and Technology (VISTEC), Street, 21210, Rayong, Thailand

‡ Program in Bioinformatics and Computational Biology, Graduate School, Chulalongkorn University, Street, 10330, Bangkok, Thailand

Fj Center of Excellence in Structural and Computational Biology, Faculty of Science, Chulalongkorn University, Street, 10330, Bangkok, Thailand

↓ Department of Theoretical Chemistry, University of Vienna, Währinger Strasse 17, Vienna, 1090, Austria

↓↓ Center of Excellence in Computational Chemistry (CECC), Department of Chemistry, Faculty of Science, Chulalongkorn University, Bangkok 10330, Thailand

§ These two authors contributed equally to this work

E-mail: thanyada.r@chula.ac.th; snutanon@vistec.ac.th

![Git1](https://github.com/user-attachments/assets/cf85bef7-c8fc-47ea-952f-37831b26883f)



### This GitHub repository provides the datasets and models accompanying our manuscript. The code accompanying this work is taken from GitHub repository of Hu et. al. (https://github.com/snap-stanford/pretrain-gnns) and Wang et. al. (https://github.com/yuyangw/MolCLR). 

## Getting Started

### Installation

Set up conda environment and clone the github repo

```
# install requirements
$ pip install torch==1.7.1+cu110 torchvision==0.8.2+cu110 -f https://download.pytorch.org/whl/torch_stable.html
$ pip install torch-geometric==1.6.3 torch-sparse==0.6.9 torch-scatter==2.0.6 -f https://pytorch-geometric.com/whl/torch-1.7.0+cu110.html
$ pip install PyYAML
$ pip install tqdm
$ conda install -c conda-forge rdkit=2020.09.1.0
$ conda install -c conda-forge tensorboard
```

### Dataset

You can download the pre-training data and datasets used in the paper in `./Dataset`. The data for pre-training can be found in `pubchem-250K.txt`. The data for Wildtype RT dataset can be found in `WT_dataset.csv` and K103N variant dataset can be found in `K103N_dataset.csv`.