---
title: Centrylink SSH/Telnet Botnet
date: 2021-01-10T02:41:14.955Z
author: Riverside Rocks
summary: A dig into a possible botnet with hosts on US-based ISP Centrylink.
tags:
  - botnet
---
A day or two ago I started noticing odd attacker IPs comming to my SSH port on my Pi. I'll show a few here:

![](https://cdn.riverside.rocks/a/health-barge-soul.png)
![](https://cdn.riverside.rocks/a/deal-mirror-caribou.png)

Both of these IPs come from the American ISP CenturyLink. Keep that name in mind, I'll bring it up later. After seeing these I thought, *huh, I wonder why a few IPs from the same company would be attempting to hack into my SSH. Maybe its just a coincidence?* I decided to check a few /24 blocks, [and the results were quite interesting.](https://cdn.riverside.rocks/a/cucumber-eater-warrior.mp4) Multiple IPs, sometimes up to 14 out of 256 IPs where reported in the last few days, specifically Jan. 9th.

My explantion for this? At the time I don't have one. I highly doubt it is directly being caused by the ISP as they seem like a legitmate company (verified on Twitter, I have heard of a customer), how ever it is worth noting I almost never get abuse from other US home ISPs. I'll be keeping my eyes out on this as something like this [happened in late 2020](https://dev.to/riversiderocks/the-fixed-line-mystery-46de). Back then I thought this was a few hacked hosts, but it might be a bit more.