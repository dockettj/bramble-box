# bramble-box
I recently developed an interest in setting up a home lab to tinker with. I wanted a low cost solution to host some home automation tools, have a place to play with new pieces of software, and experiment with container management. There are some good tutorials out there, but none of them did what I wanted, or if they did, they failed to explain what was going on at each step, meaning I was just copying and pasting instead of actually learning. Enter the **Raspberry Pi Bramble Box** project. There are no commissions on this project, just a modern walkthrough that explains what is happening at each step.

[TODO] - Add photo

Parts List:
- 4x - [Raspberry Pi 4B 4GB](https://www.amazon.com/dp/B07TC2BK1X?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [Acrylic cluster case](https://www.amazon.com/dp/B07MW3GM1T?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [USB Power Station](https://www.amazon.com/dp/B00P936188?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 2x - [USB-A to USB-C cables (3 pack)](https://www.amazon.com/dp/B092ZS6SJG?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [USB to RJ45 connector](https://www.amazon.com/dp/B09GRL3VCN?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [USB to SATA cable](https://www.amazon.com/dp/B07F7WDZGT?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [500 GB 2.5" SSD](https://www.amazon.com/dp/B07XZLN9KM?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [Netgear 5 port managed POE switch](https://www.amazon.com/dp/B08LR18SC4?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [Cat6A cables (5 pack)](https://www.amazon.com/dp/B00HEM54DK?psc=1&ref=ppx_yo2ov_dt_b_product_details)
- 1x - [Mini HDMI to HDMI cable](https://www.amazon.com/dp/B08ZY3RR9X?psc=1&ref=ppx_yo2ov_dt_b_product_details)

**Total Cost:** $482.04

**Note:** This guide assumes you have two Micro SD cards (16gb minimum), a keyboard, and some sort of screen that accepts HDMI input. If you don't have those, you should add those to your list.

## Step 1 - Assembly

Physically building the device is pretty straight forward. Follow the guide that came with the case. 

For the fan wires: 
1. Hold the part of the Pi with the USB ports and RJ45 jack against you.
2. Find the GPIO (the two columns of pins on your right).
4. Plug the red wire into the pin one closer to you than the far right corner.
5. Plug the black wire into the pin one closer to you than the red wire.
   
I stacked the power brick as my bottom, then the SSD, then the cluster with the switch attached vertically and then bundled it all with some velcro straps. You can plug in all of your CAT6 cables now, but only run power to whichever Pi you want to have as your main (head) unit. I went with the bottom one. You should also connect the SSD, and HDMI to the same one.

## Step 2 - Setting Up the Head Unit

[TODO] - Screenshot of flash tool.
