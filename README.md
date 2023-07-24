# Power6 vs. Power9
-----

the reason for this, is because A-EON X5000 board with P5020 | P5040 CPU, </br>
has become outdated. </br>
Old P-CPUs: </br>
Power5 e5500 45nm No-Altivec 2/4-cores 2Ghz PCIe v2.0 "2005-2010 technology" </br>

The idea is to make an Open Board for New T-CPUs, dual Boot Firmware: PREP and U-Boot. </br>
T-CPUs: </br>
Power6 e6500 28nm Altivec ddr3-1600 </br>
4/8/12-cores, 2-Threads per core, 1.8Ghz/1.6Ghz/1.5Ghz </br>
2x PCIe v3.0 + 2x PCIe 2.0, 3x memory channels in 12-core model. </br>
Big.Endian </br>
vs. </br>
Power9v2 4/8/18/22-cores 4-threads per core, PCIe v4.0 ddr4-ecc </br>
Bi-Endian, but most Linux distros are little.endiam. </br>

All comes down to Price. </br>
¿is worth a DIY Power6 today? </br>
Power6 has No Board, DIY. KiCAD, Target3001!, Eagle, etc... </br>
NXP Development Board is Crazy Expensive >$4500-$6000usd.BTO </br>
comes with too much all-in-one 4x different Network adapters, etc... </br>

Power9 has 3x Boards, Ready to Run. </br>

Problem with most modern Boards, </br>
is that CPU pins, Sockets Made in China are designed to fail, </br>
metal is brittle, did Not happened with older boards X58. </br>

DIY board can be: </br>
soldered CPU 2000 solder balls, or </br>
custom socket, No off the shelf part. </br>
DIY socket could be like some Fine Stylus tips, </br>
with spring tip, like a Pentium4 CPU soocket but backwards, Pins on board, </br>
like AMD Ryzem, but backwards, pins on board, but must have springs 5mm tolerance. </br>
Balls are 1mm pitch, a DIY Socket will solve a lot of soldering issues,  </br>
and will create a used CPU market, making easier for late adopters to get-in, </br>
but diy socket will increase price. </br>
other sollution can be like older PowerMac, Amiga or Pentium-II "CPU cards with PCI connector", </br>
easier than DIY socket. </br>

The idea is to make an ATX board, similar to NXP dev board, but cost reduced. </br>
different versions: with so-dimm ddr3, with standard full size ddr3 </br>
with cheap 1Gbe Ethernet, with Better 1x SFP+ 10G cage, </br>
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
