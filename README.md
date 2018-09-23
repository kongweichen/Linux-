# **运维第一周--来自小白的总结**

**前言**  
&ensp;&ensp;&ensp;&ensp;作为一个接近0基础的小白，来马哥培训学习运维课程已经接近一周了，接触了计算机和运维的知识，也碰到了一些困难。把自己学的部分知识进行总结，期待更好的自己。

## 计算机基础知识  
**计算机系统组成**  
&ensp;&ensp;&ensp;&ensp;由俗称的硬件（hardware）和软件（software）两部分所组成。

![d](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1537696057206&di=78fc58614ccba668b37a667ce9ecd75d&imgtype=0&src=http%3A%2F%2Fpic.baike.soso.com%2Fp%2F20140128%2F20140128124253-330428729.jpg)

**计算机硬件组成——冯诺依曼体系结构**  

&ensp;&ensp;&ensp;&ensp;1946年冯诺依曼提出的计算机硬件系统的组成结构
![a](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1537696641214&di=57047313a235ccdee44abda0457ae69b&imgtype=0&src=http%3A%2F%2Fimage.mamicode.com%2Finfo%2F201803%2F20180331162132591281.png)

&ensp;&ensp;&ensp;&ensp;接触运维，必然离不开服务器，服务器的硬件部分遵循冯诺依曼体系结构，但和普通的计算机又有所不同  
### 服务器硬件——CPU  
&ensp;&ensp;&ensp;&ensp;CPU由运算器和控制器组成，服务器中最重要的组成部分。目前企业用的服务器中，CPU主要品牌为英特尔旗下的 ***Xeon系列*** （使用很广）和IBM公司的 ***Power系列***（性能强悍但价格昂贵）  
&ensp;&ensp;&ensp;&ensp;CPU体系架构来分，服务器主要两类：  
&ensp;&ensp;&ensp;&ensp;x86服务器 ，又称 **CISC（复杂指令集）** 架构服务器；即通常所讲的PC服务器，它是基于PC机体系结构，使用Intel或其它兼容x86指令集的处理器芯片和Windows操作系统的服务器；价格便宜、兼容性好、稳定性较差、安全性不算太高，主要用在中小企业和非关键业务中。  
&ensp;&ensp;&ensp;&ensp;非x86服务器：包括大型机、小型机和UNIX服务器，它们是使用 **RISC（精简指令集）或EPIC（并行指令代码）** 处理器，并且主要采用UNIX和其它专用操作系统的服务器，精简指令集处理器主要有IBM公司的POWER和PowerPC处理器，SUN与富士通公司合作研发的SPARC处理器、EPIC处理器主要是Intel研发的安腾处理器等。这种服务器价格昂贵，体系封闭，但是稳定性好，性能强，主要用在金融、电信等大型企业的核心系统中。

### 服务器硬件——主板

ensp;&ensp;&ensp;&ensp;主机板(mainboard)，又叫系统板(systemboard)或母板(motherboard)。它安装在机箱内，是服务器最基本的也是最重要的部件之一。主板一般为矩形电路板，上面安装了组成计算机的主要电路系统，一般有BIOS芯片、I/O控制芯片、键和面板控制开关接口、指示灯插接件、扩充插槽、主板及插卡的直流电源供电接插件等元件。

### 服务器硬件——内存

ensp;&ensp;&ensp;&ensp;内存(Memory)也被称为内存储器，其作用是用于暂时存放CPU中的运算数据，以及与硬盘等外部存储器交换的数据。内存是计算机中重要的部件之一，它是与CPU进行沟通的桥梁，因此内存的性能对计算机的影响非常大。  
**内存带宽** ：内存与北桥芯片之间的数据传输率  
** 内存带宽=内存总线频率*数据总线位数/8

ensp;&ensp;&ensp;&ensp;外存目前主要指硬盘,主要分为机械硬盘和SSD固态硬盘两类。  
**容量** 是硬盘最主要的参数，单位有MB,GB,TB  
**硬盘接口类型** 主要有IDE/SCSI/SATA/SAS等接口类型，目前主流的硬盘接口类型为 **SATA和SAS**
接口  
机械硬盘与固态硬盘：机械硬盘价格比较低，但是读写速率相对较低，影响了服务器性能的提升，因而催生了固态硬盘，固态硬盘读写效率高、性能稳定、故障率低，但是价格也非常昂贵，基本没有性价比。

**内存与外存的区别**  
  内存在断电后会数据丢失  
  外存断电后数据可以保存

### 服务器其他硬件 ——阵列卡（Raid卡）、显卡、网卡、电源、热插拔、机柜等等

**小结**  
&ensp;&ensp;&ensp;&ensp;小白一枚，初次总结多有不足。但随着技能的熟练和知识的积累，会越来越完善的。从来没有什么救世主，知识要通过努力才能掌握。  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;——致努力生活的人们
