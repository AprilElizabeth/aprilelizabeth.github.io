---
layout: post
title: ThinkPad X1 Carbon 6th Gen Review
date: '2018-04-01T13:30:35-06:00'
tags:
- lenovo
- thinkpad
- x1 carbon
- mate desktop
- debian
- debian testing
- pop os
- ubuntu 18.04
image: ../../../assets/article_images/tumblr/172491079874_0.jpg
---
Before we really get started, I’d like to point out the last two posts were almost exactly the same…so. Good job.

<figure data-orig-width="4048" data-orig-height="3036" class="tmblr-full"><img src="../../../assets/article_images/tumblr/172491079874_0.jpg" data-orig-width="4048" data-orig-height="3036"></figure>

**Initial thoughts and what’s in a name**

I’ve always liked the ThinkPad, and Lenovo seems to have really found their footing in recent years. Build quality has certainly improved, and the X1 Carbon is absolutely the flagship model deserving of the ThinkPad moniker. The 6th gen seems to just be an improvement on what’s already extremely good.

I was picking up the box at UPS and immediately realized just how gosh dang _light_&nbsp;it was. It’s a 14″ ultrabook, and it’s lighter than my 12.2″ Surface Pro 4. Like, noticeably lighter and nicer to hold and carry than the Surface already. Driving home, I thought about what I’d name it, and once I opened up the box, I’d settled on Ryuko. The Lenovo red, combined with the slice-thinness, portability, and overall styling just makes me think Kill la Kill.

**Distro merry-go-round**

Debian has been my install of choice for pretty much everything but Miku (my gaming dekstop) which is running Ubuntu 17.10. While I usually settle on whatever stable is (Stretch, at time of writing) I figured an 8th gen Core i7 and Thunderbolt 3 would benefit greatly from testing, which means a 4.15 kernel and MATE Desktop 1.20! I did go through an Ubuntu 18.04 beta install, and I like it a lot, but it just didn’t feel right and seemed more buggy than what I’d consider reasonable. Losing my USB mouse and keyboard after disconnecting and reconnecting the TBT3 dock was one such bug.

I also tried out Pop!\_OS from System76, my former employer. I love the styling of Pop, the team has done some amazing work with the UI and the Pop Shop. Not to mention, the under-the-hood stuff like EFI firmware updates for S76 hardware. Cool stuff, for sure. But, old habits die really, really hard, and especially for something that I consider a work laptop or sysadmin companion. And so, I spent part of Saturday getting Debian Stretch installed, and then upgrading to Buster (current testing) which included MATE 1.20.

And lemme tell you, the wonderful folks of the MATE Desktop project have been really hard at work! It looks fresh and modern out of the box. HiDPI scaling is taken care of. Sure, some of the icon sets still look dated. It’s still a GNOME 2 fork. But it’s just so good, and so familiar. Don’t get me wrong, I’ve thoroughly enjoyed the customized Gnome shell in Ubuntu 17.10/18.04, but MATE does a very specific job of getting out of my way specifically, in a highly specified manner…while still having everything I need (system monitor, system tray, workspaces, application list…) immediately available. With this latest release, it feels so modernized in a deeply good way.

**Of course it’s still Linux**

The best and worst part of brand-new hardware is its newness. Debian Stretch wouldn’t even boot the installer in EFI mode, and I didn’t really want to waste time figuring out why. A BIOS-mode install is fine for what I’m doing, I can change it later if I really need to.

The Thunderbolt 3 dock actually worked immediately without any configuration at all. I did disable TBT3 security, though I could install thunderbolt-tools if I wanted, and it’s probably a Very Smart Idea considering the nature of Thunderbolt! But, DisplayPort at 60Hz, USB-C charging, it’s just a single-cable dream come true!

Battery life in Ubuntu was okay-ish, it seemed to be draining really fast. I did check some BIOS settings and everything looked OK, so I ended up installing TLP (it’s a ThinkPad after all!) and ran a battery drain test in a Debian live disk. There was a drastic improvement:

- Debian 9 Stretch w/ Gnome 3.22 Live  
- iwlwifi & WiFI on  
- tlp  
- LCD brightness around 60%  
- YouTube theater mode (on mute)  

…ran for about 5 hours from 87% battery. I’m excited to see what it’s like in Buster with MATE, since it’s so light.

But it wasn’t all peaches. The first night I suspended it (with Ubuntu installed) the battery drained to 2% overnight, in about 9 hours. What! That’s no good. I tried again with Debian last night, and same deal. After watching dmesg for a bit and poking around in the BIOS, I found some Thunderbolt related settings which might have been chewing through the battery. Juston’s got a Razer Blade and even his doesn’t run through battery in suspend like that. I’m expecting half to one percent lost per hour in suspend, anything less indicates some kind of issue. Of course, I made those changes right before this post, so I’ll have to test it out afterwards and see how things end up!

Otherwise, I’m really happy with the Buster install. I also took this as a good time to set up a recurring donation to the Debian project and make a one-time donation to Ubuntu as I’m not contributing in any other meaningful manner at this point in time…

**So what’s next**

I think the X1 is gonna be a great addition to my daily carry. The Intel WiFi has been working super well, and it might even replace my Latitude at the office. It might be nice to just have the X1 in my bag and a Linux desktop at the office. The X1 is definitely a better datacenter companion than the Surface, and with the WQHD screen, it’s much better than the FHD Latitude!

The only thing I’m missing right away is reading. The Surface was basically a fantastic tablet reader, and so I might look at replacing it with a large-format tablet specifically for manga and textbooks. I have been carrying around Juston’s old Kindle DX 2, but it’s dated and doesn’t seem to want to download any manga at all! Tragedy! But, I’ll manage.

I’ll kick off another suspend test after I finish this post and provide an update with the specific BIOS settings if they make a difference.

**Lenovo ThinkPad X1 Carbon 6th Generation  
As-configured**

- Processor: 8th Generation Intel® Core™ i7-8650U with vPro® (1.9GHz, up to 4.2GHz with Turbo Boost, 8MB Cache)  
- Display Type: 14.0" WQHD (2560 x 1440) IPS anti-glare  
- Memory: 16.0 GB LPDDR3 SODIMM 2133MHz  
- Hard Drive: 512 GB Solid State Drive, PCIe OPAL2.0  
- Graphics: Intel® UHD Graphics 620  
- Battery: 3 Cell Li-Polymer Battery 57WH  
- Bluetooth: Bluetooth Version 4.1  
- Camera: 720p HD & IR Camera  
- Fingerprint Reader: Fingerprint Reader  
- Keyboard: Keyboard Backlit - English  
- Wireless: Intel Dual Band Wireless AC (2 x 2) 8265  

I also purchased the Thunderbolt 3 docking station, which has been Very Good out of the box. Kernel 4.15 has done some amazing stuff for TBT3 hotplugging, making this an extremely exciting time for Linux on the desktop. Maybe 2018 is the year after all ;)

