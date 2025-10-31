HFMtDB
======
Overview
========
HFMtDB is a mitogenomes database for fungi of Hypocreales. <br>

数据结构
=======
HFMtDB/                                            # 仓库根目录<br>
├── README.md                                      # 必选！数据库说明文档（核心导航）<br>
├── LICENSE                                        # 必选！开源许可（如MIT，说明数据使用规则）<br>
├── metadata/                                      # 元数据文件夹（描述所有样本的基础信息）<br>
│   ├── mitogenomes_info.txt                            # 样本总表：物种名、样本ID、采集地、数据版本等<br>
│   └── reference.md                               # 引用文献/数据来源说明<br>
├── mitogenomes_sequences/                                     # 基因组序列文件夹（核心数据）<br>
│   └── Hypocreales/                               # 按类群分文件夹（如脊椎动物）<br>
│       ├── Hypocreaceae/                          # 肉座菌科<br>
│       │   ├Trichoderma_T069_mito.fa（FASTA格式）<br>
│       │   └Trichoderma_FJ059_mito.fa（FASTA格式）<br>
│       └── Bionectriaceae/                        # 生赤壳科<br>
│           ├<br>
│           └<br>
├── mitogenomes_annotations/                                   # 注释文件文件夹（可选，如基因位置、功能）<br>
│   ├── Hypocreaceae/<br>
│   │   ├── Hypocreaceae/Homo_sapiens_mt.gff       # GFF格式注释<br>
│   │   └── Homo_sapiens_mt.gbk                    # GenBank格式注释<br>
│   └── Bionectriaceae/<br>
└── scripts/                                       # 可选！辅助脚本（如批量处理、格式转换工具）<br>
    ├── 脚本.py<br>
    └── README.md       # 脚本使用说明<br>


