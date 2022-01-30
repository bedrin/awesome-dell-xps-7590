# Awesome Dell XPS
Tips to improve your experience with Dell XPS 7590 and other Dell laptops.

Disclaimer: all these instructions are written for Dell Vostro 7590 which is (almost) sharing the chassis with Dell XPS 7590 and Dell Inspiron 15 7000. Repository name says XPS for clickbait reasons since it's a much more popular model. Most (if not all) instructions are applicable for Dell XPS 7590 and many other Dell models as well.

# XPS vs Vostro vs Inspiron

https://www.dell.com/support/manuals/en-us/xps-15-7590-laptop/xps-15-7590-setup-and-specifications/dimensions-and-weight?guid=guid-7df32f47-45cf-4a08-ad99-b01eec4f3ce6&lang=en-us
https://www.dell.com/support/manuals/en-us/vostro-15-7590-laptop/vos7590_setupspecs/dimensions-and-weight?guid=guid-5c33f917-293a-4bb4-a06c-f72cc5f41548&lang=en-us
https://www.dell.com/support/manuals/en-us/inspiron-15-7590-laptop/inspiron-7590-setup-and-specifications/dimensions-and-weight?guid=guid-7df32f47-45cf-4a08-ad99-b01eec4f3ce6&lang=en-us

# Configuration

Make sure to choose option without HDD - it comes with big battery

# Upgrades

Dell provides great instructions on assembly/disassembly: https://dl.dell.com/topicspdf/vostro-15-7590-laptop_owners-manual_en-us.pdf
You can upgrade storage (2 slots M.2 2280 PCIe Gen 3.0x4 NVMe, up to 32 Gbps, no limit on capacity), memory (2 slots SODIMM DDR4 2666 MHz up to 64Gb), wireless module (1 slot M.2 2230, upgradeable to WiFi 6E and beyond)

## Storage

Since only PCIe Gen 3 is supported, there's no need to invest into Gen4+ SSDs.
Ideal SSD must have speed close to PCIe Gen3 saturation and be efficient in terms of temperature and power consumption.

Good choise: SK Hynix Gold P31 (up to 2Tb) - https://ssd.skhynix.com/gold_p31/

RAID-0 while possible won't give you any speed improvements due to saturation of PCIe bus as well - https://www.youtube.com/watch?v=DWBvDt96ZTc

## Memory

Even if Dell states that 64Gb is only supported on certain models, in fact it does work not only on XPS series but also on Inspiron / Vostro series.

DDR4 SO-DIMM 2666 MHz is supported.
Any casual CL19 memory would work, however you will face issues with low-latency "gaming" memory.
For example Patriot Viper Steel memory with timings 18-18-18-43 would not work, while Corsair Vengeance with timings 18-19-19-39 will work just fine.
If you want to squeeze maximum performance out of your laptop, check carefully if memory would work and make sure you can return it if not.

People on reddit collated a table of supported RAM for the 9570 (previous) generation: https://www.reddit.com/r/Dell/comments/8r55ys/9570_working_ram_kits/

## Wireless

Update to WiFi 6 is possible. No details yet

# BIOS

While addressing certain security issues, most recent BIOS updates disable undervolting.
Make sure you're using BIOS version 1.5.1 if you want to do undervolting.

# Links
1. https://www.youtube.com/playlist?list=PLwkH-8urcGm6rxc99tk75eZq_veJe0SUq
2. https://github.com/AaronKelley/DellFanManagement
3. https://www.dell.com/support/home/en-uk/product-support/product/vostro-15-7590-laptop/docs
4. https://ark.intel.com/content/www/us/en/ark/products/191045/intel-core-i79750h-processor-12m-cache-up-to-4-50-ghz.html
