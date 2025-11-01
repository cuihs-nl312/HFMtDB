HFMtDB
======

# Overview

**`HFMtDB`** is a comprehensive mitochondrial genome database of Hypocreales Fungi. As a group with high species diversity and unique evolutionary characteristics in the phylum Ascomycota, Hypocreales plays a crucial role in multiple fields, including material cycling in ecosystems, agricultural production, pharmaceutical research and development, and the study of fungal evolutionary mechanisms. This study integrated the mitochondrial genome data of nearly a thousand strains from **`11 families`** of Hypocreales. At the same time, genome assembly was also performed on some species without mitochondrial genomes.<br>

# Data Structure
```
HFMtDB/                                          # 数据库根目录
├── README.md                                    # 数据库说明文档（核心导航，含目录、使用指南）
├── LICENSE                                      # 开源许可（如 MIT 协议，明确数据使用、修改规则）
├── metadata/                                    # 元数据文件夹（存储所有样本的基础描述信息）
│   ├── mitogenomes_info.txt                     # 样本总表：包含物种名、样本ID、采集地、测序平台、数据版本等
│   └── reference.md                             # 引用文献/数据来源：记录原始数据发表文献、公共数据库 accession 号
├── mitogenomes_sequences/                       # 基因组序列文件夹（核心数据，存储 FASTA 格式线粒体序列）
│   ├── Bionectriaceae/                          # 科级子文件夹（生赤壳科）
│   │   ├── Trichoderma_T069_mito.fa             # FASTA 格式：木霉菌属（Trichoderma）T069 菌株线粒体序列
│   │   └── Trichoderma_FJ059_mito.fa            # FASTA 格式：木霉菌属（Trichoderma）FJ059 菌株线粒体序列
│   └── Clavicipitaceae/                         # 科级子文件夹（肉座菌科）
│   ├── Cordycipitaceae/
│   ├── Hypocreaceae/
│   ├── Nectriaceae/
│   ├── Niessliaceae/
│   ├── Ophiocordycipitaceae/
│   ├── Pseudodiploosporaceae/
│   ├── Sarocladiaceae/
│   ├── Stcahybotriaceae/
│   ├── 
├── mitogenomes_annotations/                     # 注释文件文件夹（存储基因位置、功能等注释信息）
│   ├── Hypocreaceae/                            # 科级子文件夹（对应肉座菌科序列的注释）
│   │   ├── Homo_sapiens_mt.gff                  # GFF 格式：基因结构注释（含外显子、内含子、启动子位置）
│   │   └── Homo_sapiens_mt.gbk                  # GenBank 格式：完整注释（含基因功能、碱基组成、ORF 信息）
│   └── Bionectriaceae/                          # 科级子文件夹（对应生赤壳科序列的注释，待补充文件）
│   ├──
│   ├──
│   ├──
│   ├──
│   ├──
│   ├──
└── scripts/                                     # 辅助脚本文件夹（存储数据处理、格式转换工具）
    ├── fasta_format_check.py                    # Python 脚本：批量校验 FASTA 文件格式（避免序列截断、格式错误）
    ├── gff2gbk_convert.py                       # Python 脚本：将 GFF 注释文件批量转换为 GenBank 格式
    └── README.md                                # 脚本使用说明：含依赖库安装、运行命令、参数解释
```
# How to download HFMtDB?
## Windows Download
  Go to the HFMtDB page on GitHub. Click the `Code` button on the page, then select `Download Zip`. All data from HFMtDB will then be downloaded to your computer.
  
## Linux Download
  Use the following code in the Linux command line. HFMtDB will be downloaded to the Linux directory.
```
git clone https://github.com/cuihs-nl312/HFMtDB.git
```

# Metadata
  Metadata包含所有样本的基础描述信息，这里我们使用表格文件`Hypocreales_mitogenomes_infor.txt`来展示所有物种线粒体基因组的基础信息。具体信息如下
| Family | Species | Strain | Abb | Accession | Mitogenome Size (bp) | Complete (Y/N) |Reference | Note. |
| --- | :---: | :---: |  :---: |  :---: |  :---: | :---: | :---: | ---: |
| Hypocreaceae | Trichoderma breve | T069 | HyTbT069 | PP933710.1 | 26285 | Y | https://doi.org/10.3390/ijms252212140 |-- |

# Mitogenomes_sequences
  In the Mitogenomes_sequences directory, mitochondrial genome sequence data of 11 families belonging to Hypocreales are presented. The mitochondrial genome data of each family is stored in a separate folder named after the family. The mitochondrial genome data of each strain is presented as an individual FASTA-formatted file, with the filename containing the species name and strain name.

# Mitogenomes_annotations
  In the Mitogenomes_annotation directory, the annotation data of mitochondrial genomes from 11 families of Hypocreales are presented. The mitochondrial genome annotation results for each family are stored in a separate folder named after the family. The mitochondrial genome annotation result of each strain is presented as an individual `.txt` file, with the filename containing the species name and strain name.

# Script

