# Power6 vs. Power9
-----

the reason for this, is because A-EON X5000 board with P5020 | P5040 CPU, </br>
has become outdated. </br>
Old P-CPUs: </br>
Power5 e5500 45nm No-Altivec 2|4-cores PCIe v2.0 "2005-2010 technology" </br>

The idea is to make an Open Board for New T-CPUs, dual Boot Firmware: PREP and U-Boot. </br>
T-CPUs: </br>
Power6 e6500 28nm Altivec ddr3-1600 </br>
4|8|12-cores, 2-Threads per core, 1.8Ghz/1.6Ghz/1.5Ghz </br>
2x PCIe v3.0 + 2x PCIe 2.0, 3x memory channels in 12-core model. </br>
Big.Endian </br>
vs. </br>
Power9v2 4|8|18|22-cores 4-threads per core, PCIe v4.0 ddr4-ecc </br>
Bi-Endian, but most Linux distros are little.endiam. </br>

All comes down to Price. </br>
¿is worth a DIY Power6 today? </br>
Power6 has No Board, DIY. KiCAD, Target3001!, Eagle, etc... </br>
NXP Development Board is Crazy Expensive >$4500-$6000usd.BTO </br>
comes with too much all-in-one, 4x different Network adapters, etc... </br>
[Power6](https://www.nxp.com/products/processors-and-microcontrollers/power-architecture/qoriq-communication-processors/t-series/qoriq-t4240-t4160-t4080-multicore-communications-processors:T4240) 28nm similar to Intel & AMD 2013-2015 technology, [Steamroller](https://en.wikipedia.org/wiki/Steamroller_(microarchitecture)), [Excavator](https://en.wikipedia.org/wiki/Excavator_(microarchitecture)), [Puma](https://en.wikipedia.org/wiki/Puma_(microarchitecture)), [Jaguar](https://en.wikipedia.org/wiki/Jaguar_(microarchitecture)) </br>
2MB L2 cache. </br>

[Power9](https://en.wikipedia.org/wiki/POWER9) Sforza 14nm 512KiB L2 2017 technology. </br>
has 3x Boards, Ready to Run. </br>

Problem with most modern Boards, </br>
is that CPU pins, Sockets Made in China are designed to fail, </br>
metal is brittle, and did Not happened with older boards X58. </br>

DIY board can be: </br>
soldered CPU 2000 solder balls, or </br>
custom socket, No off the shelf part. </br>
DIY socket could be like some Fine Stylus tips, </br>
with spring tip, like a [Pentium4 478 socket](https://en.wikipedia.org/wiki/Pentium_4#/media/File:Pentium_4_-_SL5TK_-_pin_side-3057.jpg) but backwards, Pins on board, </br>
like [AMD Ryzem](https://en.wikipedia.org/wiki/Ryzen#/media/File:AMD_Ryzen_7_3700X_pins_IMGP3168_smial_wp.jpg), but backwards, pins on board, and  must have springs 5mm tolerance. </br>
Balls are 1mm pitch, a DIY Socket will solve a lot of soldering issues,  </br>
and will create a used CPU market, making easier for late adopters to get-in, </br>
but diy socket will increase price. </br>
other sollution can be like older PowerMac, Amiga 4k or [Pentium-II](https://en.wikipedia.org/wiki/Pentium_II) "CPU cards with PCI connector", </br>
easier than DIY socket, CPU soldered to a small PCB, can be swaped by user very easy. </br>
2Ghz may require surface mount PCIe connector, Not Though Hole, </br>
and a metallic bracket / retention mechanism / support, like gamer boards. </br>
small CPU PCB can have standard Heatsink / waterblock mounting holes. </br>

The idea is to make an ATX board, similar to NXP dev board, but cost reduced. </br>
different versions: with so-dimm ddr3, with standard full size ddr3 </br>
with cheap 1Gbe Ethernet, with Better 1x SFP+ 10G cage, </br>
instead of CPU SATA-II 3Gbps, faster SATA-III 6Gbps to PCIe like [Sonnet Temp SSD to PCIe card](https://www.sonnettech.com/product/tempossd.html) </br>
or nothing, just PCIe slots, </br>
maybe PCI to PCIe "there are 4 different IC brands", </br> some old PCI cards like Digi001 have issues with X58 PCI bridge, but work ok n 975x. </br>
and/or NVMe U-Boot drivers </br>
Not all in 1 board. </br>

RaptorComputerSystems https://www.raptorcs.com/content/base/products.html </br>
Boards: </br>
Talos-II </br>
Talos-I </br>
Backbird </br>

CPUs: </br>
Power9 22-core $4962usd. | $225.55usd. per core. </br>
Power9 18-core $2634usd. | $146.33usd. per core. </br>
Power9 8-core  $1366usd. | $170.75usd. per core. </br>
Power9 4-core  $945usd.  | $236.25usd. per core. </br>

2x CPU board TL2MB1: </br>
$4050usd. = $2025usd. per cpu </br>
EATX, 3x PCIe x16 + 2x PCIe x8, 16x DDR4 ECC Slots. </br>
BMC-VGA </br>
 
2x CPU 1-socket unpopulated / Cost Reduced TL1MB1: </br>
https://www.raptorcs.com/content/TL1MB1/intro.html </br>
$2460usd. per CPU. </br>
EATX, 1x PCIe x16 + 1x PCIe x8, 8x DDR4 ECC Slots. </br>
BMC-VGA </br>

Single / Cost Reduced CPU board BK1MB1: </br>
https://www.raptorcs.com/content/BK1MB1/intro.html </br>
$2063usd. per CPU. </br>
8-core max, 1x PCIe x16 + 1x PCIe x8, 2x DDR4 ECC Slots. </br>
BMC-HDMI </br>

Purchasing different quantity of processors </br>
gives discrepancy in price per core. </br>

IF purchasing quantity were optimized for same price per core, </br>
Higest price per core: </br>
Power9 22-core $5197.5usd. | $236.25usd. </br>
Power9 18-core $4252.5usd. | $236.25usd. </br>
Power9 8-core  $1890usd.   | $236.25usd. </br>
Power9 4-core  $945usd.    | $236.25usd. </br>
Lowest price per core: </br>
Power9 22-core $3220usd. | $146.33usd. </br>
Power9 18-core $2634usd. | $146.33usd. </br>
Power9 8-core  $1171usd. | $146.33usd. </br>
Power9 4-core  $586usd.  | $146.33usd. </br>

having a lower price per core requires purchasing very large quantity. </br>
