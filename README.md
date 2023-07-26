# Power6 vs. Power9
-----

the reason for this, is because A-EON X5000 board with P5020 | P5040 CPU, </br>
has become outdated. </br>
Old P-CPUs: </br>
Power5 e5500 45nm No-Altivec 2|4-cores PCIe v2.0 "2005-2010 technology" </br>

The idea is to make an Open Board for New T-CPUs, dual Boot Firmware: CHRP and U-Boot, like [Fienix](https://fienixppc.blogspot.com/p/download.html), [About](https://fienixppc.blogspot.com/p/blog-page.html). </br>
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

[Power9](https://en.wikipedia.org/wiki/POWER9) 14nm Sforza 512KiB L2 2017 technology "Big L3 | small L2". </br>
has 3x Boards, Ready to Run. </br>

Problem with most modern Boards, </br>
is that CPU pins, Sockets Made in China are designed to fail, </br>
metal is brittle, did Not happened with older boards X58. </br>

DIY board can be: </br>
soldered CPU 2000 solder balls, or </br>
custom socket, No off the shelf part. </br>
DIY socket could be like some Fine Stylus tips, </br>
with spring tip, like a [Pentium4 478 socket](https://en.wikipedia.org/wiki/Pentium_4#/media/File:Pentium_4_-_SL5TK_-_pin_side-3057.jpg) but backwards, Pins on board, </br>
like [AMD Ryzen](https://en.wikipedia.org/wiki/Ryzen#/media/File:AMD_Ryzen_7_3700X_pins_IMGP3168_smial_wp.jpg), but backwards, pins on board, and  must have springs 5mm tolerance. </br>
Balls are 1mm pitch, a DIY Socket will solve a lot of soldering issues,  </br>
and will create a used CPU market, making easier for late adopters to get-in, </br>
but diy socket will increase price. </br>
other sollution can be like older PowerMac, Amiga 4k or [Pentium-II](https://en.wikipedia.org/wiki/Pentium_II) "CPU cards with PCI connector", </br>
easier than DIY socket, CPU soldered to a small PCB, can be swaped by user very easy. </br>
2Ghz may require surface mount PCIe connector, Not Though Hole, </br>
and a metallic bracket / retention mechanism / support, like gamer boards. </br>
small CPU PCB can have standard Heatsink / waterblock mounting holes. </br>
1x CPU PCIe for Vertical L. "Cost Reduced" </br>
2x PCIe for Horizontal = similar to Atmel STK600 mcu & routing cards. </br> 

The idea is to make an ATX board, compatible with many cases, </br>
similar to NXP dev board, but cost reduced. </br>
different versions: with so-dimm "laptop" ddr3, with standard full size "Desktop" ddr3 </br>
ddr can also be a PCIe module, user can swap. </br> 
with cheap 1Gbe Ethernet, with Better 1x SFP+ 10G cage, NXP recomended IC or common Marvell Aquantia AC100 [Sonnet](https://www.sonnettech.com/product/solo10g-sfp-pcie-card.html), Asus XG-C100F, etc.. </br>
with CPU SATA-II 3Gbps, with faster SATA-III 6Gbps like [Sonnet Tempo SSD to PCIe card](https://www.sonnettech.com/product/tempossd.html) </br>
or nothing, just PCIe slots, </br>
maybe with PCI to PCIe bridge "there are 4 different IC brands", </br> 
some old PCI cards like Digi001 have issues with X58 PCI, but work ok with older 975x boards. </br>
and/or NVMe U-Boot drivers, PCIe v2.0 is limited to 1600MB/s, PCIe v3.0 2500MB/s, PCIe v4.0 >5000MB/s </br>
some PCIe to NVMe cards: [Ableconn](http://www.ableconn.com/products_2.php?gid=143), [Startech](https://www.startech.com/en-us/hdd/pex8m2e2), [Sonnet](https://www.sonnettech.com/product/computer-cards/cards.html), [Areca](https://www.areca.com.tw/products/nvme-1886.html), [HighPoint](https://www.highpoint-tech.com/nvme1/ssd7540),  </br>
have a Bifurcation IC, that allows 2500MB/s in PCIe v2.0, 5000MB/s in PCIe v3.0. </br>

[RaptorComputerSystems](https://www.raptorcs.com/content/base/products.html) </br>
Boards: </br>
Talos-II </br>
Talos-I </br>
Backbird </br>

CPUs: </br>
Power9 22-core $4962usd. | $226usd. per core. </br>
Power9 18-core $2634usd. | $147usd. per core. </br>
Power9 8-core  $1366usd. | $171usd. per core. </br>
Power9 4-core  $945usd.  | $237usd. per core. </br>
Average price per core $195usd.</br>

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
Power9 22-core $5197usd. | $237usd. </br>
Power9 18-core $4252usd. | $237usd. </br>
Power9 8-core  $1890usd.   | $237usd. </br>
Power9 4-core  $945usd.    | $237usd. </br>
Lowest price per core: </br>
Power9 22-core $3220usd. | $147usd. </br>
Power9 18-core $2634usd. | $147usd. </br>
Power9 8-core  $1171usd. | $147usd. </br>
Power9 4-core  $586usd.  | $147usd. </br>

having a lower price per core requires purchasing very large quantity. </br>
REQUIRES GoFundME or similar. </br>

Power6 12-core 1.8Ghz T4240 CPU is aprox. $1600usd. | $133usd. per core, </br>
purchasing [1 unit](https://www.digikey.com/en/products/filter/embedded/microprocessors/694?s=N4IgjCBcoLQExVAYygFwE4FcCmAaEA9lANogCsIAugL7X4KSmoAsczADFfgGyIgCWAEyggYYdhHwAHVCJD5UATynYRggM4paQA) shipping in 5 days. </br>
Mouser has $1500 | $125usd. 18 week wait, minimum 12 units. </br>
The idea is a GoFundMe to purchase 108 or more, as much units as possible, to lower price as much as possible. </br>
Top of the Line 1.8Ghz 12-core model 3x ddr3 channels.</br>
[Mouser T4240 1.8Ghz](https://www.mouser.com/c/semiconductors/embedded-processors-controllers/microprocessors-mpu/?q=t4240&maximum%20clock%20frequency=1.8%20GHz) </br>
crypto disabled:
[T4240NSN7TTB](https://www.mouser.com/ProductDetail/NXP-Semiconductors/T4240NSN7TTB?qs=S0GpHP26UDLUtFS5%2Fv05eg%3D%3D)
crypto enabled:
[T4240NSE7TTB](https://www.mouser.com/ProductDetail/NXP-Semiconductors/T4240NSE7TTB?qs=S0GpHP26UDJXBDeHcjIYrQ%3D%3D)

Top of the Line 1.8Ghz 8-core model 2x ddr3 channels.</br>
[Mouser T4160 1.8GHz](https://www.mouser.com/c/semiconductors/embedded-processors-controllers/microprocessors-mpu/?maximum%20clock%20frequency=1.8%20GHz&number%20of%20cores=8%20Core&package%20%2F%20case=FC-PBGA-1932&series=T4160)</br>
crypto disabled: [T4160NSN7TTB](https://www.mouser.com/ProductDetail/NXP-Semiconductors/T4160NSN7TTB?qs=S0GpHP26UDKkFx%2FAj3ZSbQ%3D%3D)
cryprto enabled: [T4160NSE7TTB](https://www.mouser.com/ProductDetail/NXP-Semiconductors/T4160NSE7TTB?qs=S0GpHP26UDLLO6WoSz3UfA%3D%3D)</br>
$1100 - $1200usd. | $137usd. $150usd. aprox.</br>

Lowest price possible 1.5Ghz 4-core [T4080](https://www.mouser.com/c/semiconductors/embedded-processors-controllers/microprocessors-mpu/?number%20of%20cores=4%20Core&package%20%2F%20case=FC-PBGA-1932&sort=pricing)</br>
[T4080NSN7PQB](https://www.mouser.com/ProductDetail/NXP-Semiconductors/T4080NSN7PQB?qs=nr7BunVhf4pFB%252BS4fJptRg%3D%3D)</br>
$573usd. | $143usd. aprox. </br>
$682usd | $170usd. [5 day](https://www.digikey.com/en/products/filter/embedded/microprocessors/694?s=N4IgjCBcoLQExVAYygFwE4FcCmAaEA9lANogCsIAugL7X4KSmoAsADABytX4BsiIASwAmUEDDCsI%2BAA6pRIfKgCe07KICGAZxS0gA) shipping.
