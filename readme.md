# 关于modular-2
modular-2 是一台基于cortex-M 处理器的模块化电脑，它由一块STM32F429 为主的主板和丰富的IO扩展板，网络扩展板，以及微型扩展模块构成。主板搭载Arm 公司Mbed OS 操作系统。该电脑功能比arduino 更强大，比树莓PI更方便地开发。该产品适用于快速开发小型智能设备，例如专用控制器，网关，大数据采集终端，物联网终端等。
## 特点
 **易学，不费力气可以学会大多数功能**  
设计modular-2时，我们受到了ardunio，树莓PI的启发，要设计一台初学者能够快速上手，有经验工程师得心应手的嵌入式设备。让使用者不费力气就可以使用大多数功能。其实ardunio已经达到了这个目的。事实上成千上万的学生使用arduino学习嵌入式程序设计和智能设备的开发。硬件工程师也使用这种廉价的电脑板搭试电路和产品原型。但是ardunio 只是一个AVR 8 位单片机为主的小电脑，处理能力还是十分有限，如果要使用到网络协议，SPI和复杂一点的程序就力不从心了。 
   市面上也出现了许多高性能的廉价单板电脑，比较出名的是树莓PI。最新的树莓PI3基于Cortex-A53 高性能处理器，使用linux操作系统。可以运行C++，Java python等各种开发环境，比较适合教育领域。但是我们觉得在linux下的设计嵌入式实时应用程序略显复杂。而且嵌入式工程师往往对linux 操作系统并不熟悉。 
 **可扩展，具有非常大的灵活性**
 modular-2 充分地采用了模块化设计理念，主板上设计了IO扩展总线和网络扩展总线，并且针对工业控制，数据采集，物联网，智能设备开发了丰富的IO模块和网络模块。多个modular-2既可以通过ethernet，wifi ，NB-iot，LoRa 网连接，也可以通过独特的EtherDiary 以太网级联网和Serial Diary 串口级联环网构成功能强大的分布式网络。 
 **直接开发出最终产品**
 芯片公司为了让工程师们评估他们的产品，开发了各种开发板。以前原厂的开发板都普遍比较贵，现在情况有了改善，像ST公司也提供低价格的开发板。使用他们来搭试产品的样机，或者评估还是可以的。不过几乎所有的各种开发板都有一个致命的缺点，开发板的接口，或者插针遍布PCB四面，无法作为最终产品递交和长期在工业环境使用。  
 ardunio ，树莓PI们给样机搭建带来了方便，但是它们并没有降低嵌入式设备开发的成本。当样机实验完成后，哪怕是交付10台设备，我们也需要从头再来，设计自己的硬件电路，PCB，设计目标MCU的程序，元器件采购，调试生产。这么漫长的研发制造过程。
 我们希望设计这么一台设备，用户可以针对具体的应用项目，通过少部份的二次开发，可以迅速地递交最终产品。 
**合理的价格**
## 设计理念
+1	基于Arm Cortex-M 系列处理器。 
+2	既可以作为样机搭试平台，又可以构成正式产品的一部分交付。 
+3	面向专业应用，配备外壳，工业级接插件。适合工业环境长期使用。 
+4	模块化设计理念，用户可以扩展I/O接口板，网络接口板，M2-Node模块。融入自己的技术和知识产权。 
+5	可以通过网络互连，扩展功能。 
+6	易学习，不费力可以学会90%的功能。 
+7	功能确定性，没有是是而非的东西，让用户丈二和尚摸不着头脑。 

## 主板
Modular-2的主板以一个ST公司Cortex-M系列单片机为主的构成电路板。
主板的基本特性如下： 
+1  144Pin 的SOC。 
+2  DAP-Link 模块用于程序下载，调试。 
+3  OTG USB接口。 
+4  Ethernet接口。 
+5  SD卡座。 
+6  EEPROM。 
+7  2.5V 模拟参考电压。 
+8  72 线I/O 扩展板总线(我们称为PinBUS 总线)插座.  
+9  22线网路扩展板总线。  
+10 一个Pwer/Comm 接口插座。 

## I/O 接口板
## 网络模块
## 微型节点

