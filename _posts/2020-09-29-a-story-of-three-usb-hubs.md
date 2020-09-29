---
title: "A Story of ~~One~~ Three USB-C Hubs"
categories:
  - blog
tags:
  - Hardware
  - Review
---

I recently received a 16" MacBook Pro for work. Shiny as it may be, it only features four USB-C sockets (and a headphone jack) to connect to the outside world. To not end up in adapter hell, I ordered ~~one~~ three USB-C hubs until I finally found one that worked. This is my review and the story behind.

![Not one of the hubs I ended up buying, but close enough.](/assets/posts/2020-09-29-usbc_hub.jpg)

My specifications seemed (to me) modest: The hub should support 100W charging (since the 2019 MacBook Pro needs it), HDMI (for ergonomic reasons, I like to stay perfectly centered in front of my display, so I only need one video out; if you need two, or worse, two at 4K, welcome to adapter hell!), Ethernet, and a couple of type-A USB ports so I can plug-in my wireless mouse, keyboard, and other equipment.

When I started my quest, I was quite delighted to see that from around 20$, one could get USB-C hubs that effectively mirror the capabilities of docking stations of old. Something that in the pre-USB 3 era would have cost upward of 200 bucks, was now finally within reach: plug in one cable at ~~work~~ your desk and be done with it. Moreover, most of these devices are small, stylish aluminum devices that resemble the MacBook's elegance perfectly.

> It is astonishingly difficult to get a USB-C adapter hub that just works

Disappointment settled in quickly when I tried to sift-through the dozens of near-identical hubs on Amazon, many of which seem to have fake reviews: how does on even make a decision among those end- and nameless brands? So, I just started ordering adapters with the highest rating I could find, half-cosher reviews, and only the features I needed (I figured if they had more at the same price, that would naturally be detrimental to the performance of the adapter).

## [AUKEY USB C Hub 8 in 1](https://smile.amazon.de/gp/product/B07WNTM6MD/ref=ppx_yo_dt_b_asin_title_o07_s00?ie=UTF8&psc=1), 4.5 star rating (42.99 €)
I bought the AUKEY USB C Hub 8 in 1, since it explicitly mentioned its 100 Watt and MacBook Pro compatibility. Big fail. The adapter not only cut power delivery to the MacBook every 30 or so seconds (complete with annoying MacOS sounds notifying you of the same), it also got hot enough to melt a near-by chocolate bar. Moreover, it had a high static. Lastly, its electromagnetic shielding was so poor that the only way I could get my Logitech nano receiver to work was by placing it on a leash-like USB extension cable. Otherwise, the cursor would uncontrollably jump from one corner to the other. I don't know whether the adapter caused WIFI performance issues, but given its unshielded nature, I suspect so.

## [YXwin USB C Hub, 6 in 1 Type C USB C Adapter](https://smile.amazon.de/gp/product/B07PSM6RQS/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&psc=1), 4.5 star rating (34.99 €)
The ominously named YXwin USB C Hub was also a fail, but on a more subtle level. At first, it seemed to do quite well: Power delivery was constant and the hub did not become too hot. Of course, electromagnetic shielding was also poor (or non-existent) so I couldn't get my nano receiver off its leash just yet. But otherwise, I was quite happy and used it for a couple weeks in different environments. Until I noticed that my WIFI connection was slower and sometimes laggier than it should be. After two hours of playing around with the local WIFI installation, I finally zoomed-in on the culprit USB C hub. I found that the electromagnetic shielding of this hub was so bad that my WIFI's speed (measured at 100 MBbit/s at the same spot with the peripheral-free MacBook) drop down to
- below 2 Mbit/s when the adapter was used with HDMI and power simultaneously
- a very jerky 15 Mbit/s when the adapter was used with HDMI.

## [VAVA USB Hub, 8-in-1 USB C Hub](https://smile.amazon.de/gp/product/B08BNQLRTG/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1), 4.5 star rating (31.99 €, normally 39.99 €)
I just got this today. Everything works and it doesn't make annoying noises. I don't even need the USB leash, but can just directly plug-in my Logitech nano receiver, which indicates that the electromagnetic shielding is good.  Even though there is a warning on the device that it can get extremely hot (130° Fahrenheit, that's 54°C), it actually does not. Now here is a caveat: There are a few Amazon reviews of customers whose units failed after only a few months. Should this happen, I will update this blog post. If I have not, it still works happily.

Two conclusions: The cheapest product actually was best, and many Amazon reviews seem fake. Amazon should do something about it, as its reviews used to be an awesome resource to make customer-informed purchase decisions based on crowd wisdom. This is no wonder, as all hubs came with a more-or less snarky "thank you" note which promised longer warranty or other perks in exchange for a positive Amazon review.

Credits: Photo (CC) by [Khalid Bencherifa](https://commons.m.wikimedia.org/wiki/File:USB-C_Hubb_5_portar.jpg)
