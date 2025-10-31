HFMtDB
======
Overview
========
HFMtDB is a mitogenomes database for fungi of Hypocreales. <br>

数据结构
=======
```
HFMtDB/                                          # 仓库根目录
├── README.md                                    # 必选！数据库说明文档（核心导航，含目录、使用指南）
├── LICENSE                                      # 必选！开源许可（如 MIT 协议，明确数据使用、修改规则）
├── metadata/                                    # 元数据文件夹（存储所有样本的基础描述信息）
│   ├── mitogenomes_info.txt                     # 样本总表：包含物种名、样本ID、采集地、测序平台、数据版本等
│   └── reference.md                             # 引用文献/数据来源：记录原始数据发表文献、公共数据库 accession 号
├── mitogenomes_sequences/                       # 基因组序列文件夹（核心数据，存储 FASTA 格式线粒体序列）
│   └── Hypocreales/                             # 按目级类群分文件夹（此处为 Hypocreales 肉座菌目）
│       ├── Hypocreaceae/                        # 科级子文件夹（肉座菌科）
│       │   ├── Trichoderma_T069_mito.fa         # FASTA 格式：木霉菌属（Trichoderma）T069 菌株线粒体序列
│       │   └── Trichoderma_FJ059_mito.fa        # FASTA 格式：木霉菌属（Trichoderma）FJ059 菌株线粒体序列
│       └── Bionectriaceae/                      # 科级子文件夹（生赤壳科）
│           ├── [待补充物种]_mito.fa             # 预留：生赤壳科物种线粒体序列（FASTA 格式，需补充具体物种名）
│           └── [待补充物种]_mito.fa             # 预留：生赤壳科物种线粒体序列（FASTA 格式，需补充具体物种名）
├── mitogenomes_annotations/                     # 注释文件文件夹（存储基因位置、功能等注释信息）
│   ├── Hypocreaceae/                            # 科级子文件夹（对应肉座菌科序列的注释）
│   │   ├── Homo_sapiens_mt.gff                  # GFF 格式：基因结构注释（含外显子、内含子、启动子位置）
│   │   └── Homo_sapiens_mt.gbk                  # GenBank 格式：完整注释（含基因功能、碱基组成、ORF 信息）
│   └── Bionectriaceae/                          # 科级子文件夹（对应生赤壳科序列的注释，待补充文件）
└── scripts/                                     # 可选！辅助脚本文件夹（存储数据处理、格式转换工具）
    ├── fasta_format_check.py                    # Python 脚本：批量校验 FASTA 文件格式（避免序列截断、格式错误）
    ├── gff2gbk_convert.py                       # Python 脚本：将 GFF 注释文件批量转换为 GenBank 格式
    └── README.md                                # 脚本使用说明：含依赖库安装、运行命令、参数解释
```

Metadata
========


Mitogenomes_sequences
=====================


mitogenomes_annotations
=======================


Script
======
