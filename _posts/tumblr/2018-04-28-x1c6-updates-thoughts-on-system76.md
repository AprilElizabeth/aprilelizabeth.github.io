---
layout: post
title: X1C6 updates; thoughts on System76
date: '2018-04-28T21:50:09-06:00'
tags:
- x1 carbon
- debian
- linux
- lenovo
- lightdm
- system76
- thinkpad
---
<iframe style="border: 0; width: 500px; height: 120px;" src="https://bandcamp.com/EmbeddedPlayer/album=37706855/size=large/bgcol=ffffff/linkcol=63b2cc/tracklist=false/artwork=small/track=1727201182/transparent=true/" seamless=""><a href="http://iamyunomi.bandcamp.com/album/--2">ゆのもきゅ by Yunomi &amp; nicamoq</a></iframe>

Tonight has kind of a Yunomi vibe. The whole album is adorable, and tonight’s songpost choice was a close call between Makuramoto ni Ghost and Indoor Kei nara Trackmaker. Trackmaker wins. I wanted to try bandcamp embeds again, it seems to fit in a bit better.

I guess I’ve had the X1 Carbon for over a month now. As predicted, it’s been invaluable to my daily carry. I’ve been able to increase my collaboration at work, and running Linux on the metal has been really nice!

**All together now**

Even though I use a laptop (a work-issued Dell Latitude E7450, certainly no slouch) as my primary workstation, I never unplug it. It’s just enough of a hassle since, unlike the X1C, there’s no single cable solution. So, it’s unplug Ethernet, USB, mini-DP, and power, then let MATE reset for the FHD screen. And, that right there is the real hangup. I don’t have much of a point for such a tiny screen, especially when I use a 4K at home and work! I finally had a chance to take my X1C (Ryuko, remember?) to the datacenter with me yesterday, and I wasn’t fighting for screen space between a remote desktop, terminal, and browser.

So, the desk-bound Latitude wasn’t a great solution for carrying around anywhere, let alone the office. Since it’s a personal laptop, I can’t connect to the privileged WiFi, and I can’t use the VPN over the guest network. That’s a little silly, but I don’t make those rules. I can still connect to a bastion server and proxy any necessary HTTP requests through it. I used it when working through an issue with a co-worker for about 3 or 4 hours. I was happy I could be the one to travel, so they could use their primary workstation.

The X1C felt great to use on my lap or on the desk, the keyboard felt spacious and I didn’t make too many mistakes. I notice that I use the TrackPoint when I’m getting something done, and touchpad use is much more casual, like switching focus to another window, or when the laptop is further away from me. I guess if my hands aren’t actively on the keyboard, I’m more likely to use the touchpad. It was nice not having to run back to my desk and grab a charger, and when we finished up I was still at 55% from unplugging around 8am and having used it for at least one or two other meetings before. I attribute that to some power fixes I came across.

**Firmware and power troubles persist**

In my initial review, I had some issues with power which have been more-or-less resolved by a combination of an ACPI/DSDT patch and some BIOS tweaking. I’d share more, but the [Arch wiki](https://wiki.archlinux.org/index.php/Lenovo_ThinkPad_X1_Carbon_(Gen_6)) is better and updated more frequently. I’d like to try the Si03 support mentioned there, but I probably won’t until a kernel update comes along and I have to go touch the GRUB config again.

The only other problem I’ve had is, sometimes after resume, the brightness hotkeys stop working until LightDM is restarted. It’s not spine-breaking, but my eyes are pretty sensitive at night and I usually set the brightness down to minimum. I’m sure I could hack around it with xbacklight, but so far it’s only enough of an annoyance to write about and not actually _do_&nbsp;anything about…

I did get redshift installed and configured, which helps with nighttime brightness. I guess I’ve had f.lux or similar installed since working the NOC night shift a decade ago. Helpful, but not a replacement for brightness controls.

**Why not System76?**

The X1C has certainly become a talking point around my desk as well. Some of the other engineers and developers are asking what it took to get Linux installed, and one remarked it was interesting that I didn’t choose a System76. I explained how I found the true value of System76 to be for users who want a seamless Linux experience out of the box, or awesome lifetime OS support. For real, the level of detail that support team goes into, and how they seamlessly adapt for the customer’s technical competency level is unmatched in the industry. If anyone is making Linux on the desktop friendly and within-reach, it’s System76. I think that’s even more true with their work on Pop!\_OS. They’re laser-focused on user experience from start to finish, for first-timers and longtime users alike.

While working there, and even now, my only contention is the laptop build quality. It’s not bad, by any means, and the machines themselves are highly configurable and user-serviceable. But, working in support, I saw hardware failures that didn’t inspire confidence. The designs, while improving significantly, felt somewhat dated. Laptop screens had flex or bezel gaps. Battery life was…not good. As someone who highly appreciates, but does not _need_ the level of support provided by the team, I opted to get exactly what I wanted. I was shopping for a little while, and I _really_&nbsp;miss the level of testing that went into Ubuntu on S76 machines. I do feel a little twinge of regret with this silly backlight issue, knowing how we’d run _fwts_&nbsp;(firmware test suite) suspend tests over the weekend to make sure the little details like that were perfect for the end-user. They’ve expanded the QA team and now have dedicated testing staff, so it’s only getting better.

Happily, there’s light at the end of the hardware tunnel. They’ve recently announced a huge step in a long, _long_ initiative to begin manufacturing their own custom-designed laptops right here in Denver. I remember getting product requests and wishlists from customers who all had an ideal laptop in mind. Truthfully, they all sound a lot like the X1C. Of course, ThinkPads are longtime fan-favorites for Linux users! Many of them would write,&nbsp;“If you do [x y z] with the laptop, I’ll for be buying it for sure!” It was really good to see, knowing there was community support for a hardware initiative. I think it’s a good move. I’m really interested to watch the team handle a software (Pop!\_OS) and hardware initiative simultaneously. It feels…_ambitious._ That’s not to say I don’t think they can do it; quite the opposite. If any team is gonna pull it off, this is the one.

I wasn’t exactly expecting to share or include thoughts on a former employer and possible vendor, but it’s a little difficult not to address. I’m certain the team knows I wish them the best, and that I’m as excited as anyone else to see what comes next! I know they’re collecting thoughts and feedback, and I’d encourage them to not forget the amazing support team alongside the new initiatives, because they’re the golden ticket to widespread adoption.

I guess that’s about it. Though, it’s a little funny that I’m writing this on my custom-built desktop and not my&nbsp;好きなもの ThinkPad.

